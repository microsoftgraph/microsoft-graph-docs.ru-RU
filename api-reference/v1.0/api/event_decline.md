# <a name="event-decline"></a><span data-ttu-id="4aa3a-101">event: decline</span><span class="sxs-lookup"><span data-stu-id="4aa3a-101">event: decline</span></span>

<span data-ttu-id="4aa3a-102">Отклонение приглашения на указанное событие.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-102">Decline invitation to the specified event.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aa3a-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4aa3a-103">Permissions</span></span>
<span data-ttu-id="4aa3a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4aa3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4aa3a-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4aa3a-106">Permission type</span></span>      | <span data-ttu-id="4aa3a-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4aa3a-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="4aa3a-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4aa3a-108">Delegated (work or school account)</span></span> | <span data-ttu-id="4aa3a-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aa3a-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="4aa3a-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4aa3a-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aa3a-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aa3a-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="4aa3a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4aa3a-112">Application</span></span> | <span data-ttu-id="4aa3a-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4aa3a-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4aa3a-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4aa3a-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline
POST /groups/{id}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline
POST /groups/{id}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```
## <a name="request-headers"></a><span data-ttu-id="4aa3a-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4aa3a-115">Request headers</span></span>
| <span data-ttu-id="4aa3a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="4aa3a-116">Name</span></span>       | <span data-ttu-id="4aa3a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4aa3a-117">Type</span></span> | <span data-ttu-id="4aa3a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4aa3a-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4aa3a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aa3a-119">Authorization</span></span>  | <span data-ttu-id="4aa3a-120">string</span><span class="sxs-lookup"><span data-stu-id="4aa3a-120">string</span></span>  | <span data-ttu-id="4aa3a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4aa3a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4aa3a-123">Content-Type</span></span> | <span data-ttu-id="4aa3a-124">string</span><span class="sxs-lookup"><span data-stu-id="4aa3a-124">string</span></span>  | <span data-ttu-id="4aa3a-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4aa3a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4aa3a-127">Request body</span></span>
<span data-ttu-id="4aa3a-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4aa3a-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="4aa3a-129">Parameter</span></span>    | <span data-ttu-id="4aa3a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4aa3a-130">Type</span></span>   |<span data-ttu-id="4aa3a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4aa3a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4aa3a-132">comment</span><span class="sxs-lookup"><span data-stu-id="4aa3a-132">comment</span></span>|<span data-ttu-id="4aa3a-133">String</span><span class="sxs-lookup"><span data-stu-id="4aa3a-133">String</span></span>|<span data-ttu-id="4aa3a-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="4aa3a-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="4aa3a-136">sendResponse</span></span>|<span data-ttu-id="4aa3a-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="4aa3a-137">Boolean</span></span>|<span data-ttu-id="4aa3a-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="4aa3a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4aa3a-141">Response</span></span>

<span data-ttu-id="4aa3a-p106">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aa3a-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4aa3a-144">Example</span></span>
<span data-ttu-id="4aa3a-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4aa3a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4aa3a-146">Request</span></span>
<span data-ttu-id="4aa3a-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="4aa3a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4aa3a-148">Response</span></span>
##### <a name="response"></a><span data-ttu-id="4aa3a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4aa3a-149">Response</span></span>
<span data-ttu-id="4aa3a-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4aa3a-150">Here is an example of the response.</span></span>
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
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
