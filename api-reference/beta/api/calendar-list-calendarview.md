---
title: Список calendarView
description: Получите вхождения, исключений и отдельные экземпляры событий в календарном представлении определенный временной интервал,
localization_priority: Normal
ms.openlocfilehash: e56149b7a3cc89d3e1d4d149a03e409222f65374
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814338"
---
# <a name="list-calendarview"></a><span data-ttu-id="1b972-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="1b972-103">List calendarView</span></span>

> <span data-ttu-id="1b972-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b972-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b972-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b972-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b972-106">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря `(../me/calendarview)`, принадлежащего пользователю или группе, либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="1b972-106">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b972-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b972-107">Permissions</span></span>
<span data-ttu-id="1b972-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b972-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="1b972-110">События в календаре пользователя: Calendars.Read или Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="1b972-110">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="1b972-111">События в календаре группы: Group.Read.All или Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="1b972-111">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="1b972-112">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b972-112">HTTP request</span></span>
<span data-ttu-id="1b972-113"><!-- { "blockType": "ignored" } -->Пользователя или группы по умолчанию [календаря](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="1b972-113"><!-- { "blockType": "ignored" } --> A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="1b972-114">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="1b972-114">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="1b972-115">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="1b972-115">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="1b972-116">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="1b972-116">Query parameters</span></span>

<span data-ttu-id="1b972-117">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1b972-117">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="1b972-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="1b972-118">Parameter</span></span>    | <span data-ttu-id="1b972-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1b972-119">Type</span></span>   |<span data-ttu-id="1b972-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1b972-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b972-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1b972-121">startDateTime</span></span>|<span data-ttu-id="1b972-122">String</span><span class="sxs-lookup"><span data-stu-id="1b972-122">String</span></span>|<span data-ttu-id="1b972-p103">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="1b972-p103">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="1b972-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1b972-125">endDateTime</span></span>|<span data-ttu-id="1b972-126">String</span><span class="sxs-lookup"><span data-stu-id="1b972-126">String</span></span>|<span data-ttu-id="1b972-p104">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="1b972-p104">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="1b972-129">Этот метод также поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1b972-129">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1b972-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b972-130">Request headers</span></span>
| <span data-ttu-id="1b972-131">Имя</span><span class="sxs-lookup"><span data-stu-id="1b972-131">Name</span></span>       | <span data-ttu-id="1b972-132">Тип</span><span class="sxs-lookup"><span data-stu-id="1b972-132">Type</span></span> | <span data-ttu-id="1b972-133">Описание</span><span class="sxs-lookup"><span data-stu-id="1b972-133">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="1b972-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b972-134">Authorization</span></span>  | <span data-ttu-id="1b972-135">string</span><span class="sxs-lookup"><span data-stu-id="1b972-135">string</span></span> | <span data-ttu-id="1b972-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b972-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b972-138">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1b972-138">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="1b972-139">string</span><span class="sxs-lookup"><span data-stu-id="1b972-139">string</span></span> | <span data-ttu-id="1b972-140">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="1b972-140">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="1b972-141">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1b972-141">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="1b972-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1b972-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b972-143">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b972-143">Request body</span></span>
<span data-ttu-id="1b972-144">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b972-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b972-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b972-145">Response</span></span>

<span data-ttu-id="1b972-146">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1b972-146">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b972-147">Пример</span><span class="sxs-lookup"><span data-stu-id="1b972-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b972-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b972-148">Request</span></span>
<span data-ttu-id="1b972-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b972-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="1b972-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b972-150">Response</span></span>
<span data-ttu-id="1b972-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1b972-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
