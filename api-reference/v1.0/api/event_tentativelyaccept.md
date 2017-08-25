# <a name="event-tentativelyaccept"></a><span data-ttu-id="9d219-101">event: tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="9d219-101">event: tentativelyAccept</span></span>

<span data-ttu-id="9d219-102">Предварительное принятие приглашения, связанного с указанным событием.</span><span class="sxs-lookup"><span data-stu-id="9d219-102">Tentatively accept the specified event.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d219-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d219-103">Permissions</span></span>
<span data-ttu-id="9d219-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9d219-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9d219-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d219-106">Permission type</span></span>      | <span data-ttu-id="9d219-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d219-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9d219-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d219-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9d219-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d219-109">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="9d219-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d219-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d219-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d219-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="9d219-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d219-112">Application</span></span> | <span data-ttu-id="9d219-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9d219-113">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9d219-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d219-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="9d219-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d219-115">Request headers</span></span>
| <span data-ttu-id="9d219-116">Имя</span><span class="sxs-lookup"><span data-stu-id="9d219-116">Name</span></span>       | <span data-ttu-id="9d219-117">Тип</span><span class="sxs-lookup"><span data-stu-id="9d219-117">Type</span></span> | <span data-ttu-id="9d219-118">Описание</span><span class="sxs-lookup"><span data-stu-id="9d219-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9d219-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d219-119">Authorization</span></span>  | <span data-ttu-id="9d219-120">string</span><span class="sxs-lookup"><span data-stu-id="9d219-120">string</span></span>  | <span data-ttu-id="9d219-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d219-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9d219-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d219-123">Content-Type</span></span> | <span data-ttu-id="9d219-124">string</span><span class="sxs-lookup"><span data-stu-id="9d219-124">string</span></span>  | <span data-ttu-id="9d219-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d219-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d219-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d219-127">Request body</span></span>
<span data-ttu-id="9d219-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9d219-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9d219-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="9d219-129">Parameter</span></span>    | <span data-ttu-id="9d219-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9d219-130">Type</span></span>   |<span data-ttu-id="9d219-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9d219-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d219-132">comment</span><span class="sxs-lookup"><span data-stu-id="9d219-132">comment</span></span>|<span data-ttu-id="9d219-133">String</span><span class="sxs-lookup"><span data-stu-id="9d219-133">String</span></span>|<span data-ttu-id="9d219-p104">Текст, включенный в ответ. Необязательный.</span><span class="sxs-lookup"><span data-stu-id="9d219-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="9d219-136">sendResponse</span><span class="sxs-lookup"><span data-stu-id="9d219-136">sendResponse</span></span>|<span data-ttu-id="9d219-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="9d219-137">Boolean</span></span>|<span data-ttu-id="9d219-p105">Значение `true` указывает, что организатору должен быть отправлен ответ. В противном случае используется значение `false`. Необязательный. Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="9d219-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="9d219-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d219-141">Response</span></span>

<span data-ttu-id="9d219-p106">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9d219-p106">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d219-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9d219-144">Example</span></span>
<span data-ttu-id="9d219-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9d219-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9d219-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d219-146">Request</span></span>
<span data-ttu-id="9d219-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d219-147">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9d219-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d219-148">Response</span></span>
##### <a name="response"></a><span data-ttu-id="9d219-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d219-149">Response</span></span>
<span data-ttu-id="9d219-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9d219-150">Here is an example of the response.</span></span>
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
