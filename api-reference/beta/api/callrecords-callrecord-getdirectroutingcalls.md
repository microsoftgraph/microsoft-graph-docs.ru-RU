---
title: 'callRecord: getDirectRoutingCalls'
description: Получите журнал прямых вызовов маршрутов.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5dd389ddba5e3f081b850e2303833b47b832e7d7
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872921"
---
# <a name="callrecord-getdirectroutingcalls"></a><span data-ttu-id="19444-103">callRecord: getDirectRoutingCalls</span><span class="sxs-lookup"><span data-stu-id="19444-103">callRecord: getDirectRoutingCalls</span></span>

<span data-ttu-id="19444-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="19444-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19444-105">Получите журнал прямых вызовов маршрутизирования в качестве коллекции [записей directRoutingLogRow.](../resources/callrecords-directroutinglogrow.md)</span><span class="sxs-lookup"><span data-stu-id="19444-105">Get a log of direct routing calls as a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries.</span></span>

## <a name="permissions"></a><span data-ttu-id="19444-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="19444-106">Permissions</span></span>

<span data-ttu-id="19444-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19444-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19444-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19444-109">Permission type</span></span>|<span data-ttu-id="19444-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="19444-110">Permissions (from least to most privileged)</span></span>|
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19444-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19444-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19444-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19444-112">Not supported.</span></span> |
| <span data-ttu-id="19444-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19444-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19444-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19444-114">Not supported.</span></span> |
| <span data-ttu-id="19444-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="19444-115">Application</span></span>                            | <span data-ttu-id="19444-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="19444-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19444-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19444-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /communications/callRecords/getDirectRoutingCalls
```

## <a name="request-headers"></a><span data-ttu-id="19444-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19444-118">Request headers</span></span>

|<span data-ttu-id="19444-119">Имя</span><span class="sxs-lookup"><span data-stu-id="19444-119">Name</span></span>|<span data-ttu-id="19444-120">Описание</span><span class="sxs-lookup"><span data-stu-id="19444-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="19444-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19444-121">Authorization</span></span>|<span data-ttu-id="19444-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19444-p102">Bearer {token}. Required.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="19444-124">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="19444-124">Function parameters</span></span>

<span data-ttu-id="19444-125">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="19444-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="19444-126">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="19444-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="19444-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="19444-127">Parameter</span></span>|<span data-ttu-id="19444-128">Тип</span><span class="sxs-lookup"><span data-stu-id="19444-128">Type</span></span>|<span data-ttu-id="19444-129">Описание</span><span class="sxs-lookup"><span data-stu-id="19444-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19444-130">fromDateTime</span><span class="sxs-lookup"><span data-stu-id="19444-130">fromDateTime</span></span>|<span data-ttu-id="19444-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19444-131">DateTimeOffset</span></span>|<span data-ttu-id="19444-132">Начало диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="19444-132">Start of time range to query.</span></span> <span data-ttu-id="19444-133">UTC включительно.</span><span class="sxs-lookup"><span data-stu-id="19444-133">UTC, inclusive.</span></span><br/><span data-ttu-id="19444-134">Диапазон времени зависит от времени начала вызова.</span><span class="sxs-lookup"><span data-stu-id="19444-134">Time range is based on the call start time.</span></span>|
|<span data-ttu-id="19444-135">toDateTime</span><span class="sxs-lookup"><span data-stu-id="19444-135">toDateTime</span></span>|<span data-ttu-id="19444-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19444-136">DateTimeOffset</span></span>|<span data-ttu-id="19444-137">Конец диапазона времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="19444-137">End of time range to query.</span></span> <span data-ttu-id="19444-138">UTC включительно.</span><span class="sxs-lookup"><span data-stu-id="19444-138">UTC, inclusive.</span></span>|

## <a name="response"></a><span data-ttu-id="19444-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="19444-139">Response</span></span>

<span data-ttu-id="19444-140">В случае успеха эта функция возвращает код отклика и коллекцию записей `200 OK` [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="19444-140">If successful, this function returns a `200 OK` response code and a collection of [directRoutingLogRow](../resources/callrecords-directroutinglogrow.md) entries in the response body.</span></span>
  
<span data-ttu-id="19444-141">Если в диапазоне дат содержится более 1000 записей, тело также содержит URL-адрес для запроса следующей страницы `@odata.NextLink` записей вызовов.</span><span class="sxs-lookup"><span data-stu-id="19444-141">If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of call entries.</span></span> <span data-ttu-id="19444-142">Последняя страница в диапазоне дат не имеет `@odata.NextLink` .</span><span class="sxs-lookup"><span data-stu-id="19444-142">The last page in the date range does not have `@odata.NextLink`.</span></span> <span data-ttu-id="19444-143">Дополнительные сведения см. в [разгонах данных Microsoft Graph в приложении.](/graph/paging)</span><span class="sxs-lookup"><span data-stu-id="19444-143">For more information, see [paging Microsoft Graph data in your app](/graph/paging).</span></span>

## <a name="examples"></a><span data-ttu-id="19444-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="19444-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19444-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="19444-145">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "callrecord_getdirectroutingcalls"
}
-->

``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)
```

### <a name="response"></a><span data-ttu-id="19444-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="19444-146">Response</span></span>

<span data-ttu-id="19444-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="19444-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "isCollection": true
} 
-->

``` http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.directRoutingLogRow)",
    "@odata.count": 1000,
    "value": [{
            "id": "9e8bba57-dc14-533a-a7dd-f0da6575eed1",
            "correlationId": "c98e1515-a937-4b81-b8a8-3992afde64e0",
            "userId": "db03c14b-06eb-4189-939b-7cbf3a20ba27",
            "userPrincipalName": "richard.malk@contoso.com",
            "userDisplayName": "Richard Malk",
            "startDateTime": "2019-11-01T00:00:25.105Z",
            "inviteDateTime": "2019-11-01T00:00:21.949Z",
            "failureDateTime": "0001-01-01T00:00:00Z",
            "endDateTime": "2019-11-01T00:00:30.105Z",
            "duration": 5,
            "callType": "ByotIn",
            "successfulCall": true,
            "callerNumber": "+12345678**_",
            "calleeNumber": "+01234567_*_",
            "mediaPathLocation": "USWE",
            "signalingLocation": "EUNO",
            "finalSipCode": 0,
            "callEndSubReason": 540000,
            "finalSipCodePhrase": "BYE",
            "trunkFullyQualifiedDomainName": "tll-audiocodes01.adatum.biz",
            "mediaBypassEnabled": false
        }],
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getDirectRoutingCalls(fromDateTime=2019-11-01,toDateTime=2019-12-01)?$skip=1000"
}
```

## <a name="see-also"></a><span data-ttu-id="19444-148">См. также</span><span class="sxs-lookup"><span data-stu-id="19444-148">See also</span></span>

<span data-ttu-id="19444-149">_ [Отчет об использовании прямой маршрутки Microsoft Teams](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) в Центре администрирования Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="19444-149">_ [Microsoft Teams direct routing usage report](/microsoftteams/teams-analytics-and-reports/pstn-usage-report#direct-routing) in the Microsoft Teams admin center</span></span>
* <span data-ttu-id="19444-150">[Панель мониторинга состояния для прямой маршрутки](/MicrosoftTeams/direct-routing-health-dashboard) в Центре администрирования Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="19444-150">[Health Dashboard for direct routing](/MicrosoftTeams/direct-routing-health-dashboard) in the Microsoft Teams admin center</span></span>
* [<span data-ttu-id="19444-151">Отчет о вызовах STN в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="19444-151">PSTN call report in Microsoft Graph</span></span>](callrecords-callrecord-getpstncalls.md)