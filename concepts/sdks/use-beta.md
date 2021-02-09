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
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a><span data-ttu-id="6436c-103">Использование SDKs Microsoft Graph с бета-версией API</span><span class="sxs-lookup"><span data-stu-id="6436c-103">Use the Microsoft Graph SDKs with the beta API</span></span>

<span data-ttu-id="6436c-104">Многие SDKs Microsoft Graph используют конечную точку Microsoft Graph [1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6436c-104">Many of the Microsoft Graph SDKs use the [v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=false) Microsoft Graph endpoint by default.</span></span> <span data-ttu-id="6436c-105">SDKs можно использовать с конечной точкой [бета-версии](/graph/api/overview?view=graph-rest-beta&preserve-view=true) для непроизводивых приложений.</span><span class="sxs-lookup"><span data-stu-id="6436c-105">The SDKs can be used with the [beta](/graph/api/overview?view=graph-rest-beta&preserve-view=true) endpoint for non-production applications.</span></span> <span data-ttu-id="6436c-106">Способ доступа к конечной точке бета-версии зависит от используемого SDK.</span><span class="sxs-lookup"><span data-stu-id="6436c-106">The method for accessing the beta endpoint depends on which SDK you are using.</span></span>

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[<span data-ttu-id="6436c-107">C#</span><span class="sxs-lookup"><span data-stu-id="6436c-107">C#</span></span>](#tab/CS)

<span data-ttu-id="6436c-108">Чтобы вызвать бета-версию API, необходимо установить пакет [Microsoft.Graph.Beta.](https://www.nuget.org/packages/Microsoft.Graph.Beta)</span><span class="sxs-lookup"><span data-stu-id="6436c-108">In order to call the beta API, you must install the [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) package.</span></span> <span data-ttu-id="6436c-109">Использование такое же, как и у `Microsoft.Graph` пакета.</span><span class="sxs-lookup"><span data-stu-id="6436c-109">Usage is the same as the `Microsoft.Graph` package.</span></span>

```csharp
using Microsoft.Graph;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

# <a name="typescript"></a>[<span data-ttu-id="6436c-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="6436c-110">TypeScript</span></span>](#tab/typeScript)

<span data-ttu-id="6436c-111">Клиентская [библиотека JavaScript microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) может вызывать бета-версию API одним из двух способов.</span><span class="sxs-lookup"><span data-stu-id="6436c-111">The [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) can call the beta API in one of two ways.</span></span>

- <span data-ttu-id="6436c-112">Версию можно установить при `MicrosoftGraph.Client` ее создании.</span><span class="sxs-lookup"><span data-stu-id="6436c-112">You can set the version on the `MicrosoftGraph.Client` when you create it.</span></span> <span data-ttu-id="6436c-113">Все запросы, сделанные клиентом, будут перенаходить к указанной версии.</span><span class="sxs-lookup"><span data-stu-id="6436c-113">All requests made by the client will go to the specified version.</span></span>

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- <span data-ttu-id="6436c-114">Версию можно установить по конкретному запросу с помощью `version` функции `GraphRequest` объекта.</span><span class="sxs-lookup"><span data-stu-id="6436c-114">You can set the version on a specific request by using the `version` function on the `GraphRequest` object.</span></span>

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[<span data-ttu-id="6436c-115">Java</span><span class="sxs-lookup"><span data-stu-id="6436c-115">Java</span></span>](#tab/Java)

<span data-ttu-id="6436c-116">Чтобы вызвать бета-версию API, необходимо установить [Java SDK для Бета-версии Microsoft Graph.](https://github.com/microsoftgraph/msgraph-beta-sdk-java)</span><span class="sxs-lookup"><span data-stu-id="6436c-116">In order to call the beta API, you must install the [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span></span> <span data-ttu-id="6436c-117">Использование не является бета-версией SDK.</span><span class="sxs-lookup"><span data-stu-id="6436c-117">Usage is the same as the non-beta SDK.</span></span>

```Java
IGraphServiceClient graphClient = GraphServiceClient
    .builder()
    .authenticationProvider(authProvider)
    .buildClient();
```

# <a name="objective-c"></a>[<span data-ttu-id="6436c-118">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6436c-118">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6436c-119">Для [SDK Microsoft Graph для ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) требуется создать строку URL-адреса для API, который вы хотите вызвать.</span><span class="sxs-lookup"><span data-stu-id="6436c-119">The [Microsoft Graph SDK for ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) requires you to build a URL string to the API you want to call.</span></span> <span data-ttu-id="6436c-120">Он предоставляет `MSGraphBaseURL` константы для конечной точки v1.0.</span><span class="sxs-lookup"><span data-stu-id="6436c-120">It provides a constant `MSGraphBaseURL` for the v1.0 endpoint.</span></span> <span data-ttu-id="6436c-121">Чтобы использовать бета-версию, просто замените ее на `https://graph.microsoft.com/beta` .</span><span class="sxs-lookup"><span data-stu-id="6436c-121">To use beta, you simply replace that with `https://graph.microsoft.com/beta`.</span></span>

<span data-ttu-id="6436c-122">Однако модели в [SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) моделей Microsoft Graph создаются из объектов в API версии 1.0, поэтому они могут не работать с бета-объектами.</span><span class="sxs-lookup"><span data-stu-id="6436c-122">However, the models in the [Microsoft Graph Models SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) are generated from objects in the v1.0 API, so they may not work with beta objects.</span></span>

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

# <a name="php"></a>[<span data-ttu-id="6436c-123">PHP</span><span class="sxs-lookup"><span data-stu-id="6436c-123">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6436c-124">Microsoft [Graph SDK для PHP](https://github.com/microsoftgraph/msgraph-sdk-php) поддерживает конечную точку и модели бета-версии.</span><span class="sxs-lookup"><span data-stu-id="6436c-124">The [Microsoft Graph SDK for PHP](https://github.com/microsoftgraph/msgraph-sdk-php) supports the beta endpoint and models.</span></span> <span data-ttu-id="6436c-125">С помощью этого метода можно настроить конечную точку `setApiVersion` бета-версии.</span><span class="sxs-lookup"><span data-stu-id="6436c-125">You set the beta endpoint with the `setApiVersion` method.</span></span> <span data-ttu-id="6436c-126">Вам потребуется улиться в неоднозначности моделей версии 1.0 и бета-версии, предоставив псевдоним.</span><span class="sxs-lookup"><span data-stu-id="6436c-126">You will need to disambiguate the v1.0 and beta models by providing an alias.</span></span>

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
