---
title: Использование пакетов SDK Microsoft Graph с бета-версией API
description: Описание использования пакетов SDK Microsoft Graph с бета-версией API.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: a384384b4172a835160cf12b8e1fb0c06edc7fe7
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312201"
---
# <a name="use-the-microsoft-graph-sdks-with-the-beta-api"></a><span data-ttu-id="c4b99-103">Использование пакетов SDK Microsoft Graph с бета-версией API</span><span class="sxs-lookup"><span data-stu-id="c4b99-103">Use the Microsoft Graph SDKs with the beta API</span></span>

<span data-ttu-id="c4b99-104">По умолчанию пакет SDK Microsoft Graph использует конечную точку Microsoft Graph [версии 1.0](/graph/api/overview?view=graph-rest-1.0) .</span><span class="sxs-lookup"><span data-stu-id="c4b99-104">The Microsoft Graph SDKs use the [v1.0](/graph/api/overview?view=graph-rest-1.0) Microsoft Graph endpoint by default.</span></span> <span data-ttu-id="c4b99-105">Пакеты SDK можно использовать с конечной точкой [бета-версии](/graph/api/overview?view=graph-rest-beta) для непроизводственных приложений.</span><span class="sxs-lookup"><span data-stu-id="c4b99-105">The SDKs can be used with the [beta](/graph/api/overview?view=graph-rest-beta) endpoint for non-production applications.</span></span> <span data-ttu-id="c4b99-106">Метод доступа к конечной точке бета-версии зависит от того, какой пакет SDK используется.</span><span class="sxs-lookup"><span data-stu-id="c4b99-106">The method for accessing the beta endpoint depends on which SDK you are using.</span></span>

[!INCLUDE [beta-disclaimer](../../api-reference/includes/beta-disclaimer.md)]

# <a name="c"></a>[<span data-ttu-id="c4b99-107">C#</span><span class="sxs-lookup"><span data-stu-id="c4b99-107">C#</span></span>](#tab/CS)

<span data-ttu-id="c4b99-108">Для вызова бета-версии API необходимо установить пакет [Microsoft. Graph. Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) .</span><span class="sxs-lookup"><span data-stu-id="c4b99-108">In order to call the beta API, you must install the [Microsoft.Graph.Beta](https://www.nuget.org/packages/Microsoft.Graph.Beta) package.</span></span> <span data-ttu-id="c4b99-109">Использование совпадает с `Microsoft.Graph` пакетом.</span><span class="sxs-lookup"><span data-stu-id="c4b99-109">Usage is the same as the `Microsoft.Graph` package.</span></span>

```csharp
using Microsoft.Graph.Beta;

// Create a new instance of GraphServiceClient.
GraphServiceClient graphClient = new GraphServiceClient(...);
```

## <a name="typescript"></a>[<span data-ttu-id="c4b99-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="c4b99-110">TypeScript</span></span>](#tab/typeScript)

<span data-ttu-id="c4b99-111">[Клиентская библиотека JavaScript Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-javascript) может вызывать бета-версию API одним из двух способов.</span><span class="sxs-lookup"><span data-stu-id="c4b99-111">The [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) can call the beta API in one of two ways.</span></span>

- <span data-ttu-id="c4b99-112">Вы можете задать версию `MicrosoftGraph.Client` при создании.</span><span class="sxs-lookup"><span data-stu-id="c4b99-112">You can set the version on the `MicrosoftGraph.Client` when you create it.</span></span> <span data-ttu-id="c4b99-113">Все запросы, выполняемые клиентом, переходят на указанную версию.</span><span class="sxs-lookup"><span data-stu-id="c4b99-113">All requests made by the client will go to the specified version.</span></span>

    ```typescript
    const clientOptions: ClientOptions = {
      defaultVersion: 'beta',
      ...
    };

    // Initialize Graph client
    const client = MicrosoftGraph.Client.initWithMiddleware(clientOptions);
    ```

- <span data-ttu-id="c4b99-114">Вы можете задать версию в определенном запросе, используя `version` функцию для `GraphRequest` объекта.</span><span class="sxs-lookup"><span data-stu-id="c4b99-114">You can set the version on a specific request by using the `version` function on the `GraphRequest` object.</span></span>

    ```typescript
    const user = await client
      .api('/me')
      .version('beta')
      .get();
    ```

# <a name="java"></a>[<span data-ttu-id="c4b99-115">Java</span><span class="sxs-lookup"><span data-stu-id="c4b99-115">Java</span></span>](#tab/Java)

<span data-ttu-id="c4b99-116">Для вызова бета-версии API необходимо установить [пакет SDK Java для бета-версии Microsoft Graph](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span><span class="sxs-lookup"><span data-stu-id="c4b99-116">In order to call the beta API, you must install the [Microsoft Graph Beta Java SDK](https://github.com/microsoftgraph/msgraph-beta-sdk-java).</span></span> <span data-ttu-id="c4b99-117">Использование совпадает с небета-версией пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="c4b99-117">Usage is the same as the non-beta SDK.</span></span>

# <a name="objective-c"></a>[<span data-ttu-id="c4b99-118">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4b99-118">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="c4b99-119">Для работы с [пакетом SDK Microsoft Graph для обжк](https://github.com/microsoftgraph/msgraph-sdk-objc) необходимо создать строку URL-адреса для API, который требуется вызвать.</span><span class="sxs-lookup"><span data-stu-id="c4b99-119">The [Microsoft Graph SDK for ObjC](https://github.com/microsoftgraph/msgraph-sdk-objc) requires you to build a URL string to the API you want to call.</span></span> <span data-ttu-id="c4b99-120">Он предоставляет константу `MSGraphBaseURL` для конечной точки v 1.0.</span><span class="sxs-lookup"><span data-stu-id="c4b99-120">It provides a constant `MSGraphBaseURL` for the v1.0 endpoint.</span></span> <span data-ttu-id="c4b99-121">Чтобы использовать бета-версию, просто замените его на `https://graph.microsoft.com/beta` .</span><span class="sxs-lookup"><span data-stu-id="c4b99-121">To use beta, you simply replace that with `https://graph.microsoft.com/beta`.</span></span>

<span data-ttu-id="c4b99-122">Однако модели в [пакете SDK моделей Microsoft Graph](https://github.com/microsoftgraph/msgraph-sdk-objc-models) создаются на основе объектов в API v 1.0, поэтому они могут не работать с объектами бета-версии.</span><span class="sxs-lookup"><span data-stu-id="c4b99-122">However, the models in the [Microsoft Graph Models SDK](https://github.com/microsoftgraph/msgraph-sdk-objc-models) are generated from objects in the v1.0 API, so they may not work with beta objects.</span></span>

```objc
// GET /me
NSString* meUrlString = [NSString stringWithFormat:@"%@/me", "https://graph.microsoft.com/beta"];

NSURL* meUrl = [[NSURL alloc] initWithString:meUrlString];

NSMutableURLRequest* meRequest = [[NSMutableURLRequest alloc] initWithURL:meUrl];
```

---
