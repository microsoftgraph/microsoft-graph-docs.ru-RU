---
title: 'callRecord: getPstnCalls'
description: Получите журнал вызовов STN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6aa3c85c25373ecee98894ce0704b35a6de25cdb
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872914"
---
# <a name="callrecord-getpstncalls"></a><span data-ttu-id="9ed0f-103">callRecord: getPstnCalls</span><span class="sxs-lookup"><span data-stu-id="9ed0f-103">callRecord: getPstnCalls</span></span>

<span data-ttu-id="9ed0f-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="9ed0f-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed0f-105">Получите журнал вызовов STN как коллекцию записей [pstnCallLogRow.](../resources/callrecords-pstncalllogrow.md)</span><span class="sxs-lookup"><span data-stu-id="9ed0f-105">Get log of PSTN calls as a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed0f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed0f-106">Permissions</span></span>

<span data-ttu-id="9ed0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ed0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ed0f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed0f-109">Permission type</span></span>|<span data-ttu-id="9ed0f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ed0f-110">Permissions (from least to most privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ed0f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ed0f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ed0f-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-112">Not supported.</span></span> |
| <span data-ttu-id="9ed0f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ed0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed0f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-114">Not supported.</span></span> |
| <span data-ttu-id="9ed0f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ed0f-115">Application</span></span>                            | <span data-ttu-id="9ed0f-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ed0f-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ed0f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ed0f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a><span data-ttu-id="9ed0f-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="9ed0f-118">Function parameters</span></span>

<span data-ttu-id="9ed0f-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9ed0f-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9ed0f-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="9ed0f-121">Parameter</span></span>|<span data-ttu-id="9ed0f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9ed0f-122">Type</span></span>|<span data-ttu-id="9ed0f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9ed0f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ed0f-124">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed0f-124">fromDateTime</span></span>|<span data-ttu-id="9ed0f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed0f-125">DateTimeOffset</span></span>|<span data-ttu-id="9ed0f-126">Начало диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-126">Start of time range to query.</span></span> <span data-ttu-id="9ed0f-127">UTC включительно.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-127">UTC, inclusive.</span></span><br/><span data-ttu-id="9ed0f-128">Диапазон времени зависит от времени начала вызова.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-128">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="9ed0f-129">toDateTime</span><span class="sxs-lookup"><span data-stu-id="9ed0f-129">toDateTime</span></span>|<span data-ttu-id="9ed0f-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ed0f-130">DateTimeOffset</span></span>|<span data-ttu-id="9ed0f-131">Конец диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-131">End of time range to query.</span></span> <span data-ttu-id="9ed0f-132">UTC включительно.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-132">UTC, inclusive.</span></span>|

> [!IMPORTANT]
> <span data-ttu-id="9ed0f-133">Значения **fromDateTime** и **toDateTime** не могут быть больше даты в диапазоне 90 дней.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-133">The **fromDateTime** and **toDateTime** values cannot be more than a date range of 90 days.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ed0f-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ed0f-134">Request headers</span></span>

|<span data-ttu-id="9ed0f-135">Имя</span><span class="sxs-lookup"><span data-stu-id="9ed0f-135">Name</span></span>|<span data-ttu-id="9ed0f-136">Описание</span><span class="sxs-lookup"><span data-stu-id="9ed0f-136">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9ed0f-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ed0f-137">Authorization</span></span>|<span data-ttu-id="9ed0f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-p105">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="9ed0f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ed0f-140">Response</span></span>

<span data-ttu-id="9ed0f-141">В случае успеха эта функция возвращает код отклика и коллекцию записей `200 OK` [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-141">If successful, this function returns a `200 OK` response code and a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="9ed0f-142">Если в диапазоне дат содержится более 1000 записей, тело также содержит URL-адрес для запроса следующей страницы `@odata.NextLink` записей вызовов.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-142">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="9ed0f-143">Последняя страница в диапазоне дат не имеет `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="9ed0f-143">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="9ed0f-144">Дополнительные сведения см. в [разгонах данных Microsoft Graph в приложении.](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="9ed0f-144">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="9ed0f-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ed0f-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ed0f-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ed0f-146">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="9ed0f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ed0f-147">Response</span></span>

<span data-ttu-id="9ed0f-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ed0f-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "inventoryType": "Subscriber"
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(from=2019-11-01,to=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a><span data-ttu-id="9ed0f-149">См. также</span><span class="sxs-lookup"><span data-stu-id="9ed0f-149">See also</span></span>

* [<span data-ttu-id="9ed0f-150">Отчет об использовании STN Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9ed0f-150">Microsoft Teams PSTN usage report</span></span>](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [<span data-ttu-id="9ed0f-151">Отчет о прямой маршрутике в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9ed0f-151">Direct routing report in Microsoft Graph</span></span>](callrecords-callrecord-getdirectroutingcalls.md)
