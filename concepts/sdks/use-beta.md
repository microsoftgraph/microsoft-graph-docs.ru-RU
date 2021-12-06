---
title: Используйте SD-Graph Microsoft с бета-API
description: Описывает, как использовать Graph SDKs с бета-версией API.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 8d550c37c998098d07079551a3a4998e85491f9b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992269"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Используйте SD-Graph Microsoft с бета-API

Многие из служб Майкрософт Graph SDKs используют конечную точку [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph по умолчанию. SDKs можно использовать с конечной точкой [бета-версии](/graph/api/overview?view=graph-rest-beta&preserve-view=true) для непроизводимых приложений. Метод доступа к конечной точке бета-версии зависит от того, какой SDK вы используете.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD025 -->
# <a name="c"></a>[C#](#tab/CS)

Чтобы вызвать бета-API, необходимо установить [Microsoft.Graph. Бета-пакет.](https://www.nuget.org/packages/Microsoft.Graph.Beta) Использование такое же, как и `Microsoft.Graph` в пакете.

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

Клиентская [Graph Microsoft может](https://github.com/microsoftgraph/msgraph-sdk-javascript) вызывать API бета-версии одним из двух способов.

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

Чтобы вызвать бета-API, необходимо установить [microsoft Graph Java SDK.](https://github.com/microsoftgraph/msgraph-beta-sdk-java) Использование такое же, как и не бета-версия SDK.

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

В [службе Graph Microsoft для ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) требуется создать строку URL-адреса в API, который вы хотите вызвать. Он обеспечивает `MSGraphBaseURL` констант для конечной точки v1.0. Чтобы использовать бета-версию, вы просто замените это `https://graph.microsoft.com/beta` на .

Однако модели [SDK Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) microsoft models создаются из объектов API v1.0, поэтому они могут не работать с бета-объектами.

```objectivec
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

Корпорация [Майкрософт Graph SDK для PHP](https://github.com/microsoftgraph/msgraph-sdk-php) поддерживает бета-конечную точку и модели. Методом установлена конечная точка `setApiVersion` бета-версии. Вам потребуется отмыть модели v1.0 и бета-версии, предоставив псевдоним.

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

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Чтобы вызвать бета-API, необходимо установить пакет [Microsoft Graph бета-версии SDK для Go.](https://github.com/microsoftgraph/msgraph-beta-sdk-go)

```go
import (
    msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
    a "github.com/microsoft/kiota/authentication/go/azure"
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(...)

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)
```

---
