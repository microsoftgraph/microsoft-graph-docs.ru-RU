---
title: Использование пакетов SDK Microsoft Graph с бета-версией API
description: Описание использования пакетов SDK Microsoft Graph с бета-версией API.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: fe0272ca46b4bdea1d36048296d1a702b9e1f469
ms.sourcegitcommit: 70e09ebbf67f49a0c64ab7a275e751f8a68b8696
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/27/2020
ms.locfileid: "48771848"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a><span data-ttu-id="14c5d-103">Использование пакетов SDK Microsoft Graph с бета-версией API</span><span class="sxs-lookup"><span data-stu-id="14c5d-103">Use the Microsoft Graph SDKs with the beta API</span></span>

<span data-ttu-id="14c5d-104">Во многих пакетах SDK для Microsoft Graph по умолчанию используется конечная точка Microsoft Graph [версии 1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) .</span><span class="sxs-lookup"><span data-stu-id="14c5d-104">Many of the Microsoft Graph SDKs use the [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph endpoint by default.</span></span> <span data-ttu-id="14c5d-105">Пакеты SDK можно использовать с конечной точкой [бета-версии](/graph/api/overview?view=graph-rest-beta&preserve-view=true) для непроизводственных приложений.</span><span class="sxs-lookup"><span data-stu-id="14c5d-105">The SDKs can be used with the [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) endpoint for non-production applications.</span></span> <span data-ttu-id="14c5d-106">Метод доступа к конечной точке бета-версии зависит от того, какой пакет SDK используется.</span><span class="sxs-lookup"><span data-stu-id="14c5d-106">The method for accessing the beta endpoint depends on which SDK you are using.</span></span>

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[<span data-ttu-id="14c5d-107">C#</span><span class="sxs-lookup"><span data-stu-id="14c5d-107">C#</span></span>](#tab/CS)

<span data-ttu-id="14c5d-108">Для вызова бета-версии API необходимо установить пакет [Microsoft. Graph. Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) .</span><span class="sxs-lookup"><span data-stu-id="14c5d-108">In order to call the beta API, you must install the [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) package.</span></span> <span data-ttu-id="14c5d-109">Использование совпадает с `Microsoft.Graph` пакетом.</span><span class="sxs-lookup"><span data-stu-id="14c5d-109">Usage is the same as the `Microsoft.Graph` package.</span></span>

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[<span data-ttu-id="14c5d-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="14c5d-110">TypeScript</span></span>](#tab/typeScript)

<span data-ttu-id="14c5d-111">[Клиентская библиотека JavaScript Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) может вызывать бета-версию API одним из двух способов.</span><span class="sxs-lookup"><span data-stu-id="14c5d-111">The [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) can call the beta API in one of two ways.</span></span>

- <span data-ttu-id="14c5d-112">Вы можете задать версию `MicrosoftGraph.Client` при создании.</span><span class="sxs-lookup"><span data-stu-id="14c5d-112">You can set the version on the `MicrosoftGraph.Client` when you create it.</span></span> <span data-ttu-id="14c5d-113">Все запросы, выполняемые клиентом, переходят на указанную версию.</span><span class="sxs-lookup"><span data-stu-id="14c5d-113">All requests made by the client will go to the specified version.</span></span>

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- <span data-ttu-id="14c5d-114">Вы можете задать версию в определенном запросе, используя `version` функцию для `GraphRequest` объекта.</span><span class="sxs-lookup"><span data-stu-id="14c5d-114">You can set the version on a specific request by using the `version` function on the `GraphRequest` object.</span></span>

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[<span data-ttu-id="14c5d-115">Java</span><span class="sxs-lookup"><span data-stu-id="14c5d-115">Java</span></span>](#tab/Java)

<span data-ttu-id="14c5d-116">Для вызова бета-версии API необходимо установить [пакет SDK Java для бета-версии Microsoft Graph](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span><span class="sxs-lookup"><span data-stu-id="14c5d-116">In order to call the beta API, you must install the [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span></span> <span data-ttu-id="14c5d-117">Использование совпадает с небета-версией пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="14c5d-117">Usage is the same as the non-beta SDK.</span></span>

```Java
IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="14c5d-118">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14c5d-118">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="14c5d-119">Для работы с [пакетом SDK Microsoft Graph для обжк](https://github.com/microsoftgraph/msgraph-sdk-objc) необходимо создать строку URL-адреса для API, который требуется вызвать.</span><span class="sxs-lookup"><span data-stu-id="14c5d-119">The [Microsoft Graph SDK for ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) requires you to build a URL string to the API you want to call.</span></span> <span data-ttu-id="14c5d-120">Он предоставляет константу `MSGraphBaseURL` для конечной точки v 1.0.</span><span class="sxs-lookup"><span data-stu-id="14c5d-120">It provides a constant `MSGraphBaseURL` for the v1.0 endpoint.</span></span> <span data-ttu-id="14c5d-121">Чтобы использовать бета-версию, просто замените его на `https://graph.microsoft.com/beta` .</span><span class="sxs-lookup"><span data-stu-id="14c5d-121">To use beta, you simply replace that with `https://graph.microsoft.com/beta`.</span></span>

<span data-ttu-id="14c5d-122">Однако модели в [пакете SDK моделей Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) создаются на основе объектов в API v 1.0, поэтому они могут не работать с объектами бета-версии.</span><span class="sxs-lookup"><span data-stu-id="14c5d-122">However, the models in the [Microsoft Graph Models SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) are generated from objects in the v1.0 API, so they may not work with beta objects.</span></span>

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[<span data-ttu-id="14c5d-123">PHP</span><span class="sxs-lookup"><span data-stu-id="14c5d-123">PHP</span></span>](#tab/PHP)

<span data-ttu-id="14c5d-124">[Пакет SDK Microsoft Graph для PHP](https://github.com/microsoftgraph/msgraph-sdk-php) поддерживает конечную точку и модели бета-версии.</span><span class="sxs-lookup"><span data-stu-id="14c5d-124">The [Microsoft Graph SDK for PHP](https://github.com/microsoftgraph/msgraph-sdk-php) supports the beta endpoint and models.</span></span> <span data-ttu-id="14c5d-125">Конечная точка бета-тестирования задается с помощью `setApiVersion` метода.</span><span class="sxs-lookup"><span data-stu-id="14c5d-125">You set the beta endpoint with the `setApiVersion` method.</span></span> <span data-ttu-id="14c5d-126">Вам потребуется устранить неоднозначность моделей v 1.0 и Beta путем предоставления псевдонима.</span><span class="sxs-lookup"><span data-stu-id="14c5d-126">You will need to disambiguate the v1.0 and beta models by providing an alias.</span></span>

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
