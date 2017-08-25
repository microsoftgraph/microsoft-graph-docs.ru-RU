# <a name="list-calendarview"></a><span data-ttu-id="550a4-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="550a4-101">List calendarView</span></span>

<span data-ttu-id="550a4-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного календаря `(../me/calendarview)`, принадлежащего пользователю или группе, либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="550a4-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the default calendar `(../me/calendarview)` of a user or group, or some other calendar of the user's.</span></span>

## <a name="permissions"></a><span data-ttu-id="550a4-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="550a4-103">Permissions</span></span>
<span data-ttu-id="550a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="550a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

* <span data-ttu-id="550a4-106">События в календаре пользователя: Calendars.Read или Calendars.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="550a4-106">Events in a user's calendar: Calendars.Read or Calendars.ReadWrite</span></span>
* <span data-ttu-id="550a4-107">События в календаре группы: Group.Read.All или Group.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="550a4-107">Events in a group calendar: Group.Read.All or Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="550a4-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="550a4-108">HTTP request</span></span>

<span data-ttu-id="550a4-109">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550a4-109">A user's or group's default [calendar](../resources/calendar.md).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="550a4-110">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="550a4-110">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="550a4-111">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="550a4-111">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="550a4-112">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="550a4-112">Query parameters</span></span>

<span data-ttu-id="550a4-113">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="550a4-113">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="550a4-114">Параметр</span><span class="sxs-lookup"><span data-stu-id="550a4-114">Parameter</span></span>    | <span data-ttu-id="550a4-115">Тип</span><span class="sxs-lookup"><span data-stu-id="550a4-115">Type</span></span>   |<span data-ttu-id="550a4-116">Описание</span><span class="sxs-lookup"><span data-stu-id="550a4-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="550a4-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="550a4-117">startDateTime</span></span>|<span data-ttu-id="550a4-118">String</span><span class="sxs-lookup"><span data-stu-id="550a4-118">String</span></span>|<span data-ttu-id="550a4-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="550a4-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="550a4-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="550a4-121">endDateTime</span></span>|<span data-ttu-id="550a4-122">String</span><span class="sxs-lookup"><span data-stu-id="550a4-122">String</span></span>|<span data-ttu-id="550a4-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="550a4-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="550a4-125">Этот метод также поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="550a4-125">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="550a4-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="550a4-126">Request headers</span></span>
| <span data-ttu-id="550a4-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="550a4-127">Header</span></span>       | <span data-ttu-id="550a4-128">Значение</span><span class="sxs-lookup"><span data-stu-id="550a4-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="550a4-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="550a4-129">Authorization</span></span>  | <span data-ttu-id="550a4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="550a4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="550a4-132">Prefer</span><span class="sxs-lookup"><span data-stu-id="550a4-132">Prefer</span></span>  | <span data-ttu-id="550a4-p105">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="550a4-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="550a4-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="550a4-137">Request body</span></span>
<span data-ttu-id="550a4-138">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="550a4-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="550a4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="550a4-139">Response</span></span>

<span data-ttu-id="550a4-140">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="550a4-140">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="550a4-141">Пример</span><span class="sxs-lookup"><span data-stu-id="550a4-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="550a4-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="550a4-142">Request</span></span>
<span data-ttu-id="550a4-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="550a4-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00.0000000&endDateTime=2017-01-07T19:00:00.0000000
```
##### <a name="response"></a><span data-ttu-id="550a4-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="550a4-144">Response</span></span>
<span data-ttu-id="550a4-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="550a4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
