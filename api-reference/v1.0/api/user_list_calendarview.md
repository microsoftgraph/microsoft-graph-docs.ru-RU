# <a name="list-calendarview"></a><span data-ttu-id="f0ecf-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="f0ecf-101">List calendarView</span></span>

<span data-ttu-id="f0ecf-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0ecf-103">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0ecf-103">Prerequisites</span></span>
<span data-ttu-id="f0ecf-104">Для применения этого API требуется одна из указанных **областей**: *Calendars.Read; Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="f0ecf-104">One of the following scopes is required to execute this API: Calendars.Read; Calendars.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="f0ecf-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0ecf-105">HTTP request</span></span>

<span data-ttu-id="f0ecf-106">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-106">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="f0ecf-107">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f0ecf-107">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="f0ecf-108">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f0ecf-108">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="f0ecf-109">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="f0ecf-109">Query parameters</span></span>

<span data-ttu-id="f0ecf-110">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-110">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="f0ecf-111">Параметр</span><span class="sxs-lookup"><span data-stu-id="f0ecf-111">Parameter</span></span>    | <span data-ttu-id="f0ecf-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f0ecf-112">Type</span></span>   |<span data-ttu-id="f0ecf-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f0ecf-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0ecf-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f0ecf-114">startDateTime</span></span>|<span data-ttu-id="f0ecf-115">String</span><span class="sxs-lookup"><span data-stu-id="f0ecf-115">String</span></span>|<span data-ttu-id="f0ecf-p101">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="f0ecf-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f0ecf-118">endDateTime</span></span>|<span data-ttu-id="f0ecf-119">String</span><span class="sxs-lookup"><span data-stu-id="f0ecf-119">String</span></span>|<span data-ttu-id="f0ecf-p102">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="f0ecf-122">Этот метод также поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-122">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0ecf-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0ecf-123">Request headers</span></span>
| <span data-ttu-id="f0ecf-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f0ecf-124">Name</span></span>       | <span data-ttu-id="f0ecf-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f0ecf-125">Type</span></span> | <span data-ttu-id="f0ecf-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f0ecf-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f0ecf-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0ecf-127">Authorization</span></span>  | <span data-ttu-id="f0ecf-128">string</span><span class="sxs-lookup"><span data-stu-id="f0ecf-128">string</span></span>  | <span data-ttu-id="f0ecf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0ecf-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0ecf-131">Content-Type</span></span>   | <span data-ttu-id="f0ecf-132">string</span><span class="sxs-lookup"><span data-stu-id="f0ecf-132">string</span></span>  | <span data-ttu-id="f0ecf-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f0ecf-133">application/json</span></span> | 
| <span data-ttu-id="f0ecf-134">Предпочтительно</span><span class="sxs-lookup"><span data-stu-id="f0ecf-134">Prefer</span></span> | <span data-ttu-id="f0ecf-135">string</span><span class="sxs-lookup"><span data-stu-id="f0ecf-135">string</span></span> | <span data-ttu-id="f0ecf-p104">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0ecf-140">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0ecf-140">Request body</span></span>
<span data-ttu-id="f0ecf-141">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0ecf-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0ecf-142">Response</span></span>

<span data-ttu-id="f0ecf-143">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-143">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0ecf-144">Пример</span><span class="sxs-lookup"><span data-stu-id="f0ecf-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0ecf-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0ecf-145">Request</span></span>
<span data-ttu-id="f0ecf-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="f0ecf-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0ecf-147">Response</span></span>
<span data-ttu-id="f0ecf-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f0ecf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
        "response": "",
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
  "tocPath": ""
}-->
