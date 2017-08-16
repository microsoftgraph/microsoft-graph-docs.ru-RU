# <a name="post-forward"></a><span data-ttu-id="c536b-101">post: forward</span><span class="sxs-lookup"><span data-stu-id="c536b-101">post: forward</span></span>

<span data-ttu-id="c536b-p101">Пересылка записи получателю. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="c536b-p101">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="c536b-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="c536b-104">Prerequisites</span></span>
<span data-ttu-id="c536b-105">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="c536b-105">One of the following **scopes** is required to execute this API:</span></span>

<span data-ttu-id="c536b-106">*Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="c536b-106">*Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="c536b-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c536b-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="c536b-108">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c536b-108">Request headers</span></span>
| <span data-ttu-id="c536b-109">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c536b-109">Header</span></span>       | <span data-ttu-id="c536b-110">Значение</span><span class="sxs-lookup"><span data-stu-id="c536b-110">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c536b-111">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c536b-111">Authorization</span></span>  | <span data-ttu-id="c536b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c536b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c536b-114">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c536b-114">Request body</span></span>
<span data-ttu-id="c536b-115">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="c536b-115">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c536b-116">Параметр</span><span class="sxs-lookup"><span data-stu-id="c536b-116">Parameter</span></span>    | <span data-ttu-id="c536b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c536b-117">Type</span></span>   |<span data-ttu-id="c536b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c536b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c536b-119">comment</span><span class="sxs-lookup"><span data-stu-id="c536b-119">comment</span></span>|<span data-ttu-id="c536b-120">String</span><span class="sxs-lookup"><span data-stu-id="c536b-120">String</span></span>|<span data-ttu-id="c536b-121">Необязательный комментарий, который пересылается вместе с записью.</span><span class="sxs-lookup"><span data-stu-id="c536b-121">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="c536b-122">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c536b-122">toRecipients</span></span>|<span data-ttu-id="c536b-123">Коллекция объектов [recipient](../resources/recipient.md)</span><span class="sxs-lookup"><span data-stu-id="c536b-123">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="c536b-124">Получатели, которым пересылается цепочка.</span><span class="sxs-lookup"><span data-stu-id="c536b-124">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="c536b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c536b-125">Response</span></span>

<span data-ttu-id="c536b-p103">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c536b-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c536b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c536b-128">Example</span></span>
<span data-ttu-id="c536b-129">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c536b-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c536b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c536b-130">Request</span></span>
<span data-ttu-id="c536b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c536b-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="c536b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c536b-132">Response</span></span>
<span data-ttu-id="c536b-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c536b-133">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
