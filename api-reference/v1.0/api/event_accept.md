# <a name="event-accept"></a><span data-ttu-id="d47c2-101">event: accept</span><span class="sxs-lookup"><span data-stu-id="d47c2-101">event: accept</span></span>

<span data-ttu-id="d47c2-102">Принятие приглашения на указанное событие.</span><span class="sxs-lookup"><span data-stu-id="d47c2-102">Accept the specified event.</span></span>

## <a name="permissions"></a><span data-ttu-id="d47c2-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d47c2-103">Permissions</span></span>
<span data-ttu-id="d47c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d47c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d47c2-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d47c2-106">Permission type</span></span>      | <span data-ttu-id="d47c2-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d47c2-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d47c2-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d47c2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d47c2-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47c2-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="d47c2-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d47c2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d47c2-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47c2-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="d47c2-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d47c2-112">Application</span></span> | <span data-ttu-id="d47c2-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d47c2-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d47c2-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d47c2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept
POST /groups/{id}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept
POST /groups/{id}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroup/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="d47c2-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d47c2-115">Request headers</span></span>
| <span data-ttu-id="d47c2-116">Имя</span><span class="sxs-lookup"><span data-stu-id="d47c2-116">Name</span></span>       | <span data-ttu-id="d47c2-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d47c2-117">Type</span></span> | <span data-ttu-id="d47c2-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d47c2-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d47c2-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d47c2-119">Authorization</span></span>  | <span data-ttu-id="d47c2-120">string</span><span class="sxs-lookup"><span data-stu-id="d47c2-120">string</span></span>  | <span data-ttu-id="d47c2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d47c2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d47c2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d47c2-123">Content-Type</span></span> | <span data-ttu-id="d47c2-124">string</span><span class="sxs-lookup"><span data-stu-id="d47c2-124">string</span></span>  | <span data-ttu-id="d47c2-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d47c2-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d47c2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d47c2-127">Request body</span></span>
<span data-ttu-id="d47c2-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d47c2-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d47c2-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="d47c2-129">Parameter</span></span>    | <span data-ttu-id="d47c2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d47c2-130">Type</span></span>   |<span data-ttu-id="d47c2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d47c2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d47c2-132">comment</span><span class="sxs-lookup"><span data-stu-id="d47c2-132">comment</span></span>|<span data-ttu-id="d47c2-133">String</span><span class="sxs-lookup"><span data-stu-id="d47c2-133">String</span></span>|<span data-ttu-id="d47c2-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="d47c2-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="d47c2-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="d47c2-136">sendResponse</span></span>|<span data-ttu-id="d47c2-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="d47c2-137">Boolean</span></span>|<span data-ttu-id="d47c2-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="d47c2-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="d47c2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d47c2-141">Response</span></span>

<span data-ttu-id="d47c2-p106">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d47c2-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d47c2-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d47c2-144">Example</span></span>
<span data-ttu-id="d47c2-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="d47c2-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d47c2-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="d47c2-146">Request</span></span>
<span data-ttu-id="d47c2-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d47c2-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <a name="response"></a><span data-ttu-id="d47c2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d47c2-148">Response</span></span>
<span data-ttu-id="d47c2-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d47c2-149">Here is an example of the response.</span></span>
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
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
