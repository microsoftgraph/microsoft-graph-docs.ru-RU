---
title: Ответы на ошибки API безопасности Microsoft Graph
description: Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: e267cda81418e7dfce1df61f389a8ed9e0d99339
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041879"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="0d3c1-103">Ответы на ошибки API безопасности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0d3c1-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="0d3c1-104">Ошибки в API безопасности Microsoft Graph возвращаются с помощью стандартного кода состояния частичного содержимого HTTP 206 и доставляются с помощью заголовка предупреждения.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="0d3c1-105">Ошибки</span><span class="sxs-lookup"><span data-stu-id="0d3c1-105">Errors</span></span>

<span data-ttu-id="0d3c1-106">API безопасности Microsoft Graph — это Федеративная служба, которая получает несколько ответов от всех поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="0d3c1-107">При получении сообщения об ошибке HTTP с помощью API безопасности Microsoft Graph он отправляет заголовку предупреждения в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="0d3c1-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format:</span></span>
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="0d3c1-108">Этот заголовок предупреждения отправляется обратно только клиентам, когда один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="0d3c1-109">Пример:</span><span class="sxs-lookup"><span data-stu-id="0d3c1-109">For example:</span></span>

- <span data-ttu-id="0d3c1-110">HttpStatusCode. запрещено (403) может быть возвращено, если доступ к ресурсу не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="0d3c1-111">Если время ожидания поставщика истекло, в заголовке предупреждения возвращается HttpStatusCode. Гатевайтимеаут (504).</span><span class="sxs-lookup"><span data-stu-id="0d3c1-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="0d3c1-112">Если происходит ошибка внутреннего поставщика, в заголовке предупреждения используется HttpStatusCode. Интерналсервереррор (500).</span><span class="sxs-lookup"><span data-stu-id="0d3c1-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="0d3c1-113">Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждения, так как эти коды являются ожидаемыми для успешного выполнения или когда данные не были найдены соответственно.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="0d3c1-114">В федеративной системе ожидается 404, но ожидается, что данные не будут найдены одному или нескольким, но не всем, поставщикам.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="0d3c1-115">Пример</span><span class="sxs-lookup"><span data-stu-id="0d3c1-115">Example</span></span>

<span data-ttu-id="0d3c1-116">Пользователь запрашивает `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="0d3c1-117">Так как 404 и 200, ожидаемые условия, заголовок предупреждения содержит следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="0d3c1-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="0d3c1-118">**Примечание:** Каждый заголовок HTTP является коллекцией подэлементов, поэтому пользователи могут перечислить заголовок предупреждения и проверить все элементы.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="threat-indicator-bulk-action-errors"></a><span data-ttu-id="0d3c1-119">Ошибки массовых действий индикатора угроз</span><span class="sxs-lookup"><span data-stu-id="0d3c1-119">Threat indicator bulk action errors</span></span>

<span data-ttu-id="0d3c1-120">Групповые действия (создание, обновление, удаление) могут создавать два различных возможных кода ошибки:</span><span class="sxs-lookup"><span data-stu-id="0d3c1-120">Bulk actions (create, update, delete) can generate two different potential error codes:</span></span> 

- <span data-ttu-id="0d3c1-121">Код ошибки 400 указывает на то, что во время сериализации получено сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-121">A 400 error code indicates that the body provided had an error during serialization.</span></span>
- <span data-ttu-id="0d3c1-122">Код ошибки 206 указывает на то, что одно или несколько массовых действий завершились неудачно, если они были объединены со своим поставщиком.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-122">A 206 error code indicates that one or more of the bulk actions failed when it was federated out to its provider.</span></span> <span data-ttu-id="0d3c1-123">Ответ будет содержать сведения об успешном выполнении и ошибках отдельных поставщиков для каждого индикатора логики операций с угрозами.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-123">The response will contain success/error data from the individual providers for each threat intelligence indicator.</span></span> <span data-ttu-id="0d3c1-124">В отличие от [оповещений](https://docs.microsoft.com/en-us/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), все возможные сведения об ошибках будут содержаться в теле ответа для массовых действий [тииндикатор](https://docs.microsoft.com/en-us/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) .</span><span class="sxs-lookup"><span data-stu-id="0d3c1-124">Unlike [alerts](https://docs.microsoft.com/en-us/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), all potential error information will be contained within the body of the response for [tiIndicator](https://docs.microsoft.com/en-us/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) bulk actions.</span></span>

## <a name="constraints"></a><span data-ttu-id="0d3c1-125">Провероч</span><span class="sxs-lookup"><span data-stu-id="0d3c1-125">Constraints</span></span>

<span data-ttu-id="0d3c1-126">Параметр `$top` запроса OData имеет предел в 1000 оповещений, а сочетание `$top`  +  `$skip` параметров запроса OData не может превышать 6000 оповещений.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-126">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="0d3c1-127">Например, `/security/alerts?$top=10&$skip=5990` вернет код отклика `200 OK`, но `/security/alerts?$top=10&$skip=5991` вернет код отклика `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-127">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="0d3c1-128">Для этого ограничения требуется использовать параметр запроса `$filter` OData с `eventDateTime` объектом Alert из API безопасности Microsoft Graph, используя `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` и заменив значение DateTime на Последнее (6000th) оповещение.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-128">A work-round for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="0d3c1-129">Кроме того, можно задать диапазон для объекта `eventDateTime`; Пример: `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z`.</span><span class="sxs-lookup"><span data-stu-id="0d3c1-129">You can also set a range for the `eventDateTime`; for example, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z`.</span></span>

## <a name="see-also"></a><span data-ttu-id="0d3c1-130">См. также</span><span class="sxs-lookup"><span data-stu-id="0d3c1-130">See also</span></span>

<span data-ttu-id="0d3c1-131">Если у вас возникли проблемы с авторизацией, обратитесь к разделу [авторизация и API безопасности Microsoft Graph](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="0d3c1-131">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
