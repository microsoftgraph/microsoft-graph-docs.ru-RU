---
title: Выберите поставщика проверки подлинности Graph Майкрософт
description: Узнайте, как выбрать поставщиков проверки подлинности по сценарию для приложения.
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: ff898f69c2d23575e3b7c64ced22899839c11504
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264047"
---
<!-- markdownlint-disable MD001 MD024 MD025 -->

# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Выбор поставщика проверки подлинности Microsoft Graph на основе сценария

Поставщики проверки подлинности реализуют код, необходимый для приобретения маркера с помощью Библиотеки проверки подлинности Майкрософт (MSAL); обработка ряда потенциальных ошибок для таких случаев, как постепенное согласие, просроченные пароли и условный доступ; а затем установите заглавную головку авторизации http-запроса. В следующей таблице перечислены поставщики, которые соответствуют сценариям для различных [типов приложений.](/azure/active-directory/develop/v2-app-types)

| Сценарий                                                                                               | Flow/Grant         | Аудитория               | Поставщик |
|--------------------------------------------------------------------------------------------------------|--------------------|------------------------|-----|
| [Приложение для одной страницы](/azure/active-directory/develop/scenario-spa-acquire-token)                          |                    |                        |     |
|                                                                                                        | Неявный поток           | Делегированная потребительская/org | [Неявный поставщик](#implicit-provider) |
| [Веб-приложение, которое вызывает веб-API](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | Authorization Code | Делегированная потребительская/org | [Поставщик кода авторизации](#authorization-code-provider) |
|                                                                                                        | Учетные данные клиента | Только приложение               | [Поставщик учетных данных клиента](#client-credentials-provider) |
| [Веб-API, который вызывает веб-API](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | От имени       | Делегированная потребительская/org | [От имени поставщика](#on-behalf-of-provider) |
|                                                                                                        | Учетные данные клиента | Только приложение               | [Поставщик учетных данных клиента](#client-credentials-provider) |
| [Настольное приложение, которое вызывает веб-API](/azure/active-directory/develop/scenario-desktop-acquire-token)      |                    |                        |     |
|                                                                                                        | Интерактивны        | Делегированная потребительская/org | [Интерактивный поставщик](#interactive-provider) |
|                                                                                                        | Интегрированные Windows | Делегированная org          | [Интегрированный Windows поставщик](#integrated-windows-provider) |
|                                                                                                        | Владелец ресурса     | Делегированная org          | [Поставщик имен пользователей и паролей](#usernamepassword-provider) |
|                                                                                                        | Код устройства        | Делегированная org          | [Поставщик кода устройств](#device-code-provider) |
| [Приложение Daemon](/azure/active-directory/develop/scenario-daemon-acquire-token)                            |                    |                        |     |
|                                                                                                        | Учетные данные клиента | Только приложение               | [Поставщик учетных данных клиента](#client-credentials-provider) |
| [Мобильное приложение, которое вызывает веб-API](/azure/active-directory/develop/scenario-mobile-acquire-token)        |                    |                        |     |
|                                                                                                        | Интерактивны        | Делегированная потребительская/org | [Интерактивный поставщик](#interactive-provider) |

> [!NOTE]
> Разработчикам Java и Android необходимо добавить библиотеку [azure-identity,](/java/api/overview/azure/identity-readme) чтобы получить доступ к различным типам учетных данных. Разработчикам .NET необходимо добавить пакет [Azure.Identity,](/dotnet/api/azure.identity) чтобы получить доступ к различным типам учетных данных.

## <a name="authorization-code-provider"></a>Поставщик кода авторизации

Поток кода авторизации позволяет родным и веб-приложениям безопасно получать маркеры от имени пользователя. Дополнительные дополнительные платформа удостоверений Майкрософт и поток кода авторизации [OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-auth-code-flow)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// For authorization code flow, the user signs into the Microsoft
// identity platform, and the browser is redirected back to your app
// with an authorization code in the query parameters
var authorizationCode = "AUTH_CODE_FROM_REDIRECT";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.authorizationcodecredential
var authCodeCredential = new AuthorizationCodeCredential(
    tenantId, clientId, clientSecret, authorizationCode, options);

var graphClient = new GraphServiceClient(authCodeCredential, scopes);
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

Еще не доступно. Пожалуйста, поддержите или откройте запрос на [Graph Microsoft,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступна. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

---

## <a name="client-credentials-provider"></a>Поставщик учетных данных клиента

Поток клиентских учетных данных позволяет приложениям-службам работать без взаимодействия с пользователем. Доступ основан на удостоверении приложения. Дополнительные сведения см. платформа удостоверений Майкрософт и поток учетных данных [клиентов OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

# <a name="c"></a>[C#](#tab/CS)

### <a name="using-a-client-secret"></a>Использование секрета клиента

```csharp
var scopes = new[] { "User.Read.All" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.clientsecretcredential
var clientSecretCredential = new ClientSecretCredential(
    tenantId, clientId, clientSecret, options);

var graphClient = new GraphServiceClient(clientSecretCredential, scopes);
```

### <a name="using-a-client-certificate"></a>С использованием сертификата клиента

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientCertificate = new X509Certificate2("MyCertificate.pfx");

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// https://docs.microsoft.com/dotnet/api/azure.identity.clientcertificatecredential
var clientCertCredential = new ClientCertificateCredential(
    tenantId, clientId, clientCertificate, options);

var graphClient = new GraphServiceClient(clientCertCredential, scopes);
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

Пока недоступна. Пожалуйста, поддержите или откройте запрос на [Graph Microsoft,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступна. Пожалуйста, поддержите или откройте запрос на [Graph Microsoft,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

---

## <a name="on-behalf-of-provider"></a>От имени поставщика

Поток от имени применим, когда ваше приложение вызывает API службы и веб-службы, который по очереди вызывает API microsoft Graph. Дополнительные дополнительные [платформа удостоверений Майкрософт и поток OAuth 2.0 On-Behalf-Of](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

Пакет не поддерживает поток от имени по версии `Azure.Identity` 1.4.0. Вместо этого создайте настраиваемый поставщик проверки подлинности с помощью MSAL.

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// This is the incoming token to exchange using on-behalf-of flow
var oboToken = "JWT_TOKEN_TO_EXCHANGE";

var cca = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantId)
    .WithClientSecret(clientSecret)
    .Build();

// DelegateAuthenticationProvider is a simple auth provider implementation
// that allows you to define an async function to retrieve a token
// Alternatively, you can create a class that implements IAuthenticationProvider
// for more complex scenarios
var authProvider = new DelegateAuthenticationProvider(async (request) => {
    // Use Microsoft.Identity.Client to retrieve token
    var assertion = new UserAssertion(oboToken);
    var result = await cca.AcquireTokenOnBehalfOf(scopes, assertion).ExecuteAsync();

    request.Headers.Authorization =
        new System.Net.Http.Headers.AuthenticationHeaderValue("Bearer", result.AccessToken);
});

var graphClient = new GraphServiceClient(authProvider);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Код авторизации, учетные данные клиентов и потоки OAuth от имени требуют, чтобы вы реализовали настраиваемого поставщика проверки подлинности в это время. Дополнительные сведения читайте в [публикации "Использование](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) поставщика настраиваемой проверки подлинности".

# <a name="java"></a>[Java](#tab/Java)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

# <a name="android"></a>[Android](#tab/Android)

Неприменимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Неприменимо.

# <a name="php"></a>[PHP](#tab/PHP)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

---

## <a name="implicit-provider"></a>Неявный поставщик

Неявный поток грантов используется в браузерных приложениях. Дополнительные сведения см. [в платформа удостоверений Майкрософт и неявном потоке грантов.](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)

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

## <a name="device-code-provider"></a>Поставщик кода устройств

Поток кода устройства позволяет войти на устройства с помощью другого устройства. Подробные сведения [см. платформа удостоверений Майкрософт и поток кода устройства OAuth 2.0.](/azure/active-directory/develop/v2-oauth2-device-code)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

// Callback function that receives the user prompt
// Prompt contains the generated device code that use must
// enter during the auth process in the browser
Func<DeviceCodeInfo, CancellationToken, Task> callback = (code, cancellation) => {
    Console.WriteLine(code.Message);
    return Task.FromResult(0);
};

// https://docs.microsoft.com/dotnet/api/azure.identity.devicecodecredential
var deviceCodeCredential = new DeviceCodeCredential(
    callback, tenantId, clientId, options);

var graphClient = new GraphServiceClient(deviceCodeCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

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

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

---

## <a name="integrated-windows-provider"></a>Интегрированный Windows поставщик

Интегрированный поток Windows обеспечивает возможность Windows компьютеров для бесшумного приобретения маркера доступа при присоединении к домену. Подробные сведения см. в [Windows комплексной проверки подлинности.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)

# <a name="c"></a>[C#](#tab/CS)

В `Azure.Identity` данный момент пакет не поддерживает Windows проверку подлинности. Вместо этого создайте настраиваемый поставщик проверки подлинности с помощью MSAL.

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var pca = PublicClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantId)
    .Build();

// DelegateAuthenticationProvider is a simple auth provider implementation
// that allows you to define an async function to retrieve a token
// Alternatively, you can create a class that implements IAuthenticationProvider
// for more complex scenarios
var authProvider = new DelegateAuthenticationProvider(async (request) => {
    // Use Microsoft.Identity.Client to retrieve token
    var result = await pca.AcquireTokenByIntegratedWindowsAuth(scopes).ExecuteAsync();

    request.Headers.Authorization =
        new System.Net.Http.Headers.AuthenticationHeaderValue("Bearer", result.AccessToken);
});

var graphClient = new GraphServiceClient(authProvider);
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

## <a name="interactive-provider"></a>Интерактивный поставщик

Интерактивный поток используется мобильными приложениями (Xamarin и UWP) и настольными приложениями для вызова microsoft Graph от имени пользователя. Подробные сведения см. [в материале Эквайринг маркеров в интерактивном режиме.](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var options = new InteractiveBrowserCredentialOptions
{
    TenantId = tenantId,
    ClientId = clientId,
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud,
    // MUST be http://localhost or http://localhost:PORT
    // See https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/System-Browser-on-.Net-Core
    RedirectUri = new Uri("http://localhost"),
};

// https://docs.microsoft.com/dotnet/api/azure.identity.interactivebrowsercredential
var interactiveCredential = new InteractiveBrowserCredential(options);

var graphClient = new GraphServiceClient(interactiveCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

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

## <a name="usernamepassword-provider"></a>Поставщик имен пользователей и паролей

Поставщик имен пользователей и паролей позволяет приложению войти в пользователя с помощью имени пользователя и пароля. Используйте этот поток только в том случае, если вы не можете использовать другие потоки OAuth. Дополнительные сведения см. в платформа удостоверений Майкрософт и учетных данных владельца пароля ресурса [OAuth 2.0](/azure/active-directory/develop/v2-oauth-ropc)

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

var userName = "adelev@contoso.com";
var password = "P@ssword1!";

var userNamePasswordCredential = new UsernamePasswordCredential(
    userName, password, tenantId, clientId, options);

var graphClient = new GraphServiceClient(userNamePasswordCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

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

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Еще не доступно. Пожалуйста, проголосуйте за или откройте запрос Graph [майкрософт,](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph) если это важно для вас.

---

## <a name="next-steps"></a>Дальнейшие действия

* Примеры кода, которые показывают, как использовать платформа удостоверений Майкрософт для защиты различных типов приложений, см. в платформа удостоверений Майкрософт примерах кода [(конечная точка v2.0).](/azure/active-directory/develop/sample-v2-code)
* Поставщикам проверки подлинности требуется идентификация клиента. Вы захотите [зарегистрировать свое приложение после](https://portal.azure.com/) того, как настроите поставщика проверки подлинности.
* Дайте нам знать, если необходимый поток OAuth в настоящее время не поддерживается путем голосования или открытия запроса функций [Microsoft Graph.](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)
