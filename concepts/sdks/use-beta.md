---
title: Используйте SDKs Microsoft Graph с бета-API
description: Описывает использование SDKs Microsoft Graph с бета-версией API.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 4d984cd9c236b1fb2785cd998dd69fb998cd137e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941360"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Используйте SDKs Microsoft Graph с бета-API

Многие SDKs Microsoft Graph используют конечную точку [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph по умолчанию. SDKs можно использовать с конечной точкой [бета-версии](/graph/api/overview?view=graph-rest-beta&preserve-view=true) для непроизводимых приложений. Метод доступа к конечной точке бета-версии зависит от того, какой SDK вы используете.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[C#](#tab/CS)

Чтобы вызвать бета-API, необходимо установить [пакет Microsoft.Graph.Beta.](https://www.nuget.org/packages/Microsoft.Graph.Beta) Использование такое же, как и `Microsoft.Graph` в пакете.

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

Клиентская [библиотека JavaScript Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) может вызывать бета-API одним из двух способов.

- Вы можете настроить версию на момент `MicrosoftGraph.Client` ее создания. Все запросы клиента будут переходить к указанной версии.

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- Версию можно настроить по определенному запросу с помощью `version` функции `GraphRequest` объекта.

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

Чтобы вызвать бета-API, необходимо установить [SDK Microsoft Graph Beta Java.](https://github.com/microsoftgraph/msgraph-beta-sdk-java) Использование такое же, как и не бета-версия SDK.

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Для [SDK Microsoft Graph для ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) требуется создать строку URL-адреса в API, который вы хотите вызвать. Он обеспечивает `MSGraphBaseURL` констант для конечной точки v1.0. Чтобы использовать бета-версию, вы просто замените это `https://graph.microsoft.com/beta` на .

Однако модели [SDK моделей Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) создаются из объектов API v1.0, поэтому они могут не работать с бета-объектами.

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

[SDK Microsoft Graph для PHP](https://github.com/microsoftgraph/msgraph-sdk-php) поддерживает бета-конечную точку и модели. Методом установлена конечная точка `setApiVersion` бета-версии. Вам потребуется отмыть модели v1.0 и бета-версии, предоставив псевдоним.

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
