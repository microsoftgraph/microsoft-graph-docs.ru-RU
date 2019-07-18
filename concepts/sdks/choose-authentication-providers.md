---
title: Выбор поставщика проверки подлинности Microsoft Graph
description: Сведения о том, как выбрать поставщиков проверки подлинности для конкретного сценария для вашего приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 7975a2049ee16d89cfc9668babde091db7dd140e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778301"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Выбор поставщика проверки подлинности Microsoft Graph на основе сценария

Поставщики проверки подлинности реализуют код, необходимый для получения маркера с помощью библиотеки проверки подлинности Microsoft (MSAL); обрабатывать ряд потенциальных ошибок в случае появления добавочного согласия, просроченных паролей и условного доступа; а затем задайте заголовок авторизации HTTP-запроса. В следующей таблице перечислены поставщики, которые отвечают сценариям для различных [типов приложений](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).

|Сценарий | Flow/Grant | Аудитория | Поставщик|
|--|--|--|--|
| [Приложение с одной страницей](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | Неявный поток | Делегированный потребитель/org |[Неявный поставщик](#ImplicitProvider) |
| [Веб-приложение, вызывающее веб-API](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | Authorization Code | Делегированный потребитель/org | [Поставщик кода авторизации](#AuthCodeProvider) |
| | Учетные данные клиента  | Только приложение | [Поставщик учетных данных клиента](#ClientCredentialsProvider) |
| [Веб-API, вызывающий веб-API](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | От имени | Делегированный потребитель/org | [От имени поставщика](#OnBehalfOfProvider) |
| | Учетные данные клиента  | Только приложение | [Поставщик учетных данных клиента](#ClientCredentialsProvider) |
| [Классическое приложение, вызывающее веб-API](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | Интерактивны | Делегированный потребитель/org | [Интерактивный поставщик](#InteractiveProvider) |
| | Интегрированная система Windows | Делегированная org | [Интегрированный поставщик Windows](#IntegratedWindowsProvider) |
| | Владелец ресурса  | Делегированная org | [Имя пользователя и поставщик паролей](#UsernamePasswordProvider) |
| | Код устройства  | Делегированная org | [Поставщик кода устройства](#DeviceCodeProvider) |
| [Приложение демона](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | Учетные данные клиента  | Только приложение | [Поставщик учетных данных клиента](#ClientCredentialsProvider) |
| [Мобильное приложение, вызывающее веб-API](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | Интерактивны | Делегированный потребитель/org | [Интерактивный поставщик](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><a name="AuthCodeProvider"/>Поставщик кода авторизации

Потоки кода авторизации позволяют встроенным и веб-приложениям безопасно получать маркеры в имени пользователя. Для получения дополнительных сведений см [код кода авторизации платформы Microsoft Identity и OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);  
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности. Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)подлинности.

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><a name="ClientCredentialsProvider"/>Поставщик учетных данных клиента

Поток учетных данных клиента позволяет приложениям службы работать без взаимодействия с пользователем. Доступ зависит от удостоверения приложения. Дополнительные сведения см. [в статье платформа идентификации Майкрософт и процесс учетных данных клиента OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности. Дополнительные сведения см. в разделе [Использование настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)подлинности.

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><a name="OnBehalfOfProvider"/>Поставщик от имени

Потоки "от имени" применяются, когда приложение вызывает службу или веб-API, которые в своюмся вызывает API Microsoft Graph. Узнайте больше, прочитав [платформу Microsoft Identity и OAuth 2,0 от имени по поручению](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

В настоящее время код авторизации, учетные данные клиента и потоки OAuth "от имени" требуют реализации настраиваемого поставщика проверки подлинности. Для получения дополнительных сведений ознакомьтесь [с использованием настраиваемого поставщика проверки](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) подлинности.

# <a name="javatabjava"></a>[Java](#tab/Java)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><a name="ImplicitProvider"/>Неявный поставщик

Неявный поток предоставления используется в приложениях, основанных на браузерах. Для получения дополнительных сведений см [Microsoft Identity Platform и неявный поток предоставления разрешений](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).

# <a name="ctabcs"></a>[C#](#tab/CS)

Неприменимо.

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

```javascript
const clientId = "your_client_id"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new Msal.UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MicrosoftGraph.MSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[Java](#tab/Java)

Неприменимо.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><a name="DeviceCodeProvider"/>Поставщик кода устройства

Потоки кода устройства позволяют выполнять вход на устройства с помощью другого устройства. Дополнительные сведения см. [в статье платформа идентификации Майкрософт и код устройства OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="javatabjava"></a>[Java](#tab/Java)

Пока недоступно. Поддержка или открытие [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) , если это важно.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><a name="IntegratedWindowsProvider"/>Интегрированный поставщик Windows

Интегрированный поток Windows предоставляет компьютеру Windows способ получить маркер доступа без уведомления при присоединении к домену. Подробнее: встроенная [Проверка подлинности Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

Неприменимо.

# <a name="javatabjava"></a>[Java](#tab/Java)

Неприменимо.

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><a name="InteractiveProvider"/>Интерактивный поставщик

Интерактивный обмен используется приложениями для мобильных устройств (Xamarin и UWP) и приложениями для настольных ПК, чтобы вызывать Microsoft Graph в имени пользователя. Дополнительные сведения см в разделе [получение маркеров в интерактивном режиме](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="javatabjava"></a>[Java](#tab/Java)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="androidtabandroid"></a>[Android](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "CLIENT_ID_OF_YOUR_APPLICATION");
MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(msalAuthenticationProvider)
    .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><a name="UsernamePasswordProvider"/>Имя пользователя и поставщик паролей

Поставщик имени пользователя и пароля позволяет приложению выполнять вход в систему, используя имя пользователя и пароль. Используйте этот поток, только если вы не можете использовать другие потоки OAuth. Для получения дополнительных сведений см [платформа идентификации Майкрософт и учетные данные пароля владельца ресурса OAuth 2,0](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)



# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

UsernamePasswordProvider authProvider = new UsernamePasswordProvider(publicClientApplication, scopes);

GraphServiceClient graphClient = new GraphServiceClient(authProvider);

User me = await graphClient.Me.Request()
                .WithUsernamePassword(email, password)
                .GetAsync();
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/Objective-C)

Неприменимо.

# <a name="phptabphp"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проведите голосование или откройте [запрос функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) .

---

## <a name="next-steps"></a>Дальнейшие действия

* Для поставщиков проверки подлинности требуется идентификатор клиента. Вы захотите [зарегистрировать приложение](https://portal.azure.com/) после настройки поставщика проверки подлинности.
* Сообщите нам, если требуемый потоки OAuth в настоящее время не поддерживается голосованием или открытием [запроса функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
