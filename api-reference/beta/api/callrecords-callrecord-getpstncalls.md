---
title: 'callRecord: getPstnCalls'
description: Получить журнал вызовов PSTN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 57f29fdef863671c36f8b9e063c99a370e1173d1
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697195"
---
# <a name="callrecord-getpstncalls"></a><span data-ttu-id="8677c-103">callRecord: getPstnCalls</span><span class="sxs-lookup"><span data-stu-id="8677c-103">callRecord: getPstnCalls</span></span>

<span data-ttu-id="8677c-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="8677c-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8677c-105">Получите журнал вызовов PSTN в качестве коллекции записей [pstnCallLogRow.](../resources/callrecords-pstncalllogrow.md)</span><span class="sxs-lookup"><span data-stu-id="8677c-105">Get log of PSTN calls as a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="8677c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8677c-106">Permissions</span></span>

<span data-ttu-id="8677c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8677c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8677c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8677c-109">Permission type</span></span>|<span data-ttu-id="8677c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8677c-110">Permissions (from least to most privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8677c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8677c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8677c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8677c-112">Not supported.</span></span> |
| <span data-ttu-id="8677c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8677c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8677c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8677c-114">Not supported.</span></span> |
| <span data-ttu-id="8677c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8677c-115">Application</span></span>                            | <span data-ttu-id="8677c-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8677c-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8677c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8677c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a><span data-ttu-id="8677c-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="8677c-118">Function parameters</span></span>

<span data-ttu-id="8677c-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8677c-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8677c-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8677c-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8677c-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="8677c-121">Parameter</span></span>|<span data-ttu-id="8677c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8677c-122">Type</span></span>|<span data-ttu-id="8677c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8677c-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8677c-124">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="8677c-124">fromDateTime</span></span>|<span data-ttu-id="8677c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8677c-125">DateTimeOffset</span></span>|<span data-ttu-id="8677c-126">Начало диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="8677c-126">Start of time range to query.</span></span> <span data-ttu-id="8677c-127">UTC включительно.</span><span class="sxs-lookup"><span data-stu-id="8677c-127">UTC, inclusive.</span></span><br/><span data-ttu-id="8677c-128">Диапазон времени зависит от времени начала вызова.</span><span class="sxs-lookup"><span data-stu-id="8677c-128">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="8677c-129">toDateTime</span><span class="sxs-lookup"><span data-stu-id="8677c-129">toDateTime</span></span>|<span data-ttu-id="8677c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8677c-130">DateTimeOffset</span></span>|<span data-ttu-id="8677c-131">Конец диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="8677c-131">End of time range to query.</span></span> <span data-ttu-id="8677c-132">UTC включительно.</span><span class="sxs-lookup"><span data-stu-id="8677c-132">UTC, inclusive.</span></span>|

> [!IMPORTANT]
> <span data-ttu-id="8677c-133">Значения **fromDateTime** и **toDateTime** не могут быть больше диапазона дат в 90 дней.</span><span class="sxs-lookup"><span data-stu-id="8677c-133">The **fromDateTime** and **toDateTime** values cannot be more than a date range of 90 days.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8677c-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8677c-134">Request headers</span></span>

|<span data-ttu-id="8677c-135">Имя</span><span class="sxs-lookup"><span data-stu-id="8677c-135">Name</span></span>|<span data-ttu-id="8677c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="8677c-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8677c-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8677c-137">Authorization</span></span>|<span data-ttu-id="8677c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8677c-p105">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="8677c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8677c-140">Response</span></span>

<span data-ttu-id="8677c-141">В случае успешной работы эта функция возвращает код ответа и коллекцию записей `200 OK` [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8677c-141">If successful, this function returns a `200 OK` response code and a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="8677c-142">Если в диапазоне дат более 1000 записей, тело также включает URL-адрес для запроса следующей страницы записей `@odata.NextLink` вызовов.</span><span class="sxs-lookup"><span data-stu-id="8677c-142">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="8677c-143">Последняя страница в диапазоне дат не имеет `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="8677c-143">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="8677c-144">Дополнительные сведения см. в дополнительных сведениях [о сборе данных Microsoft Graph в приложении.](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="8677c-144">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="8677c-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="8677c-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8677c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8677c-146">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="8677c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8677c-147">Response</span></span>

<span data-ttu-id="8677c-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8677c-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.pstnCallLogRow)"
}
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.pstnCallLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9c4984c7-6c3c-427d-a30c-bd0b2eacee90",
            "callId": "1835317186_112562680@61.221.3.176",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:08.2589935Z",
            "endDateTime": "2019-11-01T00:03:47.2589935Z",
            "duration": 219,
            "charge": 0.00,
            "callType": "user_in",
            "currency": "USD",
            "calleeNumber": "+1234567890",
            "usageCountryCode": "US",
            "tenantCountryCode": "US",
            "connectionCharge": 0.00,
            "callerNumber": "+0123456789",
            "destinationContext": null,
            "destinationName": "United States",
            "conferenceId": null,
            "licenseCapability": "MCOPSTNU",
            "inventoryType": "Subscriber",
            "operator": "Microsoft",
            "callDurationSource": "microsoft"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a><span data-ttu-id="8677c-149">См. также</span><span class="sxs-lookup"><span data-stu-id="8677c-149">See also</span></span>

* [<span data-ttu-id="8677c-150">Отчет об использовании microsoft Teams PSTN</span><span class="sxs-lookup"><span data-stu-id="8677c-150">Microsoft Teams PSTN usage report</span></span>](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [<span data-ttu-id="8677c-151">Отчет о прямой маршрутике в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8677c-151">Direct routing report in Microsoft Graph</span></span>](callrecords-callrecord-getdirectroutingcalls.md)
