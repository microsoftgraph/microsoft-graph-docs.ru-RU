# <a name="message-reply"></a><span data-ttu-id="8eaea-101">message: reply</span><span class="sxs-lookup"><span data-stu-id="8eaea-101">message: reply</span></span>

<span data-ttu-id="8eaea-p101">Ответ отправителю сообщения. Затем сообщение сохраняется в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="8eaea-p101">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eaea-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8eaea-104">Prerequisites</span></span>
<span data-ttu-id="8eaea-105">Для применения этого API требуется одна из указанных **областей**: *Mail.Send*</span><span class="sxs-lookup"><span data-stu-id="8eaea-105">One of the following **scopes** is required to execute this API: *Mail.Send*</span></span>
## <a name="http-request"></a><span data-ttu-id="8eaea-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eaea-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="8eaea-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8eaea-107">Request headers</span></span>
| <span data-ttu-id="8eaea-108">Имя</span><span class="sxs-lookup"><span data-stu-id="8eaea-108">Name</span></span>       | <span data-ttu-id="8eaea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8eaea-109">Type</span></span> | <span data-ttu-id="8eaea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8eaea-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8eaea-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eaea-111">Authorization</span></span>  | <span data-ttu-id="8eaea-112">string</span><span class="sxs-lookup"><span data-stu-id="8eaea-112">string</span></span>  | <span data-ttu-id="8eaea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eaea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8eaea-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8eaea-115">Content-Type</span></span> | <span data-ttu-id="8eaea-116">string</span><span class="sxs-lookup"><span data-stu-id="8eaea-116">string</span></span>  | <span data-ttu-id="8eaea-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8eaea-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8eaea-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8eaea-119">Request body</span></span>
<span data-ttu-id="8eaea-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8eaea-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8eaea-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="8eaea-121">Parameter</span></span>    | <span data-ttu-id="8eaea-122">Тип</span><span class="sxs-lookup"><span data-stu-id="8eaea-122">Type</span></span>   |<span data-ttu-id="8eaea-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8eaea-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eaea-124">comment</span><span class="sxs-lookup"><span data-stu-id="8eaea-124">comment</span></span>|<span data-ttu-id="8eaea-125">String</span><span class="sxs-lookup"><span data-stu-id="8eaea-125">String</span></span>|<span data-ttu-id="8eaea-p104">Добавляемый комментарий. Может быть пустой строкой.</span><span class="sxs-lookup"><span data-stu-id="8eaea-p104">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="8eaea-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eaea-128">Response</span></span>

<span data-ttu-id="8eaea-p105">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8eaea-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eaea-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8eaea-131">Example</span></span>
<span data-ttu-id="8eaea-132">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8eaea-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8eaea-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eaea-133">Request</span></span>
<span data-ttu-id="8eaea-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8eaea-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="8eaea-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eaea-135">Response</span></span>
##### <a name="response"></a><span data-ttu-id="8eaea-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eaea-136">Response</span></span>
<span data-ttu-id="8eaea-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8eaea-137">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
