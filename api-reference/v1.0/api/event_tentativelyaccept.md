# <a name="event-tentativelyaccept"></a><span data-ttu-id="12e49-101">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="12e49-101">event: tentativelyAccept</span></span>

<span data-ttu-id="12e49-102">Предварительное принятие указанного события.</span><span class="sxs-lookup"><span data-stu-id="12e49-102">Tentatively accept the specified event.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12e49-103">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="12e49-103">Prerequisites</span></span>
<span data-ttu-id="12e49-104">Для применения этого API требуется одна из указанных **областей**: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="12e49-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="12e49-105">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12e49-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept
POST /groups/{id}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept
POST /groups/{id}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a><span data-ttu-id="12e49-106">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12e49-106">Request headers</span></span>
| <span data-ttu-id="12e49-107">Имя</span><span class="sxs-lookup"><span data-stu-id="12e49-107">Name</span></span>       | <span data-ttu-id="12e49-108">Тип</span><span class="sxs-lookup"><span data-stu-id="12e49-108">Type</span></span> | <span data-ttu-id="12e49-109">Описание</span><span class="sxs-lookup"><span data-stu-id="12e49-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12e49-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="12e49-110">Authorization</span></span>  | <span data-ttu-id="12e49-111">string</span><span class="sxs-lookup"><span data-stu-id="12e49-111">string</span></span>  | <span data-ttu-id="12e49-p101">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12e49-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="12e49-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="12e49-114">Content-Type</span></span> | <span data-ttu-id="12e49-115">string</span><span class="sxs-lookup"><span data-stu-id="12e49-115">string</span></span>  | <span data-ttu-id="12e49-p102">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12e49-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12e49-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12e49-118">Request body</span></span>
<span data-ttu-id="12e49-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="12e49-119">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="12e49-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="12e49-120">Parameter</span></span>    | <span data-ttu-id="12e49-121">Тип</span><span class="sxs-lookup"><span data-stu-id="12e49-121">Type</span></span>   |<span data-ttu-id="12e49-122">Описание</span><span class="sxs-lookup"><span data-stu-id="12e49-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12e49-123">comment</span><span class="sxs-lookup"><span data-stu-id="12e49-123">comment</span></span>|<span data-ttu-id="12e49-124">String</span><span class="sxs-lookup"><span data-stu-id="12e49-124">String</span></span>|<span data-ttu-id="12e49-p103">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="12e49-p103">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="12e49-127">sendResponse</span><span class="sxs-lookup"><span data-stu-id="12e49-127">sendResponse</span></span>|<span data-ttu-id="12e49-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="12e49-128">Boolean</span></span>|<span data-ttu-id="12e49-p104">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="12e49-p104">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="12e49-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="12e49-132">Response</span></span>

<span data-ttu-id="12e49-p105">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="12e49-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12e49-135">Пример</span><span class="sxs-lookup"><span data-stu-id="12e49-135">Example</span></span>
<span data-ttu-id="12e49-136">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="12e49-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="12e49-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="12e49-137">Request</span></span>
<span data-ttu-id="12e49-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12e49-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="12e49-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="12e49-139">Response</span></span>
##### <a name="response"></a><span data-ttu-id="12e49-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="12e49-140">Response</span></span>
<span data-ttu-id="12e49-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="12e49-141">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
