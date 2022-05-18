---
title: Использование пакетов SDK Graph Майкрософт с бета-версией API
description: Описывает использование пакетов SDK Graph Майкрософт с бета-версией API.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 2761c88fe43a5f1994c53ae8016486f2fa139962
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65460689"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a>Использование пакетов SDK Graph Майкрософт с бета-версией API

Многие пакеты SDK Graph Майкрософт по умолчанию используют [конечную точку Microsoft Graph версии 1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false). Пакеты SDK можно использовать с конечной [точкой бета-версии](/graph/api/overview?view=graph-rest-beta&preserve-view=true) для нерабочих приложений. Метод доступа к конечной точке бета-версии зависит от используемого пакета SDK.

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD025 -->
# <a name="c"></a>[C#](#tab/CS)

Чтобы вызвать API бета-версии, необходимо установить [Microsoft.Graph. Бета-версия](https://www.nuget.org/packages/Microsoft.Graph.Beta) пакета. Использование совпадает с использованием `Microsoft.Graph` пакета.

```csharp
// Version 5.x
using Microsoft.Graph.Beta;
// Version 4.x and earlier
// using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[TypeScript](#tab/typeScript)

[Клиентская Graph Microsoft JavaScript](https://github.com/microsoftgraph/msgraph-sdk-javascript) может вызывать API бета-версии одним из двух способов.

- Версию можно задать при `MicrosoftGraph.Client` ее создании. Все запросы, сделанные клиентом, будут перенаходить к указанной версии.

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- Версию можно задать по определенному запросу с помощью функции `version` в объекте `GraphRequest` .

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[Java](#tab/Java)

Чтобы вызвать API бета-версии, необходимо установить [пакет SDK Microsoft Graph Java beta](https://github.com/microsoftgraph/msgraph-beta-sdk-java). Использование совпадает с использованием пакета SDK, отличного от бета-версии.

```Java
GraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[Objective-C](#tab/Objective-C)

Пакет [microsoft Graph SDK для ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) требует создать строку URL-адреса для API, который вы хотите вызвать. Он предоставляет константу `MSGraphBaseURL` для конечной точки версии 1.0. Чтобы использовать бета-версию, просто замените ее на `https://graph.microsoft.com/beta`.

Однако модели в пакете [SDK microsoft Graph Models](https://github.com/microsoftgraph/msgraph-sdk-objc-models) создаются из объектов в API версии 1.0, поэтому они могут не работать с бета-объектами.

```objectivec
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[PHP](#tab/PHP)

Пакет [Microsoft Graph SDK для PHP](https://github.com/microsoftgraph/msgraph-sdk-php) поддерживает бета-версию конечной точки и моделей. Вы задаете конечную точку бета-версии с помощью `setApiVersion` этого метода. Необходимо устранить неоднозначность моделей версии 1.0 и бета-версий, указав псевдоним.

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

# <a name="go"></a>[Go](#tab/Go)

[!INCLUDE [go-sdk-preview](../../includes/go-sdk-preview.md)]

Чтобы вызвать API бета-версии, необходимо [установить пакет Microsoft Graph Beta SDK для Go](https://github.com/microsoftgraph/msgraph-beta-sdk-go).

```go
import (
    msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
    a "github.com/microsoft/kiota-authentication-azure-go"
)

auth, err := a.NewAzureIdentityAuthenticationProviderWithScopes(...)

adapter, err := msgraphsdk.NewGraphRequestAdapter(auth)

client := msgraphsdk.NewGraphServiceClient(adapter)
```

---
