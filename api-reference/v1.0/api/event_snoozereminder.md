# <a name="event-snoozereminder"></a><span data-ttu-id="5f11c-101">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="5f11c-101">event: snoozeReminder</span></span>

<span data-ttu-id="5f11c-102">Указание другого времени для откладывания напоминания.</span><span class="sxs-lookup"><span data-stu-id="5f11c-102">Postpone a reminder until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f11c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f11c-103">Permissions</span></span>
<span data-ttu-id="5f11c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5f11c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f11c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f11c-106">Permission type</span></span>      | <span data-ttu-id="5f11c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f11c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f11c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f11c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5f11c-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f11c-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f11c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f11c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f11c-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f11c-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5f11c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f11c-112">Application</span></span> | <span data-ttu-id="5f11c-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f11c-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f11c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f11c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder
POST /groups/{id}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder
POST /groups/{id}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="5f11c-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f11c-115">Request headers</span></span>
| <span data-ttu-id="5f11c-116">Имя</span><span class="sxs-lookup"><span data-stu-id="5f11c-116">Name</span></span>       | <span data-ttu-id="5f11c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="5f11c-117">Type</span></span> | <span data-ttu-id="5f11c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5f11c-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f11c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f11c-119">Authorization</span></span>  | <span data-ttu-id="5f11c-120">string</span><span class="sxs-lookup"><span data-stu-id="5f11c-120">string</span></span>  | <span data-ttu-id="5f11c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f11c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f11c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f11c-123">Content-Type</span></span> | <span data-ttu-id="5f11c-124">string</span><span class="sxs-lookup"><span data-stu-id="5f11c-124">string</span></span>  | <span data-ttu-id="5f11c-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f11c-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f11c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f11c-127">Request body</span></span>
<span data-ttu-id="5f11c-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5f11c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f11c-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="5f11c-129">Parameter</span></span>    | <span data-ttu-id="5f11c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5f11c-130">Type</span></span>   |<span data-ttu-id="5f11c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5f11c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f11c-132">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="5f11c-132">newReminderTime</span></span>|<span data-ttu-id="5f11c-133">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="5f11c-133">DateTimeTimeZone</span></span>|<span data-ttu-id="5f11c-134">Новые дата и время для активации напоминания.</span><span class="sxs-lookup"><span data-stu-id="5f11c-134">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="5f11c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f11c-135">Response</span></span>

<span data-ttu-id="5f11c-p104">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5f11c-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f11c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5f11c-138">Example</span></span>
<span data-ttu-id="5f11c-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="5f11c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5f11c-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f11c-140">Request</span></span>
<span data-ttu-id="5f11c-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f11c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="5f11c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f11c-142">Response</span></span>
<span data-ttu-id="5f11c-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5f11c-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
