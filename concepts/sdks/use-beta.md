---
title: Использование пакетов SDK Microsoft Graph с бета-версией API
description: Описание использования пакетов SDK Microsoft Graph с бета-версией API.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 6a0444cdb30b2e07c4d93f683aaef2f5283c3846
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288968"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Использование пакетов SDK Microsoft Graph с бета-версией API

По умолчанию пакет SDK Microsoft Graph использует конечную точку Microsoft Graph [версии 1.0](/graph/api/overview?view=graph-rest-1.0) . Пакеты SDK можно использовать с конечной точкой [бета-версии](/graph/api/overview?view=graph-rest-beta) для непроизводственных приложений. Метод доступа к конечной точке бета-версии зависит от того, какой пакет SDK используется.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[C#](#tab/CS)

Для вызова бета-версии API необходимо установить пакет [Microsoft. Graph. Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) . Использование совпадает с `Microsoft.Graph` пакетом.

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

## <a name="typescript"></a>[TypeScript](#tab/typeScript)

[Клиентская библиотека JavaScript Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) может вызывать бета-версию API одним из двух способов.

- Вы можете задать версию `MicrosoftGraph.Client` при создании. Все запросы, выполняемые клиентом, переходят на указанную версию.

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- Вы можете задать версию в определенном запросе, используя `version` функцию для `GraphRequest` объекта.

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

Для вызова бета-версии API необходимо установить [пакет SDK Java для бета-версии Microsoft Graph](https://github.com/microsoftgraph/msgraph-beta-sdk-java). Использование совпадает с небета-версией пакета SDK.

```Java
IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Для работы с [пакетом SDK Microsoft Graph для обжк](https://github.com/microsoftgraph/msgraph-sdk-objc) необходимо создать строку URL-адреса для API, который требуется вызвать. Он предоставляет константу `MSGraphBaseURL` для конечной точки v 1.0. Чтобы использовать бета-версию, просто замените его на `https://graph.microsoft.com/beta` .

Однако модели в [пакете SDK моделей Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) создаются на основе объектов в API v 1.0, поэтому они могут не работать с объектами бета-версии.

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

---
