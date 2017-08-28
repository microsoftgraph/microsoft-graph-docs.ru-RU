# <a name="create-event"></a><span data-ttu-id="26e75-101">Создание объекта Event</span><span class="sxs-lookup"><span data-stu-id="26e75-101">Create Event</span></span>

<span data-ttu-id="26e75-102">С помощью этого API можно создать объект Event в календаре по умолчанию или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="26e75-102">Use this API to create a new Event in the default or the specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="26e75-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26e75-103">Permissions</span></span>
<span data-ttu-id="26e75-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26e75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26e75-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e75-106">Permission type</span></span>      | <span data-ttu-id="26e75-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e75-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26e75-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e75-108">Delegated (work or school account)</span></span> | <span data-ttu-id="26e75-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e75-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26e75-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e75-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26e75-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e75-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="26e75-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26e75-112">Application</span></span> | <span data-ttu-id="26e75-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26e75-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26e75-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e75-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="26e75-115">[Календарь](../resources/calendar.md) пользователя или группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="26e75-115">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="26e75-116">Экземпляр [calendar](../resources/calendar.md) пользователя в экземпляре по умолчанию [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="26e75-116">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="26e75-117">[Календарь](../resources/calendar.md) пользователя в определенной группе [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="26e75-117">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="26e75-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26e75-118">Request headers</span></span>
| <span data-ttu-id="26e75-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26e75-119">Header</span></span>       | <span data-ttu-id="26e75-120">Значение</span><span class="sxs-lookup"><span data-stu-id="26e75-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26e75-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26e75-121">Authorization</span></span>  | <span data-ttu-id="26e75-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e75-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="26e75-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26e75-124">Content-Type</span></span>  | <span data-ttu-id="26e75-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26e75-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26e75-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26e75-127">Request body</span></span>
<span data-ttu-id="26e75-128">Предоставьте в тексте запроса описание объекта [Event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26e75-128">In the request body, supply a JSON representation of [Event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="26e75-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e75-129">Response</span></span>

<span data-ttu-id="26e75-130">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Event](../resources/event.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="26e75-130">If successful, this method returns `201, Created` response code and [Event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26e75-131">Пример</span><span class="sxs-lookup"><span data-stu-id="26e75-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26e75-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e75-132">Request</span></span>
<span data-ttu-id="26e75-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26e75-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/events
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
<span data-ttu-id="26e75-134">Предоставьте в тексте запроса описание объекта [event](../resources/event.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26e75-134">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="26e75-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="26e75-135">Response</span></span>
<span data-ttu-id="26e75-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="26e75-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
