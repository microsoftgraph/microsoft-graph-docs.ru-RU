---
title: Ответы на ошибки API безопасности Microsoft Graph
description: Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 0c85fb6ffe9881960226ec4dc73a7487ce764d94
ms.sourcegitcommit: f359d8d3946af55dc76a02bb7bf522a4d50a2707
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/26/2019
ms.locfileid: "39263239"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="10555-103">Ответы на ошибки API безопасности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="10555-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="10555-104">Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.</span><span class="sxs-lookup"><span data-stu-id="10555-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="10555-105">Ошибки</span><span class="sxs-lookup"><span data-stu-id="10555-105">Errors</span></span>

<span data-ttu-id="10555-106">API безопасности Microsoft Graph — это Федеративная служба, которая получает несколько ответов от всех поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="10555-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="10555-107">При получении сообщения об ошибке HTTP с помощью API безопасности Microsoft Graph он отправляет заголовку предупреждения в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="10555-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="10555-108">Этот заголовок предупреждения отправляется обратно только клиентам, когда один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404.</span><span class="sxs-lookup"><span data-stu-id="10555-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="10555-109">Например:</span><span class="sxs-lookup"><span data-stu-id="10555-109">For example:</span></span>

- <span data-ttu-id="10555-110">HttpStatusCode. запрещено (403) может быть возвращено, если доступ к ресурсу не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="10555-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="10555-111">Если время ожидания поставщика истекло, в заголовке предупреждения возвращается HttpStatusCode. Гатевайтимеаут (504).</span><span class="sxs-lookup"><span data-stu-id="10555-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="10555-112">Если происходит ошибка внутреннего поставщика, в заголовке предупреждения используется HttpStatusCode. Интерналсервереррор (500).</span><span class="sxs-lookup"><span data-stu-id="10555-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="10555-113">Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждения, так как эти коды являются ожидаемыми для успешного выполнения или когда данные не были найдены соответственно.</span><span class="sxs-lookup"><span data-stu-id="10555-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="10555-114">В федеративной системе ожидается 404, но ожидается, что данные не будут найдены одному или нескольким, но не всем, поставщикам.</span><span class="sxs-lookup"><span data-stu-id="10555-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="10555-115">Пример</span><span class="sxs-lookup"><span data-stu-id="10555-115">Example</span></span>

<span data-ttu-id="10555-116">Пользователь запрашивает `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="10555-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="10555-117">Так как 404 и 200, ожидаемые условия, заголовок предупреждения содержит следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="10555-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="10555-118">**Примечание:** Каждый заголовок HTTP является коллекцией подэлементов, поэтому пользователи могут перечислить заголовок предупреждения и проверить все элементы.</span><span class="sxs-lookup"><span data-stu-id="10555-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="10555-119">Провероч</span><span class="sxs-lookup"><span data-stu-id="10555-119">Constraints</span></span>

<span data-ttu-id="10555-120">Параметр `$top` запроса OData имеет лимит в 1000 оповещений.</span><span class="sxs-lookup"><span data-stu-id="10555-120">The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="10555-121">Рекомендуется включать только `$top` `$skip` в первый запрос GET.</span><span class="sxs-lookup"><span data-stu-id="10555-121">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="10555-122">Можно использовать `@odata.nextLink` для разбивки на страницы.</span><span class="sxs-lookup"><span data-stu-id="10555-122">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="10555-123">При необходимости вы можете использовать `$skip`не более 500 оповещений.</span><span class="sxs-lookup"><span data-stu-id="10555-123">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="10555-124">Например, `/security/alerts?$top=10&$skip=500` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=501` вернет код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="10555-124">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="10555-125">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="10555-125">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

<span data-ttu-id="10555-126">Воркаараунд для этого ограничения — использовать параметр запроса `$filter` OData с `eventDateTime` объектом Alert из API безопасности Microsoft Graph, используя `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` и заменив значение DateTime на Последнее (1500th) оповещение.</span><span class="sxs-lookup"><span data-stu-id="10555-126">A workaaround for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (1500th) alert.</span></span> <span data-ttu-id="10555-127">Кроме того, можно задать диапазон для объекта `eventDateTime`; Например, *Alerts? $Filter = евентдатетиме **gt** 2018-11 –**11**T00:00:00.000 z&евентдатетиме **lt** 2018-11 –**12**T00:00:00.000 z*</span><span class="sxs-lookup"><span data-stu-id="10555-127">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="10555-128">См. также</span><span class="sxs-lookup"><span data-stu-id="10555-128">See also</span></span>

<span data-ttu-id="10555-129">Если у вас возникли проблемы с авторизацией, обратитесь к разделу [авторизация и API безопасности Microsoft Graph](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="10555-129">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
