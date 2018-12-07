---
title: Сообщения об ошибках API безопасности Microsoft Graph
description: Ошибки в API-Интерфейс безопасности Microsoft Graph возвращаются с помощью стандартных код состояния HTTP 206 Частичное контента и являются через заголовок предупреждения.
ms.openlocfilehash: 9ac124f763e7668471f89beffb968cb883217e80
ms.sourcegitcommit: 4aebfaefc23e02a98b2fec35958cd2110020f15f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/06/2018
ms.locfileid: "27184506"
---
# <a name="microsoft-graph-security-api-error-responses"></a><span data-ttu-id="8da54-103">Сообщения об ошибках API безопасности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8da54-103">Microsoft Graph Security API error responses</span></span>

<span data-ttu-id="8da54-104">Ошибки в API-Интерфейс безопасности Microsoft Graph возвращаются с помощью стандартных код состояния HTTP 206 Частичное контента и являются через заголовок предупреждения.</span><span class="sxs-lookup"><span data-stu-id="8da54-104">Errors in the Microsoft Graph Security API are returned using the standard HTTP 206 Partial Content status code and are delivered via a warning header.</span></span>

## <a name="errors"></a><span data-ttu-id="8da54-105">Ошибки</span><span class="sxs-lookup"><span data-stu-id="8da54-105">Errors</span></span>

<span data-ttu-id="8da54-106">API-Интерфейс безопасности Microsoft Graph — федеративных служба, которая получает несколько ответов от всех поставщиков данных.</span><span class="sxs-lookup"><span data-stu-id="8da54-106">The Microsoft Graph Security API is a federated service that receives multiple responses from all data providers.</span></span> <span data-ttu-id="8da54-107">При получении ошибки HTTP с API-Интерфейс безопасности Microsoft Graph возвращается предупреждение заголовка в следующем формате:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="8da54-107">When an HTTP error is received by the Microsoft Graph Security API, it will send back a warning header in the following format: <!-- { "blockType": "ignored" } --></span></span>

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

<span data-ttu-id="8da54-108">Этот заголовок предупреждение только отправляется обратно клиентов при один из поставщиков данных возвращает код ошибки, отличный от 2xx или 404.</span><span class="sxs-lookup"><span data-stu-id="8da54-108">This warning header is only sent back to clients when one of the data providers returns an error code other than 2xx or 404.</span></span> <span data-ttu-id="8da54-109">Пример:</span><span class="sxs-lookup"><span data-stu-id="8da54-109">For example:</span></span>

- <span data-ttu-id="8da54-110">HttpStatusCode.Forbidden (403) может быть возвращено, если не предоставляется доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="8da54-110">HttpStatusCode.Forbidden (403) might be returned if the access to the resource is not granted.</span></span>
- <span data-ttu-id="8da54-111">Если поставщик времени ожидания, HttpStatusCode.GatewayTimeout (504) возвращается в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="8da54-111">If a provider times out, HttpStatusCode.GatewayTimeout (504) is returned in the warning header.</span></span>
- <span data-ttu-id="8da54-112">Если происходит ошибка внутреннего поставщика HttpStatusCode.InternalServerError (500) используется в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="8da54-112">If an internal provider error happens, HttpStatusCode.InternalServerError (500) is used in the warning header.</span></span>

<span data-ttu-id="8da54-113">Если поставщик данных возвращает 2xx или 404, он не отображается в заголовке предупреждение так как эти коды для успеха или когда данные не найдены соответственно.</span><span class="sxs-lookup"><span data-stu-id="8da54-113">If a data provider returns 2xx or 404, it’s not shown in the warning header because these codes are expected for success or when data is not found respectively.</span></span> <span data-ttu-id="8da54-114">В системе с федеративным 404 не найден ожидается как количество раз данные известно только один или несколько, но не для всех поставщиков.</span><span class="sxs-lookup"><span data-stu-id="8da54-114">In a federated system, a 404 not found is expected as many times the data is only known to one or several, but not all, providers.</span></span>

## <a name="example"></a><span data-ttu-id="8da54-115">Пример</span><span class="sxs-lookup"><span data-stu-id="8da54-115">Example</span></span>

<span data-ttu-id="8da54-116">Пользователь запрашивает `security/alerts/{alert_id}`.</span><span class="sxs-lookup"><span data-stu-id="8da54-116">A user asks for `security/alerts/{alert_id}`.</span></span>

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

<span data-ttu-id="8da54-117">Так как 404 и 200 ожидаемых условиях, предупреждение заголовка содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8da54-117">Because both 404 and 200 are expected conditions, the warning header contains the following:</span></span>

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> <span data-ttu-id="8da54-118">**Примечание:** Каждого заголовка HTTP — это коллекция элементов, чтобы пользователи могли предупреждение заголовок перечислить и проверить все элементы.</span><span class="sxs-lookup"><span data-stu-id="8da54-118">**Note:** Each HTTP header is a collection of subitems, so users can enumerate the Warning header and check all items.</span></span>

## <a name="constraints"></a><span data-ttu-id="8da54-119">Ограничения</span><span class="sxs-lookup"><span data-stu-id="8da54-119">Constraints</span></span>

<span data-ttu-id="8da54-120">`$top` Параметр запроса OData для которого настроено ограничение 1000 оповещений и сочетание `$top`  +  `$skip` параметров не может превышать 6000 оповещения запросов OData.</span><span class="sxs-lookup"><span data-stu-id="8da54-120">The `$top` OData query parameter has a limit of 1000 alerts, and a combination of `$top` + `$skip` OData query parameters cannot exceed 6000 alerts.</span></span> <span data-ttu-id="8da54-121">Например `/security/alerts?$top=10&$skip=5990` возвращает `200 OK` код ответа, но `/security/alerts?$top=10&$skip=5991` возвращает `400 Bad Request` код ответа.</span><span class="sxs-lookup"><span data-stu-id="8da54-121">For example, `/security/alerts?$top=10&$skip=5990` will return a `200 OK` response code, but `/security/alerts?$top=10&$skip=5991` will return a `400 Bad Request` response code.</span></span>

<span data-ttu-id="8da54-122">Обходной предела является использование `$filter` параметр запроса OData с `eventDateTime` оповещения сущности из Microsoft Graph безопасности API, с помощью `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` и замените значение даты и времени последнего предупреждения (6000th).</span><span class="sxs-lookup"><span data-stu-id="8da54-122">A work-around for this limit is to use the `$filter` OData query parameter with the `eventDateTime` of the alert entity from the Microsoft Graph Security API, using `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` and replacing the dateTime value with the last (6000th) alert.</span></span> <span data-ttu-id="8da54-123">Можно также задать диапазон для `eventDateTime`; например *alerts?$ фильтра = Дата и время **gt** 2018-11 -**11**T00:00:00.000Z & Дата и время **lt** 2018-11 -**12**T00:00:00.000Z*</span><span class="sxs-lookup"><span data-stu-id="8da54-123">You can also set a range for the `eventDateTime`; for example, *alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z*</span></span>

## <a name="see-also"></a><span data-ttu-id="8da54-124">См. также</span><span class="sxs-lookup"><span data-stu-id="8da54-124">See also</span></span>

<span data-ttu-id="8da54-125">Если у вас возникли неполадки с авторизации, видеть [авторизации и API -Интерфейс Microsoft Graph безопасности](/graph/security-authorization).</span><span class="sxs-lookup"><span data-stu-id="8da54-125">If you’re having trouble with authorization, see [Authorization and the Microsoft Graph Security API](/graph/security-authorization).</span></span>
