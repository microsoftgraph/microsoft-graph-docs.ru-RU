---
title: Настройка клиента службы microsoft Graph SDK
description: Содержит инструкции по изменению поведения клиента службы microsoft Graph SDK по умолчанию.
ms.localizationpriority: medium
author: DarrelMiller
ms.openlocfilehash: 292548544abba7cd56bd2154cec576e0bb3fba0a
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733166"
---
# <a name="customize-the-microsoft-graph-sdk-service-client"></a>Настройка клиента службы microsoft Graph SDK

Клиент microsoft Graph SDK настраивает набор ПО промежуточного слоя по умолчанию, который позволяет пакету SDK взаимодействовать с конечными точками Graph Майкрософт. Этот набор по умолчанию настраивается, что позволяет изменить поведение клиента. Например, можно вставить настроенное ведение журнала или добавить обработчик тестов для имитации определенных сценариев. Вы можете добавлять и удалять компоненты ПО промежуточного слоя. Важно отметить, что порядок выполнения компонентов ПО промежуточного слоя очень важен.

## <a name="c"></a>[C#](#tab/csharp)

```csharp
// using Azure.Identity;
// https://docs.microsoft.com/dotnet/api/azure.identity.interactivebrowsercredential
var interactiveCredential = new InteractiveBrowserCredential(...);

var authProvider = new TokenCredentialAuthProvider(
    interactiveCredential, scopes);

var handlers = GraphClientFactory.CreateDefaultHandlers(authProvider);

// Remove a default handler
var compressionHandler =
    handlers.Where(h => h is CompressionHandler).FirstOrDefault();
handlers.Remove(compressionHandler);

// Add a new one
// ChaosHandler simulates random server failures
handlers.Add(new ChaosHandler());

var httpClient = GraphClientFactory.Create(handlers);

var customGraphClient = new GraphServiceClient(httpClient);

var messages = await customGraphClient.Me.Messages.Request()
    .Top(100)
    .Select(m => m.Subject)
    .GetAsync();
```

## <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
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

// Create an authentication handler that uses custom auth provider
const authHandler = new MicrosoftGraph.AuthenticationHandler(authProvider);

// Create a custom logging handler
const loggingHandler = new CustomLoggingHandler();

// Create a standard HTTP message handler
const httpHandler = new MicrosoftGraph.HTTPMessageHandler();

// Use setNext to chain handlers together
// auth -> logging -> http
authHandler.setNext(loggingHandler);
loggingHandler.setNext(httpHandler);

// Pass the first middleware in the chain in the middleWare property
const client = MicrosoftGraph.Client.initWithMiddleware({
  defaultVersion: 'v1.0',
  debugLogging: true,
  middleware: authHandler,
});

const response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();
```

### <a name="customlogginghandlerts"></a>CustomLoggingHandler.ts

```typescript
import { Context, Middleware } from "@microsoft/microsoft-graph-client";

export default class CustomLoggingHandler implements Middleware {
  private nextMiddleware: any = null;

  execute = async (context: Context): Promise<void> => {
    console.log(`Logging request: ${context.request.toString()}`);
    return await this.nextMiddleware.execute(context);
  }
  setNext = (middleware: Middleware): void => {
    this.nextMiddleware = middleware;
  }
}
```

## <a name="java"></a>[Java](#tab/java)

```java
import com.azure.identity.InteractiveBrowserCredential;
import com.azure.identity.InteractiveBrowserCredentialBuilder;
import com.microsoft.graph.authentication.TokenCredentialAuthProvider;
import com.microsoft.graph.httpcore.HttpClients;

import okhttp3.OkHttpClient;

final List<String> scopes = Arrays.asList("User.Read");

final InteractiveBrowserCredential credential =
    new InteractiveBrowserCredentialBuilder()
        .clientId("clientId")
        .redirectUrl("redirectUrl")
        .build();

final TokenCredentialAuthProvider authProvider =
    new TokenCredentialAuthProvider(scopes, credential);
// you can configure any OkHttpClient option and add interceptors
// Note: com.microsoft.graph:microsoft-graph:3.0 or above is required
// for a complete description of available configuration options https://square.github.io/okhttp/4.x/okhttp/okhttp3/-ok-http-client/-builder/
final OkHttpClient httpClient = HttpClients.createDefault(authProvider)
    .newBuilder()
    .followSslRedirects(false) // sample configuration to apply to client
    .build();

final GraphServiceClient graphServiceClient = GraphServiceClient
    .builder()
    .httpClient(httpClient)
    .buildClient();
```

## <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

```go
import (
    a "github.com/microsoft/kiota-authentication-azure-go"
    khttp "github.com/microsoft/kiota-http-go"
    msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
    core "github.com/microsoftgraph/msgraph-sdk-go-core"
)

// Auth provider
auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(...)

// Get default middleware from SDK
defaultMiddleware := core.GetDefaultMiddlewaresWithOptions(msgraphsdk.GetDefaultClientOptions())

// Get instance of custom middleware
// Implement a custom middleware by implementing the Middleware interface
// https://github.com/microsoft/kiota-http-go/blob/main/middleware.go
allMiddleware := append(defaultMiddleware, mycustom.NewCustomHandler())

// Create an HTTP client with the middleware
httpClient := khttp.GetDefaultClient(allMiddleware...)

// Create the adapter
// Passing nil values causes the adapter to use default implementations
adapter, err :=
    msgraphsdk.NewGraphRequestAdapterWithParseNodeFactoryAndSerializationWriterFactoryAndHttpClient(
        auth, nil, nil, httpClient)

client := msgraphsdk.NewGraphServiceClient(adapter)
```

---

## <a name="configuring-the-http-proxy-for-the-client"></a>Настройка прокси-сервера HTTP для клиента

В некоторых средах клиентские приложения должны использовать прокси-сервер HTTP, прежде чем они могут получить доступ к общедоступному Интернету. В этом разделе показано, как настроить прокси-сервер для пакетов SDK Graph Майкрософт.

<!-- markdownlint-disable MD024 -->
## <a name="c"></a>[C#](#tab/csharp)

```csharp
// URI to proxy
var proxyAddress = "http://localhost:8888";

// Create a new System.Net.Http.HttpClientHandler with the proxy
var handler = new HttpClientHandler
{
    // Create a new System.Net.WebProxy
    // See WebProxy documentation for scenarios requiring
    // authentication to the proxy
    Proxy = new WebProxy(new Uri(proxyAddress))
};

// Create an options object for the credential being used
// For example, here we're using a ClientSecretCredential so
// we create a ClientSecretCredentialOptions object
var options = new ClientSecretCredentialOptions
{
    // Create a new Azure.Core.HttpClientTransport
    Transport = new HttpClientTransport(handler)
};

var credential = new ClientSecretCredential(
    "YOUR_TENANT_ID",
    "YOUR_CLIENT_ID",
    "YOUR_CLIENT_SECRET",
    options
);

var scopes = new[] { "https://graph.microsoft.com/.default" };

// This example works with Microsoft.Graph 4+
var httpClient = GraphClientFactory.Create(new TokenCredentialAuthProvider(credential, scopes), proxy: new WebProxy(new Uri(proxyAddress)));

var graphClient = new GraphServiceClient(httpClient);
```

## <a name="typescript"></a>[TypeScript](#tab/typeScript)

```typescript
// Create a credential from @azure/identity package
const credential = new ClientSecretCredential(
  'YOUR_TENANT_ID',
  'YOUR_CLIENT_ID',
  'YOUR_CLIENT_SECRET',
  {
    proxyOptions: {
      host: 'localhost',
      port: 8888,
      // If proxy requires authentication
      //username: '',
      //password: ''
    },
  }
);

// Create a Graph token credential provider
const tokenAuthProvider = new TokenCredentialAuthenticationProvider(
  credential,
  {
    scopes: [ 'https://graph.microsoft.com/.default' ]
  });

const client = MicrosoftGraph.Client.initWithMiddleware({
  authProvider: tokenAuthProvider,
  // Configure proxy in fetchOptions
  fetchOptions: {
    agent: new HttpsProxyAgent('http://localhost:8888')
  }
});
```

## <a name="java"></a>[Java](#tab/java)

```Java
final int proxyPort = 8080;
final InetSocketAddress proxyInetAddress = new InetSocketAddress("proxy.ip.or.hostname", proxyPort);

// The section below configures the proxy for the Azure Identity client
// and is only needed if you rely on Azure Identity for authentication
final ProxyOptions pOptions = new ProxyOptions(ProxyOptions.Type.HTTP, proxyInetAddress);
pOptions.setCredentials("username", "password");
final HttpClientOptions clientOptions = new HttpClientOptions();
clientOptions.setProxyOptions(pOptions);
final HttpClient azHttpClient = HttpClient.createDefault(clientOptions);

// Or any other credential the application is using
final ClientSecretCredential clientSecretCredential =
    new ClientSecretCredentialBuilder()
        .clientId(CLIENT_ID)
        .clientSecret(CLIENT_SECRET)
        .tenantId(TENANT_GUID)
        // don't forget that addition to use the configured client
        .httpClient(azHttpClient)
        .build();
final TokenCredentialAuthProvider authenticationProvider =
    new TokenCredentialAuthProvider(Arrays.asList(SCOPES), clientSecretCredential);

// The section below configures the proxy for the Microsoft Graph SDK client
final Proxy proxy = new Proxy(Proxy.Type.HTTP, proxyInetAddress);

// This block is only needed if the proxy requires authentication
final Authenticator proxyAuthenticator = new Authenticator() {
  @Override
  public Request authenticate(Route route, Response response) throws IOException {
    String credential = Credentials.basic("username", "password");
    return response.request().newBuilder()
        .header("Proxy-Authorization", credential)
        .build();
  }
};

final OkHttpClient graphHttpClient =
    HttpClients.createDefault(authenticationProvider)
        .newBuilder()
        .proxy(proxy)
        .proxyAuthenticator(proxyAuthenticator)
        .build();

final GraphServiceClient graphServiceClient =
    GraphServiceClient
        .builder()
        .httpClient(graphHttpClient)
        .buildClient();

```

> [!NOTE]
> Дополнительные сведения о конфигурации прокси-сервера удостоверений Azure см. в [разделе ProxyOptions](/java/api/com.azure.core.http.proxyoptions.proxyoptions).

## <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Пакет Microsoft Graph SDK для Go в настоящее время не поддерживает прокси-сервер HTTP. [Дополнительные сведения см. GitHub этой](https://github.com/microsoftgraph/msgraph-sdk-go-core/issues/15) проблеме.

---
