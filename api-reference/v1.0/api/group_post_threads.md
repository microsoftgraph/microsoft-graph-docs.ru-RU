# <a name="create-conversation-thread"></a><span data-ttu-id="2383d-101">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="2383d-101">Create conversation thread</span></span>

<span data-ttu-id="2383d-102">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="2383d-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="2383d-p101">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread_reply.md) и [записи](post_reply.md).</span><span class="sxs-lookup"><span data-stu-id="2383d-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="2383d-105">Примечание. Вы также можете [создать цепочку и существующей беседе](conversation_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="2383d-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="2383d-106">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="2383d-106">Prerequisites</span></span>
<span data-ttu-id="2383d-107">Для применения этого API требуется одна из указанных **областей**: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="2383d-107">One of the following **scopes** is required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="2383d-108">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2383d-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="2383d-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2383d-109">Request headers</span></span>
| <span data-ttu-id="2383d-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2383d-110">Header</span></span>       | <span data-ttu-id="2383d-111">Значение</span><span class="sxs-lookup"><span data-stu-id="2383d-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2383d-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2383d-112">Authorization</span></span>  | <span data-ttu-id="2383d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2383d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2383d-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2383d-115">Content-Type</span></span>  | <span data-ttu-id="2383d-116">application/json</span><span class="sxs-lookup"><span data-stu-id="2383d-116">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2383d-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2383d-117">Request body</span></span>
<span data-ttu-id="2383d-118">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2383d-118">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="2383d-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="2383d-119">Response</span></span>

<span data-ttu-id="2383d-120">В случае успеха этот метод возвращает код отклика `201, Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2383d-120">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2383d-121">Пример</span><span class="sxs-lookup"><span data-stu-id="2383d-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2383d-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="2383d-122">Request</span></span>
<span data-ttu-id="2383d-123">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2383d-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads
Content-type: application/json

{
  "topic": "New Conversation Thread Topic",
  "posts": [{
    "body": {
      "contentType": "html",
      "content": "this is body content"
    },
    "newParticipants": [{
      "emailAddress": {
        "name": "Alex Darrow",
        "address": "alexd@contoso.com"
      }
    }]
  }]
}
```
##### <a name="response"></a><span data-ttu-id="2383d-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="2383d-124">Response</span></span>
<span data-ttu-id="2383d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2383d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
