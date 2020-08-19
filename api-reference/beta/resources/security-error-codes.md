---
title: Ответы на ошибки API безопасности Microsoft Graph
description: Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: bf863b7a0acc2b7ece38f10272497cb3e5267d07
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810393"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="d5392-103">Ответы на ошибки API безопасности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d5392-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="d5392-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5392-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5392-105">Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.</span><span class="sxs-lookup"><span data-stu-id="d5392-105">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="d5392-106">Ошибки</span><span class="sxs-lookup"><span data-stu-id="d5392-106">Errors</span></span>

<span data-ttu-id="d5392-107">API безопасности Microsoft Graph — это Федеративная служба, которая получает несколько ответов от всех поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="d5392-107">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="d5392-108">При получении сообщения об ошибке HTTP с помощью API безопасности Microsoft Graph он отправляет заголовку предупреждения в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="d5392-108">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="d5392-109">Этот заголовок предупреждения отправляется обратно только клиентам, когда один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404.</span><span class="sxs-lookup"><span data-stu-id="d5392-109">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="d5392-110">Пример:</span><span class="sxs-lookup"><span data-stu-id="d5392-110">For example:</span></span>

- <span data-ttu-id="d5392-111">HttpStatusCode. запрещено (403) может быть возвращено, если доступ к ресурсу не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="d5392-111">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="d5392-112">Если время ожидания поставщика истекло, в заголовке предупреждения возвращается HttpStatusCode. Гатевайтимеаут (504).</span><span class="sxs-lookup"><span data-stu-id="d5392-112">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="d5392-113">Если происходит ошибка внутреннего поставщика, в заголовке предупреждения используется HttpStatusCode. Интерналсервереррор (500).</span><span class="sxs-lookup"><span data-stu-id="d5392-113">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="d5392-114">Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждения, так как эти коды являются ожидаемыми для успешного выполнения или когда данные не были найдены соответственно.</span><span class="sxs-lookup"><span data-stu-id="d5392-114">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="d5392-115">В федеративной системе ожидается 404, но ожидается, что данные не будут найдены одному или нескольким, но не всем, поставщикам.</span><span class="sxs-lookup"><span data-stu-id="d5392-115">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="d5392-116">Пример</span><span class="sxs-lookup"><span data-stu-id="d5392-116">Example</span></span>

<span data-ttu-id="d5392-117">Пользователь запрашивает `security/alerts/{alert_id}` .</span><span class="sxs-lookup"><span data-stu-id="d5392-117">A user asks for `security/alerts/{alert_id}`.</span></span>

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

<span data-ttu-id="d5392-118">Так как 404 и 200, ожидаемые условия, заголовок предупреждения содержит следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="d5392-118">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="d5392-119">**Примечание:** Каждый заголовок HTTP является коллекцией подэлементов, поэтому пользователи могут перечислить заголовок предупреждения и проверить все элементы.</span><span class="sxs-lookup"><span data-stu-id="d5392-119">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="threat-indicator-bulk-action-errors"></a><span data-ttu-id="d5392-120">Ошибки массовых действий индикатора угроз</span><span class="sxs-lookup"><span data-stu-id="d5392-120">Threat indicator bulk action errors</span></span>

<span data-ttu-id="d5392-121">Групповые действия (создание, обновление, удаление) могут создавать два различных возможных кода ошибки:</span><span class="sxs-lookup"><span data-stu-id="d5392-121">Bulk actions (create, update, delete) can generate two different potential error codes:</span></span>

- <span data-ttu-id="d5392-122">Код ошибки 400 указывает на то, что во время сериализации получено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d5392-122">A 400 error code indicates that the body provided had an error during serialization.</span></span>
- <span data-ttu-id="d5392-123">Код ошибки 206 указывает на то, что одно или несколько массовых действий завершились неудачно, если они были объединены со своим поставщиком.</span><span class="sxs-lookup"><span data-stu-id="d5392-123">A 206 error code indicates that one or more of the bulk actions failed when it was federated out to its provider.</span></span> <span data-ttu-id="d5392-124">Ответ будет содержать сведения об успешном выполнении и ошибках отдельных поставщиков для каждого индикатора логики операций с угрозами.</span><span class="sxs-lookup"><span data-stu-id="d5392-124">The response will contain success/error data from the individual providers for each threat intelligence indicator.</span></span> <span data-ttu-id="d5392-125">В отличие от [оповещений](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), все возможные сведения об ошибках будут содержаться в теле ответа для массовых действий [тииндикатор](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) .</span><span class="sxs-lookup"><span data-stu-id="d5392-125">Unlike [alerts](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), all potential error information will be contained within the body of the response for [tiIndicator](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) bulk actions.</span></span>

## <a name="constraints"></a><span data-ttu-id="d5392-126">Провероч</span><span class="sxs-lookup"><span data-stu-id="d5392-126">Constraints</span></span>

<span data-ttu-id="d5392-127">`$top`Параметр запроса OData имеет лимит в 1000 оповещений.</span><span class="sxs-lookup"><span data-stu-id="d5392-127">The `$top` OData query parameter has a limit of 1000 alerts.</span></span> <span data-ttu-id="d5392-128">В первый запрос GET рекомендуется включить только параметр `$top`, но не параметр `$skip`.</span><span class="sxs-lookup"><span data-stu-id="d5392-128">We recommend that you include only `$top` and not `$skip` in your first GET query.</span></span> <span data-ttu-id="d5392-129">Для разбивки на страницы можно использовать параметр `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="d5392-129">You can use `@odata.nextLink` for pagination.</span></span> <span data-ttu-id="d5392-130">Если требуется применить параметр `$skip`, он имеет ограничение в 500 оповещений.</span><span class="sxs-lookup"><span data-stu-id="d5392-130">If you need to use `$skip`, it has a limit of 500 alerts.</span></span> <span data-ttu-id="d5392-131">Например, `/security/alerts?$top=10&$skip=500` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=501` вернет код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="d5392-131">For example, `/security/alerts?$top=10&$skip=500` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=501` will return a `400 Bad Request` response code.</span></span> <span data-ttu-id="d5392-132">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="d5392-132">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

<span data-ttu-id="d5392-133">Чтобы устранить это ограничения, используйте `$filter` параметр запроса OData с `eventDateTime` объектом Alert из API безопасности Microsoft Graph, используя `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` и заменив значение DateTime на Последнее (1500th) оповещение.</span><span class="sxs-lookup"><span data-stu-id="d5392-133">A workaround for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (1500th) alert.</span></span> <span data-ttu-id="d5392-134">Кроме того, можно задать диапазон для, например `eventDateTime` , `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z` .</span><span class="sxs-lookup"><span data-stu-id="d5392-134">You can also set a range for the `eventDateTime`; for example, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z`.</span></span>

## <a name="see-also"></a><span data-ttu-id="d5392-135">См. также</span><span class="sxs-lookup"><span data-stu-id="d5392-135">See also</span></span>

<span data-ttu-id="d5392-136">Если у вас возникли проблемы с авторизацией, обратитесь к разделу [авторизация и API безопасности Microsoft Graph](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="d5392-136">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
