---
title: Настройка клиента службы SDK Microsoft Graph
description: В этом разделе приведены инструкции по изменению поведения клиента службы SDK Microsoft Graph по умолчанию.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: dd8fdca9d093c8164dd486fb185d462b9de0ff0d
ms.sourcegitcommit: 6eadb95e21b2e7eb5d6b081b91999cb91070f397
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2020
ms.locfileid: "48299279"
---
# <a name="customize-the-microsoft-graph-sdk-service-client"></a><span data-ttu-id="e73f0-103">Настройка клиента службы SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e73f0-103">Customize the Microsoft Graph SDK service client</span></span>

<span data-ttu-id="e73f0-104">Клиент SDK Microsoft Graph настраивает набор по умолчанию по промежуточного слоя, который позволяет пакету SDK общаться с конечными точками Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e73f0-104">The Microsoft Graph SDK client configures a default set of middleware that allows the SDK to communicate with the Microsoft Graph endpoints.</span></span> <span data-ttu-id="e73f0-105">Этот набор по умолчанию является настраиваемым, позволяя изменить поведение клиента.</span><span class="sxs-lookup"><span data-stu-id="e73f0-105">This default set is customizable, allowing you to change the behavior of the client.</span></span> <span data-ttu-id="e73f0-106">Например, можно вставить настраиваемое ведение журнала или добавить обработчик тестов для имитации определенных сценариев.</span><span class="sxs-lookup"><span data-stu-id="e73f0-106">For example, you can insert customized logging, or add a test handler to simulate specific scenarios.</span></span> <span data-ttu-id="e73f0-107">Вы можете добавлять и удалять компоненты промежуточного слоя.</span><span class="sxs-lookup"><span data-stu-id="e73f0-107">You can add and remove middleware components.</span></span> <span data-ttu-id="e73f0-108">Важно отметить, что порядок выполнения компонентов по промежуточного слоя важен.</span><span class="sxs-lookup"><span data-stu-id="e73f0-108">It is important to note that the order in which middleware components run is significant.</span></span>

## <a name="c"></a>[<span data-ttu-id="e73f0-109">C#</span><span class="sxs-lookup"><span data-stu-id="e73f0-109">C#</span></span>](#tab/csharp)

```csharp
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

## <a name="typescript"></a>[<span data-ttu-id="e73f0-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="e73f0-110">TypeScript</span></span>](#tab/typeScript)

```typescript
// Create a custom auth provider
let authProvider = new SimpleAuthProvider(accessToken);
// Create an authentication handler that uses custom auth provider
let authHandler = new MicrosoftGraph.AuthenticationHandler(authProvider);

// Create a custom logging handler
let loggingHandler = new CustomLoggingHandler();

// Create a standard HTTP message handler
let httpHandler = new MicrosoftGraph.HTTPMessageHandler();

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

let response: PageCollection = await client
  .api('/me/messages?$top=10&$select=sender,subject')
  .get();
```

### <a name="simpleauthproviderts"></a><span data-ttu-id="e73f0-111">Симплеауспровидер. TS</span><span class="sxs-lookup"><span data-stu-id="e73f0-111">SimpleAuthProvider.ts</span></span>

```typescript
import { AuthenticationProvider } from "@microsoft/microsoft-graph-client";

export default class SimpleAuthProvider implements AuthenticationProvider {
  private accessToken: string;

  constructor(accessToken: string) {
    this.accessToken = accessToken;
  }

  getAccessToken = async (): Promise<string> => {
    return this.accessToken;
  }
}
```

### <a name="customlogginghandlerts"></a><span data-ttu-id="e73f0-112">Кустомлоггингхандлер. TS</span><span class="sxs-lookup"><span data-stu-id="e73f0-112">CustomLoggingHandler.ts</span></span>

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

## <a name="java"></a>[<span data-ttu-id="e73f0-113">Java</span><span class="sxs-lookup"><span data-stu-id="e73f0-113">Java</span></span>](#tab/java)

```java
// you can configure any OkHttpClient option and add interceptors
// Note: com.microsoft.graph:microsoft-graph:2.3 or above is required
// for a complete description of available configuration options https://square.github.io/okhttp/4.x/okhttp/okhttp3/-ok-http-client/-builder/
final OkHttpClient httpClient = HttpClients.createDefault(coreAuthenticationProvider)
                                .newBuilder()
                                .followSslRedirects(false) // sample configuration to apply to client
                                .build();

final IHttpProvider httpProvider = DefaultClientConfig
                          .createWithAuthenticationProvider(authenticationProvider)
                          .getHttpProvider(httpClient);

final IGraphServiceClient graphServiceClient = GraphServiceClient
                .builder()
                .authenticationProvider(authenticationProvider)
                .httpProvider(httpProvider)
                .buildClient();
```

---
