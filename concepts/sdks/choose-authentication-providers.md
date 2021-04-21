---
title: Выберите поставщика проверки подлинности Microsoft Graph
description: Узнайте, как выбрать поставщиков проверки подлинности по сценарию для приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 726fbf1334a99ab6a854bd4627052d154187105c
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921128"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Выберите поставщика проверки подлинности Microsoft Graph в зависимости от сценария

Поставщики проверки подлинности реализуют код, необходимый для приобретения маркера с помощью Библиотеки проверки подлинности Майкрософт (MSAL); обработка ряда потенциальных ошибок для таких случаев, как постепенное согласие, просроченные пароли и условный доступ; а затем установите заглавную головку авторизации http-запроса. В следующей таблице перечислены поставщики, которые соответствуют сценариям для различных [типов приложений.](/azure/active-directory/develop/v2-app-types)

|Сценарий | Flow/Grant | Аудитория | Поставщик|
|--|--|--|--|
| [Приложение для одной страницы](/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | Неявный поток | Делегированная потребительская/org |[Неявный поставщик](#ImplicitProvider) |
| [Веб-приложение, которое вызывает веб-API](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | Authorization Code | Делегированная потребительская/org | [Поставщик кода авторизации](#AuthCodeProvider) |
| | Учетные данные клиента  | Только приложение | [Поставщик учетных данных клиента](#ClientCredentialsProvider) |
| [Веб-API, который вызывает веб-API](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | От имени | Делегированная потребительская/org | [От имени поставщика](#OnBehalfOfProvider) |
| | Учетные данные клиента  | Только приложение | [Поставщик учетных данных клиента](#ClientCredentialsProvider) |
| [Настольное приложение, которое вызывает веб-API](/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | Интерактивны | Делегированная потребительская/org | [Интерактивный поставщик](#InteractiveProvider) |
| | Интегрированная Windows | Делегированная org | [Интегрированный поставщик Windows](#IntegratedWindowsProvider) |
| | Владелец ресурса  | Делегированная org | [Имя пользователя / Поставщик паролей](#UsernamePasswordProvider) |
| | Код устройства  | Делегированная org | [Поставщик кода устройства](#DeviceCodeProvider) |
| [Приложение Daemon](/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | Учетные данные клиента  | Только приложение | [Поставщик учетных данных клиента](#ClientCredentialsProvider) |
| [Мобильное приложение, которое вызывает веб-API](/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | Интерактивны | Делегированная потребительская/org | [Интерактивный поставщик](#InteractiveProvider) |

> Примечание. Разработчикам Java и Android необходимо добавить библиотеку [azure-identity,](/java/api/overview/azure/identity-readme?view=azure-java-stable) чтобы получить доступ к различным типам учетных данных.

## <a name="authorization-code-provider"></a><a name="AuthCodeProvider" ></a>Поставщик кода авторизации

Поток кода авторизации позволяет родным и веб-приложениям безопасно получать маркеры от имени пользователя. Дополнительные данные см. в записи платформы удостоверений Майкрософт и потока кода авторизации [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-auth-code-flow)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время. Дополнительные сведения см. в [специальном поставщике проверки подлинности.](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)

# <a name="java"></a>[Java](#tab/Java)

```java
final AuthorizationCodeCredential authCodeCredential = new AuthorizationCodeCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret) //required for web apps, do not set for native apps
        .authorizationCode(authorizationCode)
        .redirectUrl(redirectUri)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, authCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Еще не доступно. Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступна. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

---

##  <a name="client-credentials-provider"></a><a name="ClientCredentialsProvider"></a>Поставщик учетных данных клиента

Поток клиентских учетных данных позволяет приложениям-службам работать без взаимодействия с пользователем. Доступ основан на удостоверении приложения. Дополнительные сведения см. в веб-сайте Платформы удостоверений Майкрософт и потока учетных данных клиента [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время. Дополнительные сведения см. в [специальном поставщике проверки подлинности.](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)

# <a name="java"></a>[Java](#tab/Java)

```java
final ClientSecretCredential clientSecretCredential = new ClientSecretCredentialBuilder()
        .clientId(clientId)
        .clientSecret(clientSecret)
        .tenantId(tenant)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, clientSecretCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Пока недоступна. Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступна. Пожалуйста, поддержите или откройте [запрос на функцию Microsoft Graph,](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) если это важно для вас.

---

##  <a name="on-behalf-of-provider"></a><a name="OnBehalfOfProvider"></a>От имени поставщика

Поток от имени применим, когда приложение вызывает API службы/веб-службы, который по очереди вызывает API Microsoft Graph. Узнайте больше, прочитав платформу удостоверений Майкрософт и [поток OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время. Дополнительные сведения читайте в [публикации "Использование](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) поставщика настраиваемой проверки подлинности".

# <a name="java"></a>[Java](#tab/Java)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

---

## <a name="implicit-provider"></a><a name="ImplicitProvider"></a>Неявный поставщик

Неявный поток грантов используется в браузерных приложениях. Дополнительные сведения см. в [записи платформы удостоверений Майкрософт и потока неявных грантов.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)

# <a name="c"></a>[C#](#tab/CS)

Неприменимо.

# <a name="javascript"></a>[Javascript](#tab/Javascript)

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
const authProvider = new MicrosoftGraph.ImplicitMSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="java"></a>[Java](#tab/Java)

Неприменимо.

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

##  <a name="device-code-provider"></a><a name="DeviceCodeProvider"></a>Поставщик кода устройств

Поток кода устройства позволяет войти на устройства с помощью другого устройства. Подробные сведения см. в материале Платформа удостоверений Майкрософт и поток кода [кода устройств OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-device-code)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

# <a name="java"></a>[Java](#tab/Java)

```java
final DeviceCodeCredential deviceCodeCredential = new DeviceCodeCredentialBuilder()
                    .clientId(clientId)
                    .challengeConsumer(challenge -> {
                        // lets user know of the challenge
                        System.out.println(challenge.getMessage());
                    })
                    .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, deviceCodeCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

---

##  <a name="integrated-windows-provider"></a><a name="IntegratedWindowsProvider"></a>Интегрированный поставщик Windows

Интегрированный поток Windows позволяет компьютерам Windows безмолвно приобретать маркер доступа при присоединении к домену. Подробные сведения см. [в материале Интегрированная проверка подлинности Windows.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Неприменимо.

# <a name="java"></a>[Java](#tab/Java)

Неприменимо.

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

##  <a name="interactive-provider"></a><a name="InteractiveProvider"></a>Интерактивный поставщик

Интерактивный поток используется мобильными приложениями (Xamarin и UWP) и настольными приложениями для вызова Microsoft Graph от имени пользователя. Подробные сведения см. [в материале Эквайринг маркеров в интерактивном режиме.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)

# <a name="c"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

# <a name="java"></a>[Java](#tab/Java)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

```java
final InteractiveBrowserCredential interactiveBrowserCredential = new InteractiveBrowserCredentialBuilder()
                .clientId(clientId)
                .redirectUrl("http://localhost:8765")
                .build();
final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, interactiveBrowserCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[PHP](#tab/PHP)

Неприменимо.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Неприменимо.

---

##  <a name="usernamepassword-provider"></a><a name="UsernamePasswordProvider"></a>Поставщик имен пользователей и паролей

Поставщик имен пользователей и паролей позволяет приложению войти в пользователя с помощью имени пользователя и пароля. Используйте этот поток только в том случае, если вы не можете использовать другие потоки OAuth. Дополнительные сведения см. в веб-сайте Платформы удостоверений Майкрософт и учетных данных владельца паролей владельца ресурсов [OAuth 2.0.](/azure/active-directory/develop/v2-oauth-ropc)



# <a name="c"></a>[C#](#tab/CS)

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

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

# <a name="java"></a>[Java](#tab/Java)

```java
final UsernamePasswordCredential usernamePasswordCredential = new UsernamePasswordCredentialBuilder()
        .clientId(clientId)
        .username(username)
        .password(password)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, usernamePasswordCredential);

final GraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(tokenCredentialAuthProvider)
    .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Еще не доступно. Если это важно, проголосуйте за или откройте запрос на функцию [Microsoft Graph.](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)

---

## <a name="next-steps"></a>Дальнейшие действия

* Поставщикам проверки подлинности требуется идентификация клиента. Вы захотите [зарегистрировать свое приложение после](https://portal.azure.com/) того, как настроите поставщика проверки подлинности.
* Дайте нам знать, если необходимый поток OAuth в настоящее время не поддерживается путем голосования или открытия запроса [функции Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).