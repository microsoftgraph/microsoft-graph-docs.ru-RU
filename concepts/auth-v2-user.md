---
title: Получение доступа от имени пользователя
description: Для чтения и записи ресурсов от имени пользователя с помощью Microsoft Graph ваше приложение должно получать маркер доступа из Azure AD и вкладывать этот маркер в запросы для Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: graphiamtop20
ms.openlocfilehash: d2b3c7a26a0a4d5005f22893e0295585f5e7033b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846158"
---
# <a name="get-access-on-behalf-of-a-user"></a>Получение доступа от имени пользователя

To use Microsoft Graph to read and write resources on behalf of a user, your app must get an access token from the Microsoft identity platform and attach the token to requests that it sends to Microsoft Graph. The exact authentication flow that you will use to get access tokens will depend on the kind of app you are developing and whether you want to use OpenID Connect to sign the user in to your app. One common flow used by native and mobile apps and also by some Web apps is the OAuth 2.0 authorization code grant flow. This topic  walks through an example using this flow.

## <a name="authentication-and-authorization-steps"></a>Этапы проверки подлинности и авторизации

Ниже перечислены основные действия, необходимые для получения маркера доступа из конечной точки платформы удостоверений Майкрософт с помощью потока предоставления кода авторизации OAuth 2.0.

1. Регистрация приложения в Azure AD.
2. Получение авторизации.
3. Получение маркера доступа.
4. Вызовы Microsoft Graph с помощью маркера доступа.
5. Получение нового маркера доступа с помощью маркера обновления.

## <a name="1-register-your-app"></a>1. Регистрация приложения

To use the Microsoft identity platform endpoint, you must register your app using the Azure [app registration portal](https://go.microsoft.com/fwlink/?linkid=2083908). You can use either a Microsoft account or a work or school account to register an app.

Чтобы настроить приложение на использование потока предоставления кода авторизации OAuth 2.0, во время регистрации приложения необходимо сохранить следующие значения:

- идентификатор приложения (клиента), назначенный порталом регистрации;
- секрет клиента (приложения) — пароль либо открытый и закрытый ключ (сертификат). Это необязательно для нативных приложений;
- URI перенаправления (или URL-адрес ответа), с помощью которого приложение будет получать отклики от Azure AD.

Инструкции по настройке приложения на портале Azure см. в статье [Регистрация приложения](./auth-register-app-v2.md).

## <a name="2-get-authorization"></a>2. Получение авторизации

Чтобы получить маркер доступа для многих потоков OpenID Connect и OAuth 2.0, сначала необходимо перенаправить пользователя к конечной точке `/authorize` платформы удостоверений Майкрософт. Azure AD обеспечит вход пользователя и запрашивание его согласия на предоставление приложению необходимых разрешений. В потоке предоставления кода авторизации после получения согласия Azure AD возвращает приложению код авторизации, который оно может передать конечной точке `/token` платформы удостоверений Майкрософт, чтобы получить маркер доступа.

### <a name="authorization-request"></a>Запрос авторизации

Ниже представлен пример запроса для конечной точки `/authorize`.

При использовании конечной точки платформы удостоверений Майкрософт разрешения запрашиваются с помощью параметра `scope`. В этом примере запрашиваются разрешения Microsoft Graph _User.Read_ и _Mail.Read_, которые позволяют приложению просматривать профиль и почту вошедшего пользователя. Разрешение _offline\_access_ запрашивается, чтобы приложение могло получить маркер обновления, с помощью которого оно сможет получить новый маркер доступа, когда истечет срок действия текущего.

```
// Line breaks for legibility only

https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize?
client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&response_type=code
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&response_mode=query
&scope=offline_access%20user.read%20mail.read
&state=12345
```

| Параметр     | Обязательный    | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| tenant        | обязательно    | The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id     | обязательно    | Идентификатор приложения, назначенный [порталом регистрации](https://go.microsoft.com/fwlink/?linkid=2083908) для приложения.                                                                                                                                                                                                                                                                                                                                                                                   |
| response_type | Обязательный    | Должен включать значение `code` для потока кода авторизации.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| redirect_uri  | Рекомендуемый | The redirect_uri of your app, where authentication responses can be sent and received by your app.  It must exactly match one of the redirect_uris you registered in the app registration portal, except it must be URL encoded.  For native and mobile apps, you should use the default value of `https://login.microsoftonline.com/common/oauth2/nativeclient`.                                                                                                                                       |
| область         | обязательно    | A space-separated list of the Microsoft Graph permissions that you want the user to consent to. This may also include OpenID scopes.                                                                                                                                                                                                                                                                                                                                                                    |
| response_mode | Рекомендуемый | Specifies the method that should be used to send the resulting token back to your app.  Can be `query` or `form_post`.                                                                                                                                                                                                                                                                                                                                                                                  |
| состояние         | Рекомендуемый | A value included in the request that will also be returned in the token response.  It can be a string of any content that you wish.  A randomly generated unique value is typically used for [preventing cross-site request forgery attacks](https://tools.ietf.org/html/rfc6749#section-10.12).  The state is also used to encode information about the user's state in the app before the authentication request occurred, such as the page or view they were on.                                     |

> **Important**: Microsoft Graph exposes two kinds of permissions: application and delegated. For apps that run with a signed-in user, you request delegated permissions in the `scope` parameter. These permissions delegate the privileges of the signed-in user to your app, allowing it to act as the signed-in user when making calls to Microsoft Graph. For more detailed information about the permissions available through Microsoft Graph, see the [Permissions reference](./permissions-reference.md).

### <a name="consent-experience"></a>Предоставление согласия

На этом этапе пользователю предлагается указать свои учетные данные для проверки подлинности с помощью Майкрософт. Конечная точка платформы удостоверений Майкрософт версии 2.0 также обеспечивает согласие пользователя на предоставление указанных разрешений с помощью параметра запроса `scope`.  Если пользователь не согласился предоставить какое-либо из этих разрешений, а администратор не давал предварительного согласия от имени всех пользователей в организации, пользователям будет предложено согласиться предоставить необходимые разрешения.

Ниже представлен пример диалогового окна согласия для учетной записи Майкрософт.

![Диалоговое окно согласия для учетной записи Майкрософт](./images/v2-consumer-consent.png)

> **Try** If you have a Microsoft account or an Azure AD work or school account, you can try this for yourself by clicking the following link. After signing in, your browser should be redirected to `https://localhost/myapp/` with a `code` in the address bar.
>
> <a href="https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F&response_mode=query&scope=offline_access%20user.read%20mail.read&state=12345" target="_blank">https://login.microsoftonline.com/common/oauth2/v2.0/authorize...</a>

### <a name="authorization-response"></a>Отклик на авторизацию

If the user consents to the permissions your app requested, the response will contain the authorization code in the `code` parameter. Here is an example of a successful response to the previous request. Because the `response_mode` parameter in the request was set to `query`, the response is returned in the query string of the redirect URL.

```
GET https://localhost/myapp/?
code=M0ab92efe-b6fd-df08-87dc-2c6500a7f84d
&state=12345
```

| Параметр | Описание                                                                                                                                                                                                                        |
|-----------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| code      | The authorization_code that the app requested. The app can use the authorization code to request an access token for the target resource.  Authorization_codes are very short lived, typically they expire after about 10 minutes. |
| состояние     | If a state parameter is included in the request, the same value should appear in the response. The app should verify that the state values in the request and response are identical.                                              |

## <a name="3-get-a-token"></a>3. Получение маркера

Приложение использует значение `code` (код авторизации), полученное на предыдущем этапе, чтобы запрашивать маркер доступа путем отправки запроса `POST` конечной точке `/token`.

### <a name="token-request"></a>Запрос на получение маркера

```
// Line breaks for legibility only

POST /{tenant}/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

| Параметр     | Обязательный              | Описание                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| tenant        | обязательно              | The `{tenant}` value in the path of the request can be used to control who can sign into the application.  The allowed values are `common` for both Microsoft accounts and work or school accounts, `organizations` for work or school accounts only, `consumers` for Microsoft accounts only, and tenant identifiers such as the tenant ID or domain name.  For more detail, see [protocol basics](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints). |
| client_id     | обязательно              | Идентификатор приложения, назначенный [порталом регистрации](https://go.microsoft.com/fwlink/?linkid=2083908) для приложения.                                                                                                                                                                                                                                                                                                                                                                                  |
| grant_type    | Обязательный              | Должно быть задано значение `authorization_code` для потока кода авторизации.                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| scope         | обязательно              | A space-separated list of scopes.  The scopes requested in this leg must be equivalent to or a subset of the scopes requested in the first (authorization) leg.  If the scopes specified in this request span multiple resource servers, then the v2.0 endpoint will return a token for the resource specified in the first scope.                                                                                                                                                                      |
| code          | Обязательный              | Код авторизации, полученный на первом этапе потока.                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| redirect_uri  | Обязательный              | То же значение URI перенаправления, которое использовалось для получения кода авторизации.                                                                                                                                                                                                                                                                                                                                                                                                                            |
| client_secret | Обязательный для веб-приложений | The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side.                                                                                                                                                                                     |

### <a name="token-response"></a>Ответ с маркером

Несмотря на то что маркер доступа непрозрачен для приложения, отклик содержит список разрешений, для которых подходит маркер, в параметре `scope`.

```json
{
    "token_type": "Bearer",
    "scope": "user.read%20Fmail.read",
    "expires_in": 3600,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4..."
}
```

| Параметр     | Описание                                                                                                                                                                                                                                                                                                                                                                                  |
|---------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| token_type    | Indicates the token type value. The only type that Azure AD supports is Bearer.                                                                                                                                                                                                                                                                                                              |
| область         | Разделенный пробелами список разрешений Microsoft Graph, для которых действителен маркер доступа.                                                                                                                                                                                                                                                                                                |
| expires_in    | Срок действия маркера доступа (в секундах).                                                                                                                                                                                                                                                                                                                                             |
| access_token  | The requested access token. Your app can use this token to call Microsoft Graph.                                                                                                                                                                                                                                                                                                             |
| refresh_token | Маркер обновления OAuth 2.0. С его помощью приложение сможет запрашивать дополнительные маркеры доступа, когда истечет срок действия текущего.  Маркеры обновления имеют большие сроки действия, и с их помощью можно сохранять доступ к ресурсам в течение длительного времени.  Дополнительные сведения см. в [справочнике по маркерам версии 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-tokens). |

## <a name="4-use-the-access-token-to-call-microsoft-graph"></a>4. Вызов Microsoft Graph с помощью маркера доступа

After you have an access token, you can use it to call Microsoft Graph by including it in the `Authorization` header of a request. The following request gets the profile of the signed-in user.

```
GET https://graph.microsoft.com/v1.0/me
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com

```

Успешный ответ выглядит приблизительно следующим образом (некоторые заголовки были удалены).

```
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 727.0022
Date: Thu, 20 Apr 2017 05:21:18 GMT
Content-Length: 407

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="5-use-the-refresh-token-to-get-a-new-access-token"></a>5. Получение нового маркера доступа с помощью маркера обновления

Access tokens are short lived, and you must refresh them after they expire to continue accessing resources.  You can do so by submitting another `POST` request to the `/token` endpoint, this time providing the `refresh_token` instead of the `code`.

### <a name="request"></a>Запрос

```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&refresh_token=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=refresh_token
&client_secret=JqQX2PNo9bpM0uEihUPzyrh      // NOTE: Only required for web apps
```

| Параметр     | Обязательный              | Описание                                                                                                                                                                                                                                                                                                         |
|---------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| client_id     | обязательно              | Идентификатор приложения, назначенный [порталом регистрации](https://go.microsoft.com/fwlink/?linkid=2083908) для приложения.                                                                                                                                                                                               |
| grant_type    | Обязательный              | Должно быть задано значение `refresh_token`.                                                                                                                                                                                                                                                                                            |
| scope         | обязательно              | A space-separated list of permissions (scopes).  The permissions requested must be equivalent to or a subset of the permissions requested in the original authorization_code request.                                                                                                                               |
| refresh_token | Обязательный              | Маркер обновления, полученный с помощью запроса на получение маркера.                                                                                                                                                                                                                                                       |
| redirect_uri  | Обязательный              | То же значение URI перенаправления, которое использовалось для получения кода авторизации.                                                                                                                                                                                                                                        |
| client_secret | Обязательный для веб-приложений | The application secret that you created in the app registration portal for your app.  It should not be used in a native app, because client_secrets cannot be reliably stored on devices.  It is required for web apps and web APIs, which have the ability to store the client_secret securely on the server side. |

### <a name="response"></a>Отклик

Успешный отклик с маркером будет выглядеть примерно так:

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "token_type": "Bearer",
    "expires_in": 3599,
    "scope": "user.read%20mail.read",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4...",
}
```
| Параметр     | Описание                                                                                                                                                                        |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| access_token  | The requested access token. The app can use this token in calls to Microsoft Graph.                                                                                                |
| token_type    | Indicates the token type value. The only type that Azure AD supports is Bearer                                                                                                     |
| expires_in    | Срок действия маркера доступа (в секундах).                                                                                                                                   |
| scope         | Разрешения (области), для которых действителен маркер доступа.                                                                                                                       |
| refresh_token | A new OAuth 2.0 refresh token. You should replace the old refresh token with this newly acquired refresh token to ensure your refresh tokens remain valid for as long as possible. |

## <a name="supported-app-scenarios-and-additional-resources"></a>Поддерживаемые сценарии приложений и дополнительные ресурсы

Вы можете вызывать Microsoft Graph от имени пользователя из приложений следующих типов:

- [Нативные или мобильные приложения](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-overview)
- [Веб-приложения](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview)
- [Одностраничные приложения (SPA)](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-overview)
- [Внутренние веб-API](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview) (к примеру, когда клиентское приложение, например нативное, реализует функции в серверной части веб-API). При использовании конечной точки платформы удостоверений Майкрософт у клиентского приложения и внутреннего веб-API должны быть одинаковые идентификаторы приложения.

Дополнительные сведения о поддерживаемых сценариях приложений с конечной точкой платформы удостоверений Майкрософт см. в статье [Сценарии приложений и потоки проверки подлинности](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios).

> **Примечание**. Вызов Microsoft Graph из отдельного веб-API в настоящее время не поддерживается конечной точкой платформы удостоверений Майкрософт. Для этого сценария необходимо использовать конечную точку Azure AD.

Дополнительные сведения о получении доступа к Microsoft Graph от имени пользователя из конечной точки платформы удостоверений Майкрософт:

- Ссылки на документацию по протоколам и руководства по началу работы для различных типов приложений см. в [документации по конечным точкам платформы удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview).
- Дополнительные сведения о поддерживаемых типах приложений и потоках проверки подлинности см. в статье [Типы приложений версии 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types).
- Дополнительные сведения о рекомендуемых библиотеках проверки подлинности и серверном ПО промежуточного слоя (как от корпорации Майкрософт, так и от сторонних разработчиков) для платформы удостоверений Майкрософт см. в статье [Библиотеки проверки подлинности Azure Active Directory версии 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries).

## <a name="endpoint-considerations"></a>Рекомендации, связанные с конечной точкой

Корпорация Майкрософт продолжает поддерживать конечную точку Azure AD. Существует [ряд отличий](https://docs.microsoft.com/azure/active-directory/develop/azure-ad-endpoint-comparison) между конечной точкой платформы удостоверений Майкрософт и конечной точкой Azure AD. При использовании конечной точки Azure AD:

- Для каждой платформы приложению потребуется отдельный идентификатор (идентификатор клиента).
- Если приложение поддерживается несколькими клиентами, необходимо в явной форме настроить его в таком качестве на [портале Azure](https://portal.azure.com).
- Все разрешения, необходимые приложению, должен настроить разработчик. Конечная точка Azure AD не поддерживает динамическое (добавочное) согласие.
- The Azure AD endpoint uses a `resource` parameter in authorization and token requests to specify the resource, such as Microsoft Graph, for which it wants permissions. The endpoint does not support the `scope` parameter.
- The Azure AD endpoint does not expose a specific endpoint for administrator consent. Instead apps use the `prompt=admin_consent` parameter in the authorization request to obtain administrator consent for an organization. For more information, see **Triggering the Azure AD consent framework at runtime** in [Integrating applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications).

Дополнительные сведения о получении доступа к Microsoft Graph от имени пользователя из конечной точки Azure AD:

- Дополнительные сведения об использовании конечной точки платформы удостоверений Майкрософт для различных типов приложений см. по ссылкам **Начало работы** в [документации для разработчиков по платформе удостоверений Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide). Документация содержит ссылки на обзорные статьи, краткие руководства, учебники, примеры кода и документацию по протоколам для различных типов приложений, поддерживаемых конечной точкой платформы удостоверений Майкрософт.
- Сведения о библиотеке проверки подлинности Майкрософт (MSAL) и серверном ПО промежуточного слоя, доступном для использования с конечной точкой платформы удостоверений Майкрософт, см. в статье [Библиотеки проверки подлинности Майкрософт](https://docs.microsoft.com/azure/active-directory/develop/msal-overview).
