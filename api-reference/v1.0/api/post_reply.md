# <a name="post-reply"></a><span data-ttu-id="9dc7c-101">post: reply</span><span class="sxs-lookup"><span data-stu-id="9dc7c-101">post: reply</span></span>

<span data-ttu-id="9dc7c-p101">Ответ на запись и добавление новой записи в указанную цепочку беседы группы. Вы можете указать в запросе родительскую беседу вместе с цепочкой или только родительскую цепочку.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-p101">Reply to a post and add a new post to the specified thread in a group conversation. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dc7c-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9dc7c-104">Permissions</span></span>
<span data-ttu-id="9dc7c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9dc7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9dc7c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dc7c-107">Permission type</span></span>      | <span data-ttu-id="9dc7c-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dc7c-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9dc7c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dc7c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9dc7c-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc7c-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="9dc7c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dc7c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dc7c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-112">Not supported.</span></span>    | 
|<span data-ttu-id="9dc7c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dc7c-113">Application</span></span> | <span data-ttu-id="9dc7c-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dc7c-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9dc7c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dc7c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="9dc7c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dc7c-116">Request headers</span></span>
| <span data-ttu-id="9dc7c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9dc7c-117">Header</span></span>       | <span data-ttu-id="9dc7c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9dc7c-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9dc7c-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dc7c-119">Authorization</span></span>  | <span data-ttu-id="9dc7c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9dc7c-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dc7c-122">Request body</span></span>
<span data-ttu-id="9dc7c-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9dc7c-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="9dc7c-124">Parameter</span></span>    | <span data-ttu-id="9dc7c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9dc7c-125">Type</span></span>   |<span data-ttu-id="9dc7c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9dc7c-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dc7c-127">post</span><span class="sxs-lookup"><span data-stu-id="9dc7c-127">post</span></span>|[<span data-ttu-id="9dc7c-128">post</span><span class="sxs-lookup"><span data-stu-id="9dc7c-128">post</span></span>](../resources/post.md)|<span data-ttu-id="9dc7c-129">Новая запись для ответа.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-129">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="9dc7c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dc7c-130">Response</span></span>

<span data-ttu-id="9dc7c-p104">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dc7c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9dc7c-133">Example</span></span>
<span data-ttu-id="9dc7c-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-134">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9dc7c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dc7c-135">Request</span></span>
<span data-ttu-id="9dc7c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="9dc7c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dc7c-137">Response</span></span>
##### <a name="response"></a><span data-ttu-id="9dc7c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dc7c-138">Response</span></span>
<span data-ttu-id="9dc7c-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9dc7c-139">Here is an example of the response.</span></span>
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
