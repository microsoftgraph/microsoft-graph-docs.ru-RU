---
title: Список calendarView
description: Получение исключений, повторяемых или единичных экземпляров событий в представлении календаря, которое определяется заданным диапазоном времени,
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: eef9e350a2fb6ccb701346cce169eed60be38f31
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443821"
---
# <a name="list-calendarview"></a><span data-ttu-id="b0bcc-103">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="b0bcc-103">List calendarView</span></span>

<span data-ttu-id="b0bcc-104">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря `(../me/calendarview)`, принадлежащего пользователю или группе, либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-104">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0bcc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0bcc-105">Permissions</span></span>
<span data-ttu-id="b0bcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0bcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="b0bcc-108">События в календаре пользователя: Calendars.Read или Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-108">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="b0bcc-109">События в календаре группы: Group.Read.All или Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-109">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b0bcc-110">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0bcc-110">HTTP request</span></span>

<span data-ttu-id="b0bcc-111">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-111">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b0bcc-112">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b0bcc-112">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b0bcc-113">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b0bcc-113">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="b0bcc-114">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b0bcc-114">Query parameters</span></span>

<span data-ttu-id="b0bcc-115">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-115">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="b0bcc-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="b0bcc-116">Parameter</span></span>    | <span data-ttu-id="b0bcc-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b0bcc-117">Type</span></span>   |<span data-ttu-id="b0bcc-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b0bcc-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0bcc-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bcc-119">startDateTime</span></span>|<span data-ttu-id="b0bcc-120">String</span><span class="sxs-lookup"><span data-stu-id="b0bcc-120">String</span></span>|<span data-ttu-id="b0bcc-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="b0bcc-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="b0bcc-123">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b0bcc-123">endDateTime</span></span>|<span data-ttu-id="b0bcc-124">String</span><span class="sxs-lookup"><span data-stu-id="b0bcc-124">String</span></span>|<span data-ttu-id="b0bcc-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="b0bcc-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="b0bcc-127">Этот метод также поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-127">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b0bcc-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0bcc-128">Request headers</span></span>
| <span data-ttu-id="b0bcc-129">Имя</span><span class="sxs-lookup"><span data-stu-id="b0bcc-129">Name</span></span>       | <span data-ttu-id="b0bcc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b0bcc-130">Type</span></span> | <span data-ttu-id="b0bcc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b0bcc-131">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="b0bcc-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0bcc-132">Authorization</span></span>  | <span data-ttu-id="b0bcc-133">string</span><span class="sxs-lookup"><span data-stu-id="b0bcc-133">string</span></span> | <span data-ttu-id="b0bcc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b0bcc-136">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b0bcc-136">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="b0bcc-137">string</span><span class="sxs-lookup"><span data-stu-id="b0bcc-137">string</span></span> | <span data-ttu-id="b0bcc-138">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-138">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="b0bcc-139">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-139">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="b0bcc-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0bcc-141">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b0bcc-141">Request body</span></span>
<span data-ttu-id="b0bcc-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0bcc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0bcc-143">Response</span></span>

<span data-ttu-id="b0bcc-144">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-144">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0bcc-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b0bcc-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0bcc-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0bcc-146">Request</span></span>
<span data-ttu-id="b0bcc-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0bcc-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0bcc-148">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0bcc-149">C#</span><span class="sxs-lookup"><span data-stu-id="b0bcc-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0bcc-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0bcc-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0bcc-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0bcc-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b0bcc-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0bcc-152">Response</span></span>
<span data-ttu-id="b0bcc-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0bcc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
