---
title: Выбор поставщика проверки Graph Майкрософт
description: Узнайте, как выбрать поставщики проверки подлинности для конкретного сценария для приложения.
ms.localizationpriority: medium
author: MichaelMainer
ms.openlocfilehash: 040a42ae20ee48d5af92dd4460b2e26b059ffea7
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733246"
---
<!-- markdownlint-disable MD001 MD024 MD025 -->

# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>Выбор поставщика проверки подлинности Microsoft Graph на основе сценария

Поставщики проверки подлинности реализуют код, необходимый для получения маркера с помощью библиотеки проверки подлинности Майкрософт (MSAL); обрабатывать ряд потенциальных ошибок в таких случаях, как добавочное согласие, просроченные пароли и условный доступ; и задайте заголовок авторизации HTTP-запроса. В следующей таблице перечислены поставщики, соответствующие сценариям для различных [типов приложений](/azure/active-directory/develop/v2-app-types).

| Сценарий                                                                                               | Flow/Grant         | Аудитория               | Поставщик |
|--------------------------------------------------------------------------------------------------------|--------------------|------------------------|-----|
| [Одностраничного приложения](/azure/active-directory/develop/scenario-spa-acquire-token)                          | Код авторизации с PKCE | Делегированный потребитель или организация | [Поставщик кода авторизации](#authorization-code-provider) |
| [Веб-приложение, вызывающее веб-API](/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | Authorization Code | Делегированный потребитель или организация | [Поставщик кода авторизации](#authorization-code-provider) |
|                                                                                                        | Учетные данные клиента | Только приложение               | [Поставщик учетных данных клиента](#client-credentials-provider) |
| [Веб-API, который вызывает веб-API](/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) |                    |                        |     |
|                                                                                                        | От имени       | Делегированный потребитель или организация | [От имени поставщика](#on-behalf-of-provider) |
|                                                                                                        | Учетные данные клиента | Только приложение               | [Поставщик учетных данных клиента](#client-credentials-provider) |
| [Настольное приложение, вызывающее веб-API](/azure/active-directory/develop/scenario-desktop-acquire-token)      |                    |                        |     |
|                                                                                                        | Интерактивны        | Делегированный потребитель или организация | [Интерактивный поставщик](#interactive-provider) |
|                                                                                                        | Интегрированные Windows | Делегированная организация          | [Интегрированный поставщик Windows](#integrated-windows-provider) |
|                                                                                                        | Владелец ресурса     | Делегированная организация          | [Поставщик имени пользователя и пароля](#usernamepassword-provider) |
|                                                                                                        | Код устройства        | Делегированная организация          | [Поставщик кода устройства](#device-code-provider) |
| [Управляющее приложение](/azure/active-directory/develop/scenario-daemon-acquire-token)                            |                    |                        |     |
|                                                                                                        | Учетные данные клиента | Только приложение               | [Поставщик учетных данных клиента](#client-credentials-provider) |
| [Мобильное приложение, вызывающее веб-API](/azure/active-directory/develop/scenario-mobile-acquire-token)        |                    |                        |     |
|                                                                                                        | Интерактивны        | Делегированный потребитель или организация | [Интерактивный поставщик](#interactive-provider) |

> [!NOTE]
> Следующие фрагменты кода были написаны с использованием последних версий соответствующих пакетов SDK. Если с этими фрагментами кода возникают ошибки компилятора, убедитесь, что у вас есть последние версии. Используемые поставщики проверки подлинности предоставляются следующими библиотеками удостоверений Azure:
>
> - Разработчикам .NET необходимо добавить [пакет Azure.Identity](/dotnet/api/azure.identity) .
> - Разработчикам JavaScript необходимо добавить библиотеку [@azure/identity](/javascript/api/@azure/identity) .
> - Разработчикам Java и Android необходимо добавить [библиотеку azure-identity](/java/api/overview/azure/identity-readme) .

## <a name="authorization-code-provider"></a>Поставщик кода авторизации

Поток кода авторизации позволяет собственным и веб-приложениям безопасно получать маркеры от имени пользователя. Дополнительные сведения см[. в платформа удостоверений Майкрософт кода авторизации OAuth 2.0](/azure/active-directory/develop/v2-oauth2-auth-code-flow).

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

// using Azure.Identity;
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

### <a name="using-azuremsal-browser-for--browser-applications"></a>Использование @azure/msal-browser для браузерных приложений

```javascript

const {
    PublicClientApplication,
    InteractionType,
    AccountInfo
} = require("@azure/msal-browser");

const {
    AuthCodeMSALBrowserAuthenticationProvider,
    AuthCodeMSALBrowserAuthenticationProviderOptions
} = require("@microsoft/microsoft-graph-client/authProviders/authCodeMsalBrowser");

const options: AuthCodeMSALBrowserAuthenticationProviderOptions: {
    account: account, // the AccountInfo instance to acquire the token for.
    interactionType: InteractionType.PopUp, // msal-browser InteractionType
    scopes: ["user.read", "mail.send"] // example of the scopes to be passed
}

// Pass the PublicClientApplication instance from step 2 to create AuthCodeMSALBrowserAuthenticationProvider instance
const authProvider: new AuthCodeMSALBrowserAuthenticationProvider(publicClientApplication, options),
```

### <a name="using-azureidentity-for-server-side-applications"></a>Использование @azure/identity для серверных приложений

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    AuthorizationCodeCredential
} = require("@azure/identity");

const credential = new AuthorizationCodeCredential(
    "<YOUR_TENANT_ID>",
    "<YOUR_CLIENT_ID>",
    "<AUTH_CODE_FROM_QUERY_PARAMETERS>",
    "<REDIRECT_URL>"
);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

```

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

Не применимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Не применимо.

# <a name="php"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, обратитесь в службу поддержки или [Graph майкрософт](https://aka.ms/graphrequests).

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewAuthorizationCodeCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "AUTH_CODE",
    "REDIRECT_URL",
    &azidentity.AuthorizationCodeCredentialOptions {
        ClientSecret: "CLIENT_SECRET",
    },
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="client-credentials-provider"></a>Поставщик учетных данных клиента

Поток учетных данных клиента позволяет приложениям-службам выполняться без взаимодействия с пользователем. Доступ основан на удостоверении приложения. Дополнительные сведения см. в платформа удостоверений Майкрософт и потоке учетных данных клиента [OAuth 2.0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).

# <a name="c"></a>[C#](#tab/CS)

### <a name="using-a-client-secret"></a>Использование секрета клиента

```csharp
// The client credentials flow requires that you request the
// /.default scope, and preconfigure your permissions on the
// app registration in Azure. An administrator must grant consent
// to those permissions beforehand.
var scopes = new[] { "https://graph.microsoft.com/.default" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// using Azure.Identity;
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

// using Azure.Identity;
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

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    ClientSecretCredential
} = require("@azure/identity");

const credential = new ClientSecretCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider
    // Use the authProvider object to create the class.
});
```

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

Не применимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Не применимо.

# <a name="php"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, обратитесь в службу поддержки или [Graph майкрософт](https://aka.ms/graphrequests).

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, обратитесь в службу поддержки или [Graph майкрософт](https://aka.ms/graphrequests).

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewClientSecretCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "CLIENT_SECRET",
    nil,
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="on-behalf-of-provider"></a>От имени поставщика

Поток "от имени" применяется, когда приложение вызывает службу или веб-API, который, в свою API Graph. Дополнительные сведения см[. в платформа удостоверений Майкрософт и потоке On-Behalf-Of oAuth 2.0](/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)

# <a name="c"></a>[C#](#tab/CS)

Пакет `Azure.Identity` не поддерживает поток on-behalf-of в версии 1.4.0. Вместо этого создайте пользовательский поставщик проверки подлинности с помощью MSAL.

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Values from app registration
var clientId = "YOUR_CLIENT_ID";
var clientSecret = "YOUR_CLIENT_SECRET";

// using Azure.Identity;
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

Для потоков OAuth от имени в данный момент необходимо реализовать настраиваемый поставщик проверки подлинности. [Дополнительные сведения см](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md). с помощью пользовательского поставщика проверки подлинности.

# <a name="java"></a>[Java](#tab/Java)

```java
final OnBehalfOfCredential onBehalfOfCredential = new OnBehalfOfCredentialBuilder()
        .clientId(clientID)
        .pfxCertificate(pfxCertificatePath) // or .pemCertificate(certificatePath) or .clientSecret("ClientSecret")
        .clientCertificatePassword(pfxCertificatePassword) // remove if using pemCertificate or clientSecret
        .tokenCachePersistenceOptions(tokenCachePersistenceOptions) //Optional: enables the persistent token cache which is disabled by default
        .userAssertion(userAssertion)
        .build();

final TokenCredentialAuthProvider tokenCredentialAuthProvider = new TokenCredentialAuthProvider(scopes, onBehalfOfCredential);

final GraphServiceClient graphClient = GraphServiceClient
        .builder()
        .authenticationProvider(tokenCredentialAuthProvider)
        .buildClient();

final User me = graphClient.me().buildRequest().get();
```

# <a name="android"></a>[Android](#tab/Android)

Не применимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Не применимо.

# <a name="php"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

---

## <a name="implicit-provider"></a>Неявный поставщик

Поток неявной проверки подлинности не рекомендуется из-за его [недостатков](https://datatracker.ietf.org/doc/html/draft-ietf-oauth-browser-based-apps-04#section-9.8.6). Общедоступные клиенты, такие как собственные приложения и приложения JavaScript, теперь должны использовать поток кода авторизации с расширением PKCE. [Справочные материалы](https://oauth.net/2/grant-types/implicit/).

## <a name="device-code-provider"></a>Поставщик кода устройства

Поток кода устройства позволяет выполнять вход на устройства с помощью другого устройства. Дополнительные сведения см[. платформа удостоверений Майкрософт и потоке кода устройства OAuth 2.0](/azure/active-directory/develop/v2-oauth2-device-code).

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
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

```javascript
const {
    Client
} = require("@microsoft/microsoft-graph-client");
const {
    TokenCredentialAuthenticationProvider
} = require("@microsoft/microsoft-graph-client/authProviders/azureTokenCredentials");
const {
    DeviceCodeCredential
} = require("@azure/identity");

const credential = new DeviceCodeCredential(tenantId, clientId, clientSecret);
const authProvider = new TokenCredentialAuthenticationProvider(credential, {
    scopes: [scopes]
});

const client = Client.initWithMiddleware({
    debugLogging: true,
    authProvider
    // Use the authProvider object to create the class.
});
```

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

Не применимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Не применимо.

# <a name="php"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewDeviceCodeCredential(&azidentity.DeviceCodeCredentialOptions{
    ClientID: "CLIENT_ID",
    UserPrompt: func(ctx context.Context, message azidentity.DeviceCodeMessage) error {
        fmt.Println(message.Message)
        return nil
    },
})

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="integrated-windows-provider"></a>Интегрированный поставщик Windows

Интегрированный поток Windows позволяет Windows автоматически получать маркер доступа при присоединении к домену. Дополнительные сведения см. в [разделе проверка подлинности Windows](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).

# <a name="c"></a>[C#](#tab/CS)

В `Azure.Identity` настоящее время пакет не поддерживает Windows встроенной проверки подлинности. Вместо этого создайте пользовательский поставщик проверки подлинности с помощью MSAL.

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

Не применимо.

# <a name="java"></a>[Java](#tab/Java)

Не применимо.

# <a name="android"></a>[Android](#tab/Android)

Не применимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Не применимо.

# <a name="php"></a>[PHP](#tab/PHP)

Не применимо.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Не применимо.

# <a name="go"></a>[Go](#tab/Go)

Не применимо.

---

## <a name="interactive-provider"></a>Интерактивный поставщик

Интерактивный поток используется мобильными приложениями (Xamarin и UWP) и классическими приложениями для вызова Microsoft Graph от имени пользователя. Дополнительные сведения см [. в интерактивном разделе "Получение маркеров"](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
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

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

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

```objectivec
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID"
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication
 andOptions:authProviderOptions];
```

# <a name="php"></a>[PHP](#tab/PHP)

Не применимо.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Не применимо.

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewInteractiveBrowserCredential(&azidentity.InteractiveBrowserCredentialOptions {
    TenantID: "TENANT_ID",
    ClientID: "CLIENT_ID",
    RedirectURL: "REDIRECT_URL",
})

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="usernamepassword-provider"></a>Поставщик имени пользователя и пароля

Поставщик имени пользователя и пароля позволяет приложению входить в систему с помощью имени пользователя и пароля. Используйте этот поток только в том случае, если вы не можете использовать другие потоки OAuth. Дополнительные сведения см[. в платформа удостоверений Майкрософт и учетных данных пароля владельца ресурса OAuth 2.0](/azure/active-directory/develop/v2-oauth-ropc).

# <a name="c"></a>[C#](#tab/CS)

```csharp
var scopes = new[] { "User.Read" };

// Multi-tenant apps can use "common",
// single-tenant apps must use the tenant ID from the Azure portal
var tenantId = "common";

// Value from app registration
var clientId = "YOUR_CLIENT_ID";

// using Azure.Identity;
var options = new TokenCredentialOptions
{
    AuthorityHost = AzureAuthorityHosts.AzurePublicCloud
};

var userName = "adelev@contoso.com";
var password = "P@ssword1!";

// https://docs.microsoft.com/dotnet/api/azure.identity.usernamepasswordcredential
var userNamePasswordCredential = new UsernamePasswordCredential(
    userName, password, tenantId, clientId, options);

var graphClient = new GraphServiceClient(userNamePasswordCredential, scopes);
```

# <a name="javascript"></a>[Javascript](#tab/Javascript)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

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

Не применимо.

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Не применимо.

# <a name="php"></a>[PHP](#tab/PHP)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

# <a name="ruby"></a>[Ruby](#tab/Ruby)

Пока недоступно. Если это важно, проголосуйте за Graph [microsoft](https://aka.ms/graphrequests) Graph функции.

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    "context"

    azidentity "github.com/Azure/azure-sdk-for-go/sdk/azidentity"
    a "github.com/microsoft/kiota-authentication-azure-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
)

cred, err := azidentity.NewUsernamePasswordCredential(
    "TENANT_ID",
    "CLIENT_ID",
    "USER_NAME",
    "PASSWORD",
    nil,
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(cred, []string{"User.Read"})

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)

result, err := client.Me().Get(nil)
```

---

## <a name="next-steps"></a>Дальнейшие действия

- Примеры кода, в которых показано, как использовать платформа удостоверений Майкрософт для защиты различных типов приложений, см. в платформа удостоверений Майкрософт примерах кода [(конечная точка версии 2.0).](/azure/active-directory/develop/sample-v2-code)
- Поставщикам проверки подлинности требуется идентификатор клиента. Вы захотите [зарегистрировать приложение после](https://portal.azure.com/) настройки поставщика проверки подлинности.
- Сообщите нам, если требуемый поток OAuth в настоящее время не поддерживается путем голосования или открытия запроса функции [Microsoft Graph.](https://aka.ms/graphrequests)
