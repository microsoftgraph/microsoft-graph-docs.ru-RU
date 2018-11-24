# <a name="list-calendarview"></a><span data-ttu-id="775dc-101">Список calendarView</span><span class="sxs-lookup"><span data-stu-id="775dc-101">List calendarView</span></span>

<span data-ttu-id="775dc-102">Получение исключений, повторяемых или единичных экземпляров событий в таком представлении стандартного либо другого календаря пользователя, которое определяется заданным диапазоном времени.</span><span class="sxs-lookup"><span data-stu-id="775dc-102">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's default calendar, or from some other calendar of the user's.</span></span>
## <a name="permissions"></a><span data-ttu-id="775dc-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="775dc-103">Permissions</span></span>
<span data-ttu-id="775dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="775dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="775dc-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="775dc-106">Permission type</span></span>      | <span data-ttu-id="775dc-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="775dc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="775dc-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="775dc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="775dc-109">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="775dc-109">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="775dc-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="775dc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="775dc-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="775dc-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="775dc-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="775dc-112">Application</span></span> | <span data-ttu-id="775dc-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="775dc-113">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="775dc-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="775dc-114">HTTP request</span></span>

<span data-ttu-id="775dc-115">Экземпляр [calendar](../resources/calendar.md) по умолчанию для пользователя.</span><span class="sxs-lookup"><span data-stu-id="775dc-115">A user's default [calendar](../resources/calendar.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="775dc-116">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="775dc-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="775dc-117">[Календарь](../resources/calendar.md) в определенном объекте [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="775dc-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a><span data-ttu-id="775dc-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="775dc-118">Query parameters</span></span>

<span data-ttu-id="775dc-119">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="775dc-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="775dc-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="775dc-120">Parameter</span></span>    | <span data-ttu-id="775dc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="775dc-121">Type</span></span>   |<span data-ttu-id="775dc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="775dc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="775dc-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="775dc-123">startDateTime</span></span>|<span data-ttu-id="775dc-124">String</span><span class="sxs-lookup"><span data-stu-id="775dc-124">String</span></span>|<span data-ttu-id="775dc-p102">Дата и время начала диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="775dc-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="775dc-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="775dc-127">endDateTime</span></span>|<span data-ttu-id="775dc-128">String</span><span class="sxs-lookup"><span data-stu-id="775dc-128">String</span></span>|<span data-ttu-id="775dc-p103">Дата и время окончания диапазона, представленные в формате ISO 8601. Пример: "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="775dc-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="775dc-131">Этот метод также поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="775dc-131">This method also supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="775dc-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="775dc-132">Request headers</span></span>
| <span data-ttu-id="775dc-133">Имя</span><span class="sxs-lookup"><span data-stu-id="775dc-133">Name</span></span>       | <span data-ttu-id="775dc-134">Тип</span><span class="sxs-lookup"><span data-stu-id="775dc-134">Type</span></span> | <span data-ttu-id="775dc-135">Описание</span><span class="sxs-lookup"><span data-stu-id="775dc-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="775dc-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="775dc-136">Authorization</span></span>  | <span data-ttu-id="775dc-137">string</span><span class="sxs-lookup"><span data-stu-id="775dc-137">string</span></span> | <span data-ttu-id="775dc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="775dc-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="775dc-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="775dc-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="775dc-141">string</span><span class="sxs-lookup"><span data-stu-id="775dc-141">string</span></span> | <span data-ttu-id="775dc-142">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="775dc-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="775dc-143">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="775dc-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="775dc-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="775dc-144">Optional.</span></span> |
| <span data-ttu-id="775dc-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="775dc-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="775dc-146">string</span><span class="sxs-lookup"><span data-stu-id="775dc-146">string</span></span> | <span data-ttu-id="775dc-147">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="775dc-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="775dc-148">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="775dc-148">Values can be "text" or "html".</span></span> <span data-ttu-id="775dc-149">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="775dc-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="775dc-150">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="775dc-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="775dc-151">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="775dc-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="775dc-152">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="775dc-152">Request body</span></span>
<span data-ttu-id="775dc-153">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="775dc-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="775dc-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="775dc-154">Response</span></span>

<span data-ttu-id="775dc-155">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="775dc-155">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="775dc-156">Пример</span><span class="sxs-lookup"><span data-stu-id="775dc-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="775dc-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="775dc-157">Request</span></span>
<span data-ttu-id="775dc-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="775dc-158">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a><span data-ttu-id="775dc-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="775dc-159">Response</span></span>
<span data-ttu-id="775dc-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="775dc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
