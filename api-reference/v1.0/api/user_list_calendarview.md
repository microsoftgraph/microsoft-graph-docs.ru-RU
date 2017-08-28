# <a name="list-calendarview"></a><span data-ttu-id="b5050-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="b5050-101">List calendarView</span></span>

<span data-ttu-id="b5050-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="b5050-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="b5050-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5050-103">Permissions</span></span>
<span data-ttu-id="b5050-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5050-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5050-106">Permission type</span></span>      | <span data-ttu-id="b5050-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5050-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5050-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5050-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b5050-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5050-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b5050-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5050-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5050-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5050-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b5050-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5050-112">Application</span></span> | <span data-ttu-id="b5050-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5050-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5050-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5050-114">HTTP request</span></span>

<span data-ttu-id="b5050-115">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5050-115">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b5050-116">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b5050-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="b5050-117">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="b5050-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="b5050-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="b5050-118">Query parameters</span></span>

<span data-ttu-id="b5050-119">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="b5050-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="b5050-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="b5050-120">Parameter</span></span>    | <span data-ttu-id="b5050-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b5050-121">Type</span></span>   |<span data-ttu-id="b5050-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b5050-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5050-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b5050-123">startDateTime</span></span>|<span data-ttu-id="b5050-124">String</span><span class="sxs-lookup"><span data-stu-id="b5050-124">String</span></span>|<span data-ttu-id="b5050-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="b5050-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="b5050-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b5050-127">endDateTime</span></span>|<span data-ttu-id="b5050-128">String</span><span class="sxs-lookup"><span data-stu-id="b5050-128">String</span></span>|<span data-ttu-id="b5050-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="b5050-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="b5050-131">Этот метод также поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b5050-131">This method also supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5050-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5050-132">Request headers</span></span>
| <span data-ttu-id="b5050-133">Имя</span><span class="sxs-lookup"><span data-stu-id="b5050-133">Name</span></span>       | <span data-ttu-id="b5050-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b5050-134">Type</span></span> | <span data-ttu-id="b5050-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b5050-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b5050-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5050-136">Authorization</span></span>  | <span data-ttu-id="b5050-137">string</span><span class="sxs-lookup"><span data-stu-id="b5050-137">string</span></span>  | <span data-ttu-id="b5050-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5050-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5050-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5050-140">Content-Type</span></span>   | <span data-ttu-id="b5050-141">string</span><span class="sxs-lookup"><span data-stu-id="b5050-141">string</span></span>  | <span data-ttu-id="b5050-142">application/json</span><span class="sxs-lookup"><span data-stu-id="b5050-142">application/json</span></span> |
| <span data-ttu-id="b5050-143">Предпочтительно</span><span class="sxs-lookup"><span data-stu-id="b5050-143">Prefer</span></span> | <span data-ttu-id="b5050-144">string</span><span class="sxs-lookup"><span data-stu-id="b5050-144">string</span></span> | <span data-ttu-id="b5050-p105">outlook.timezone="Стандартное восточное время США". Необязательный. С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе. Если этот заголовок не задан, ответ возвращается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b5050-p105">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5050-149">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b5050-149">Request body</span></span>
<span data-ttu-id="b5050-150">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5050-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5050-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5050-151">Response</span></span>

<span data-ttu-id="b5050-152">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5050-152">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5050-153">Пример</span><span class="sxs-lookup"><span data-stu-id="b5050-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5050-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5050-154">Request</span></span>
<span data-ttu-id="b5050-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5050-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="b5050-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="b5050-156">Response</span></span>
<span data-ttu-id="b5050-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b5050-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
