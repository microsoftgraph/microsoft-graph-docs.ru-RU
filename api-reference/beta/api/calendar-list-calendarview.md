---
title: Список calendarView
description: Получите вхождения, исключений и отдельные экземпляры событий в календарном представлении определенный временной интервал,
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b360d47c99de387daf5b421623f926ad7912b912
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520895"
---
# <a name="list-calendarview"></a><span data-ttu-id="e4611-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="e4611-103">List calendarView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4611-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря `(../me/calendarview)`, принадлежащего пользователю или группе, либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="e4611-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4611-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4611-105">Permissions</span></span>
<span data-ttu-id="e4611-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="e4611-108">События в календаре пользователя: Calendars.Read или Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="e4611-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="e4611-109">События в календаре группы: Group.Read.All или Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="e4611-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e4611-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4611-110">HTTP request</span></span>
<span data-ttu-id="e4611-111"><!-- { "blockType": "ignored" } -->Пользователя или группы по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="e4611-111"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="e4611-112">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="e4611-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="e4611-113">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="e4611-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="e4611-114">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="e4611-114">Query parameters</span></span>

<span data-ttu-id="e4611-115">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="e4611-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="e4611-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="e4611-116">Parameter</span></span>    | <span data-ttu-id="e4611-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e4611-117">Type</span></span>   |<span data-ttu-id="e4611-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e4611-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4611-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e4611-119">startDateTime</span></span>|<span data-ttu-id="e4611-120">String</span><span class="sxs-lookup"><span data-stu-id="e4611-120">String</span></span>|<span data-ttu-id="e4611-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e4611-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="e4611-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e4611-123">endDateTime</span></span>|<span data-ttu-id="e4611-124">String</span><span class="sxs-lookup"><span data-stu-id="e4611-124">String</span></span>|<span data-ttu-id="e4611-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="e4611-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="e4611-127">Этот метод также поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e4611-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e4611-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4611-128">Request headers</span></span>
| <span data-ttu-id="e4611-129">Имя</span><span class="sxs-lookup"><span data-stu-id="e4611-129">Name</span></span>       | <span data-ttu-id="e4611-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e4611-130">Type</span></span> | <span data-ttu-id="e4611-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e4611-131">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="e4611-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4611-132">Authorization</span></span>  | <span data-ttu-id="e4611-133">string</span><span class="sxs-lookup"><span data-stu-id="e4611-133">string</span></span> | <span data-ttu-id="e4611-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4611-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4611-136">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="e4611-136">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="e4611-137">string</span><span class="sxs-lookup"><span data-stu-id="e4611-137">string</span></span> | <span data-ttu-id="e4611-138">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="e4611-138">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="e4611-139">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e4611-139">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="e4611-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e4611-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4611-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4611-141">Request body</span></span>
<span data-ttu-id="e4611-142">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4611-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4611-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4611-143">Response</span></span>

<span data-ttu-id="e4611-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e4611-144">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4611-145">Пример</span><span class="sxs-lookup"><span data-stu-id="e4611-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4611-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4611-146">Request</span></span>
<span data-ttu-id="e4611-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4611-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="e4611-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4611-148">Response</span></span>
<span data-ttu-id="e4611-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e4611-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-list-calendarview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
