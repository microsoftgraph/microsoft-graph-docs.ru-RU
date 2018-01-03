# <a name="list-events"></a><span data-ttu-id="481ca-101">Список событий</span><span class="sxs-lookup"><span data-stu-id="481ca-101">List events</span></span>

<span data-ttu-id="481ca-p101">Получение списка событий в календаре.  Этот список содержит собрания с одним экземпляром и образцы рядов.</span><span class="sxs-lookup"><span data-stu-id="481ca-p101">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="481ca-104">Чтобы получить расширенные экземпляры события, вы можете [получить представление календаря](calendar_list_calendarview.md) или [экземпляры события](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="481ca-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="481ca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="481ca-105">Permissions</span></span>
<span data-ttu-id="481ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="481ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="481ca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="481ca-108">Permission type</span></span>      | <span data-ttu-id="481ca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="481ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="481ca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="481ca-110">Delegated (work or school account)</span></span> | <span data-ttu-id="481ca-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="481ca-111">Calendars.Read</span></span>    |
|<span data-ttu-id="481ca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="481ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="481ca-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="481ca-113">Calendars.Read</span></span>    |
|<span data-ttu-id="481ca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="481ca-114">Application</span></span> | <span data-ttu-id="481ca-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="481ca-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="481ca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="481ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="481ca-117">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="481ca-117">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events
GET /groups/{id}/calendar/events
```
<span data-ttu-id="481ca-118">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="481ca-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendarGroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="481ca-119">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="481ca-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="481ca-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="481ca-120">Optional query parameters</span></span>
<span data-ttu-id="481ca-121">Этот метод поддерживает [параметры запросов OData]((http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters)) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="481ca-121">This method supports the [OData Query Parameters]((http://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="481ca-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="481ca-122">Request headers</span></span>
| <span data-ttu-id="481ca-123">Имя</span><span class="sxs-lookup"><span data-stu-id="481ca-123">Name</span></span>       | <span data-ttu-id="481ca-124">Тип</span><span class="sxs-lookup"><span data-stu-id="481ca-124">Type</span></span> | <span data-ttu-id="481ca-125">Описание</span><span class="sxs-lookup"><span data-stu-id="481ca-125">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="481ca-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="481ca-126">Authorization</span></span>  | <span data-ttu-id="481ca-127">string</span><span class="sxs-lookup"><span data-stu-id="481ca-127">string</span></span> | <span data-ttu-id="481ca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="481ca-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="481ca-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="481ca-130">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="481ca-131">string</span><span class="sxs-lookup"><span data-stu-id="481ca-131">string</span></span> | <span data-ttu-id="481ca-132">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в отклике.</span><span class="sxs-lookup"><span data-stu-id="481ca-132">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> <span data-ttu-id="481ca-133">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="481ca-133">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="481ca-134">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="481ca-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="481ca-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="481ca-135">Request body</span></span>
<span data-ttu-id="481ca-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="481ca-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="481ca-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="481ca-137">Response</span></span>

<span data-ttu-id="481ca-138">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="481ca-138">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="481ca-139">Пример</span><span class="sxs-lookup"><span data-stu-id="481ca-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="481ca-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="481ca-140">Request</span></span>
<span data-ttu-id="481ca-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="481ca-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendar/events
```
##### <a name="response"></a><span data-ttu-id="481ca-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="481ca-142">Response</span></span>
<span data-ttu-id="481ca-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="481ca-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
