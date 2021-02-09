---
title: Использование SDKs Microsoft Graph с бета-версией API
description: Описывается использование SDKs Microsoft Graph с бета-версией API.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 919751d2e57361bdd35380d0891ac8b4264b7aa8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161385"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Использование SDKs Microsoft Graph с бета-версией API

Многие SDKs Microsoft Graph используют конечную точку Microsoft Graph [1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) по умолчанию. SDKs можно использовать с конечной точкой [бета-версии](/graph/api/overview?view=graph-rest-beta&preserve-view=true) для непроизводивых приложений. Способ доступа к конечной точке бета-версии зависит от используемого SDK.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[C#](#tab/CS)

Чтобы вызвать бета-версию API, необходимо установить пакет [Microsoft.Graph.Beta.](https://www.nuget.org/packages/Microsoft.Graph.Beta) Использование такое же, как и у `Microsoft.Graph` пакета.

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

Клиентская [библиотека JavaScript microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) может вызывать бета-версию API одним из двух способов.

- Версию можно установить при `MicrosoftGraph.Client` ее создании. Все запросы, сделанные клиентом, будут перенаходить к указанной версии.

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- Версию можно установить по конкретному запросу с помощью `version` функции `GraphRequest` объекта.

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

Чтобы вызвать бета-версию API, необходимо установить [Java SDK для Бета-версии Microsoft Graph.](https://github.com/microsoftgraph/msgraph-beta-sdk-java) Использование не является бета-версией SDK.

```Java
IGraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Для [SDK Microsoft Graph для ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) требуется создать строку URL-адреса для API, который вы хотите вызвать. Он предоставляет `MSGraphBaseURL` константы для конечной точки v1.0. Чтобы использовать бета-версию, просто замените ее на `https://graph.microsoft.com/beta` .

Однако модели в [SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) моделей Microsoft Graph создаются из объектов в API версии 1.0, поэтому они могут не работать с бета-объектами.

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

Microsoft [Graph SDK для PHP](https://github.com/microsoftgraph/msgraph-sdk-php) поддерживает конечную точку и модели бета-версии. С помощью этого метода можно настроить конечную точку `setApiVersion` бета-версии. Вам потребуется улиться в неоднозначности моделей версии 1.0 и бета-версии, предоставив псевдоним.

```php
use Microsoft\Graph\Graph;
use Beta\Microsoft\Graph\Model as BetaModel;

class UseBeta
{
    public function run()
    {
        $accessToken = 'xxx';

        $graph = new Graph();
        $graph->setAccessToken($accessToken);

        $user = $graph->setApiVersion("beta")
                      ->createRequest("GET", "/me")
                      ->setReturnType(BetaModel\User::class)
                      ->execute();

        echo "Hello, I am $user->getGivenName() ";
    }
}
```

---
