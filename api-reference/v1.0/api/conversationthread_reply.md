# <a name="conversationthread-reply"></a><span data-ttu-id="155c6-101">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="155c6-101">conversationThread: reply</span></span>

<span data-ttu-id="155c6-p101">Ответ на цепочку в беседе группы и добавление в нее новой записи. Вы можете указать в запросе всю родительскую беседу или только цепочку.</span><span class="sxs-lookup"><span data-stu-id="155c6-p101">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="155c6-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="155c6-104">Prerequisites</span></span>
<span data-ttu-id="155c6-105">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="155c6-105">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="155c6-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="155c6-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="155c6-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="155c6-107">Request headers</span></span>
| <span data-ttu-id="155c6-108">Заголовок</span><span class="sxs-lookup"><span data-stu-id="155c6-108">Header</span></span>       | <span data-ttu-id="155c6-109">Значение</span><span class="sxs-lookup"><span data-stu-id="155c6-109">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="155c6-110">Авторизация</span><span class="sxs-lookup"><span data-stu-id="155c6-110">Authorization</span></span>  | <span data-ttu-id="155c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="155c6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="155c6-113">Content-Type</span><span class="sxs-lookup"><span data-stu-id="155c6-113">Content-Type</span></span>  | <span data-ttu-id="155c6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="155c6-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="155c6-116">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="155c6-116">Request body</span></span>
<span data-ttu-id="155c6-117">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="155c6-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="155c6-118">Параметр</span><span class="sxs-lookup"><span data-stu-id="155c6-118">Parameter</span></span>    | <span data-ttu-id="155c6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="155c6-119">Type</span></span>   |<span data-ttu-id="155c6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="155c6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="155c6-121">post</span><span class="sxs-lookup"><span data-stu-id="155c6-121">post</span></span>|[<span data-ttu-id="155c6-122">post</span><span class="sxs-lookup"><span data-stu-id="155c6-122">post</span></span>](../resources/post.md)|<span data-ttu-id="155c6-123">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="155c6-123">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="155c6-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="155c6-124">Response</span></span>

<span data-ttu-id="155c6-p104">В случае успешного выполнения этот метод возвращает код отклика `202, Accepted`. В теле отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="155c6-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="155c6-127">Пример</span><span class="sxs-lookup"><span data-stu-id="155c6-127">Example</span></span>
<span data-ttu-id="155c6-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="155c6-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="155c6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="155c6-129">Request</span></span>
<span data-ttu-id="155c6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="155c6-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="155c6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="155c6-131">Response</span></span>
<span data-ttu-id="155c6-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="155c6-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
