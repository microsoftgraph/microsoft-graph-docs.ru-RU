# <a name="event-dismissreminder"></a><span data-ttu-id="4febc-101">event: dismissReminder</span><span class="sxs-lookup"><span data-stu-id="4febc-101">event: dismissReminder</span></span>

<span data-ttu-id="4febc-102">Отключить напоминание, которое было активировано для [события](../resources/event.md) в [календаре](../resources/calendar.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="4febc-102">Dismiss a reminder that has been triggered for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4febc-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4febc-103">Permissions</span></span>
<span data-ttu-id="4febc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4febc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4febc-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4febc-106">Permission type</span></span>      | <span data-ttu-id="4febc-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4febc-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4febc-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4febc-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4febc-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4febc-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4febc-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4febc-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4febc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4febc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="4febc-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4febc-112">Application</span></span> | <span data-ttu-id="4febc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4febc-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4febc-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4febc-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/events/{id}/dismissReminder

POST /me/calendar/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder

POST /me/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroup/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="4febc-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4febc-115">Request headers</span></span>
| <span data-ttu-id="4febc-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4febc-116">Name</span></span>       | <span data-ttu-id="4febc-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4febc-117">Type</span></span> | <span data-ttu-id="4febc-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4febc-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4febc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4febc-119">Authorization</span></span>  | <span data-ttu-id="4febc-120">string</span><span class="sxs-lookup"><span data-stu-id="4febc-120">string</span></span>  | <span data-ttu-id="4febc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4febc-p102">Bearer {token}. Required.</span></span> |

<br/>

## <a name="response"></a><span data-ttu-id="4febc-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="4febc-123">Response</span></span>

<span data-ttu-id="4febc-p103">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4febc-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4febc-126">Пример</span><span class="sxs-lookup"><span data-stu-id="4febc-126">Example</span></span>

<span data-ttu-id="4febc-127">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4febc-127">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4febc-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4febc-128">Request</span></span>
<span data-ttu-id="4febc-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4febc-129">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/dismissReminder
```

<br/>

### <a name="response"></a><span data-ttu-id="4febc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4febc-130">Response</span></span>
<span data-ttu-id="4febc-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4febc-131">Here is an example of the response.</span></span>

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
  "description": "event: dismissReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
