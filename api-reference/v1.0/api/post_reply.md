# <a name="post-reply"></a><span data-ttu-id="dc0d2-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="dc0d2-101">post: reply</span></span>

<span data-ttu-id="dc0d2-p101">Ответ на запись и добавление новой записи в указанную цепочку беседы группы. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc0d2-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="dc0d2-104">Prerequisites</span></span>
<span data-ttu-id="dc0d2-105">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="dc0d2-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="dc0d2-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="dc0d2-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="dc0d2-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc0d2-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="dc0d2-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc0d2-108">Request headers</span></span>
| <span data-ttu-id="dc0d2-109">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dc0d2-109">Header</span></span>       | <span data-ttu-id="dc0d2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="dc0d2-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dc0d2-111">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc0d2-111">Authorization</span></span>  | <span data-ttu-id="dc0d2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc0d2-114">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc0d2-114">Request body</span></span>
<span data-ttu-id="dc0d2-115">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc0d2-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="dc0d2-116">Parameter</span></span>    | <span data-ttu-id="dc0d2-117">Тип</span><span class="sxs-lookup"><span data-stu-id="dc0d2-117">Type</span></span>   |<span data-ttu-id="dc0d2-118">Описание</span><span class="sxs-lookup"><span data-stu-id="dc0d2-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc0d2-119">post</span><span class="sxs-lookup"><span data-stu-id="dc0d2-119">post</span></span>|[<span data-ttu-id="dc0d2-120">post</span><span class="sxs-lookup"><span data-stu-id="dc0d2-120">post</span></span>](../resources/post.md)|<span data-ttu-id="dc0d2-121">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-121">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="dc0d2-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0d2-122">Response</span></span>

<span data-ttu-id="dc0d2-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc0d2-125">Пример</span><span class="sxs-lookup"><span data-stu-id="dc0d2-125">Example</span></span>
<span data-ttu-id="dc0d2-126">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-126">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dc0d2-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc0d2-127">Request</span></span>
<span data-ttu-id="dc0d2-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "datetime-value",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "lastModifiedDateTime": "datetime-value",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```

##### <a name="response"></a><span data-ttu-id="dc0d2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0d2-129">Response</span></span>
##### <a name="response"></a><span data-ttu-id="dc0d2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc0d2-130">Response</span></span>
<span data-ttu-id="dc0d2-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dc0d2-131">Here is an example of the response.</span></span>
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
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
