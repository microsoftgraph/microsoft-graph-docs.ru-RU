---
title: 'Каллрекорд: Жетпстнкаллс'
description: Получение журнала звонков PSTN.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 598c3c4fe8abd1b1dcc77cea1d2f513b439771a3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601106"
---
# <a name="callrecord-getpstncalls"></a><span data-ttu-id="dd511-103">Каллрекорд: Жетпстнкаллс</span><span class="sxs-lookup"><span data-stu-id="dd511-103">callRecord: getPstnCalls</span></span>

<span data-ttu-id="dd511-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="dd511-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd511-105">Получение журнала вызовов PSTN в виде коллекции записей [пстнкалллогров](../resources/callrecords-pstncalllogrow.md) .</span><span class="sxs-lookup"><span data-stu-id="dd511-105">Get log of PSTN calls as a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd511-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd511-106">Permissions</span></span>

<span data-ttu-id="dd511-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd511-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd511-109">Permission type</span></span>|<span data-ttu-id="dd511-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd511-110">Permissions (from most to least privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd511-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd511-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd511-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd511-112">Not supported.</span></span> |
| <span data-ttu-id="dd511-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd511-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd511-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd511-114">Not supported.</span></span> |
| <span data-ttu-id="dd511-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd511-115">Application</span></span>                            | <span data-ttu-id="dd511-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd511-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd511-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd511-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getPstnCalls
```

## <a name="function-parameters"></a><span data-ttu-id="dd511-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="dd511-118">Function parameters</span></span>

<span data-ttu-id="dd511-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="dd511-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="dd511-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="dd511-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="dd511-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="dd511-121">Parameter</span></span>|<span data-ttu-id="dd511-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dd511-122">Type</span></span>|<span data-ttu-id="dd511-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dd511-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd511-124">фромдатетиме</span><span class="sxs-lookup"><span data-stu-id="dd511-124">fromDateTime</span></span>|<span data-ttu-id="dd511-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd511-125">DateTimeOffset</span></span>|<span data-ttu-id="dd511-126">Начало диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="dd511-126">Start of time range to query.</span></span> <span data-ttu-id="dd511-127">UTC, включительно.</span><span class="sxs-lookup"><span data-stu-id="dd511-127">UTC, inclusive.</span></span><br/><span data-ttu-id="dd511-128">Диапазон времени основан на времени начала вызова.</span><span class="sxs-lookup"><span data-stu-id="dd511-128">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="dd511-129">тодатетиме</span><span class="sxs-lookup"><span data-stu-id="dd511-129">toDateTime</span></span>|<span data-ttu-id="dd511-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd511-130">DateTimeOffset</span></span>|<span data-ttu-id="dd511-131">Конец диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="dd511-131">End of time range to query.</span></span> <span data-ttu-id="dd511-132">UTC, включительно.</span><span class="sxs-lookup"><span data-stu-id="dd511-132">UTC, inclusive.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="dd511-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd511-133">Request headers</span></span>

|<span data-ttu-id="dd511-134">Имя</span><span class="sxs-lookup"><span data-stu-id="dd511-134">Name</span></span>|<span data-ttu-id="dd511-135">Описание</span><span class="sxs-lookup"><span data-stu-id="dd511-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dd511-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd511-136">Authorization</span></span>|<span data-ttu-id="dd511-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd511-p105">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="dd511-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd511-139">Response</span></span>

<span data-ttu-id="dd511-140">В случае успешного выполнения эта функция возвращает `200 OK` код отклика и коллекцию записей [пстнкалллогров](../resources/callrecords-pstncalllogrow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd511-140">If successful, this function returns a `200 OK` response code and a collection of [pstnCallLogRow](../resources/callrecords-pstncalllogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="dd511-141">Если в диапазоне дат больше 1000 записей, в тексте также включается `@odata.NextLink` URL-адрес для запроса следующей страницы записей вызова.</span><span class="sxs-lookup"><span data-stu-id="dd511-141">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="dd511-142">Последняя страница в диапазоне дат не имеет значения `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="dd511-142">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="dd511-143">Дополнительные сведения см в разделе [разбиение данных Microsoft Graph в приложении](/graph/paging).</span><span class="sxs-lookup"><span data-stu-id="dd511-143">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="dd511-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="dd511-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd511-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd511-145">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getpstncalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getPstnCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="dd511-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd511-146">Response</span></span>

<span data-ttu-id="dd511-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dd511-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dd511-148">См. также</span><span class="sxs-lookup"><span data-stu-id="dd511-148">See also</span></span>

* [<span data-ttu-id="dd511-149">Отчет об использовании Microsoft Teams PSTN</span><span class="sxs-lookup"><span data-stu-id="dd511-149">Microsoft Teams PSTN usage report</span></span>](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
* [<span data-ttu-id="dd511-150">Отчет о прямой маршрутизации в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="dd511-150">Direct routing report in Microsoft Graph</span></span>](callrecords-callrecord-getdirectroutingcalls.md)