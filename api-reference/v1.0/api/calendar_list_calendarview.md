# <a name="list-calendarview"></a><span data-ttu-id="da792-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="da792-101">List calendarView</span></span>

<span data-ttu-id="da792-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря `(../me/calendarview)`, принадлежащего пользователю или группе, либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="da792-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da792-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="da792-103">Prerequisites</span></span>
<span data-ttu-id="da792-104">Для применения этого API требуется одна из таких **областей**:</span><span class="sxs-lookup"><span data-stu-id="da792-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="da792-105">События в календаре пользователя: _Calendars.Read_ или _Calendars.ReadWrite_.</span><span class="sxs-lookup"><span data-stu-id="da792-105">Events in a user's calendar: _Calendars.Read_ or _Calendars.ReadWrite_</span></span>
* <span data-ttu-id="da792-106">События в календаре группы: _Group.Read.All_ или _Group.ReadWrite.All_.</span><span class="sxs-lookup"><span data-stu-id="da792-106">Events in a group calendar: _Group.Read.All_ or _Group.ReadWrite.All_</span></span>

## <a name="http-request"></a><span data-ttu-id="da792-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da792-107">HTTP request</span></span>

<span data-ttu-id="da792-108">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="da792-108">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="da792-109">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="da792-109">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="da792-110">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="da792-110">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="da792-111">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="da792-111">Query parameters</span></span>

<span data-ttu-id="da792-112">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="da792-112">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="da792-113">Параметр</span><span class="sxs-lookup"><span data-stu-id="da792-113">Parameter</span></span>    | <span data-ttu-id="da792-114">Тип</span><span class="sxs-lookup"><span data-stu-id="da792-114">Type</span></span>   |<span data-ttu-id="da792-115">Описание</span><span class="sxs-lookup"><span data-stu-id="da792-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da792-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da792-116">startDateTime</span></span>|<span data-ttu-id="da792-117">String</span><span class="sxs-lookup"><span data-stu-id="da792-117">String</span></span>|<span data-ttu-id="da792-p101">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="da792-p101">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="da792-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="da792-120">endDateTime</span></span>|<span data-ttu-id="da792-121">String</span><span class="sxs-lookup"><span data-stu-id="da792-121">String</span></span>|<span data-ttu-id="da792-p102">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="da792-p102">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="da792-124">Этот метод также поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="da792-124">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da792-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da792-125">Request headers</span></span>
| <span data-ttu-id="da792-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da792-126">Header</span></span>       | <span data-ttu-id="da792-127">Значение</span><span class="sxs-lookup"><span data-stu-id="da792-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da792-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da792-128">Authorization</span></span>  | <span data-ttu-id="da792-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da792-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da792-131">Prefer</span><span class="sxs-lookup"><span data-stu-id="da792-131">Prefer</span></span>  | <span data-ttu-id="da792-p104">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="da792-p104">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da792-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="da792-136">Request body</span></span>
<span data-ttu-id="da792-137">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da792-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da792-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="da792-138">Response</span></span>

<span data-ttu-id="da792-139">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="da792-139">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da792-140">Пример</span><span class="sxs-lookup"><span data-stu-id="da792-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da792-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="da792-141">Request</span></span>
<span data-ttu-id="da792-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da792-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="da792-143">Ответ</span><span class="sxs-lookup"><span data-stu-id="da792-143">Response</span></span>
<span data-ttu-id="da792-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="da792-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
