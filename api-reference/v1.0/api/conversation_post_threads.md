# <a name="create-thread"></a><span data-ttu-id="a47e7-101">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="a47e7-101">Create thread</span></span>

<span data-ttu-id="a47e7-102">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="a47e7-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="a47e7-p101">Создание указанных цепочки и записи. Используйте [цепочку ответов](conversationthread_reply.md), чтобы размещать дальнейшие записи в этой цепочке. Кроме того, если вы получаете идентификатор записи, вы можете [ответить](post_reply.md) на эту запись в цепочке.</span><span class="sxs-lookup"><span data-stu-id="a47e7-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="a47e7-106">Примечание. Вы также можете [начать новую беседу, создав цепочку](group_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="a47e7-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a47e7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a47e7-107">Prerequisites</span></span>
<span data-ttu-id="a47e7-108">Для применения этого API требуются указанные ниже **области**. *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="a47e7-108">The following **scopes** are required to execute this API: *Group.ReadWrite.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="a47e7-109">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a47e7-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="a47e7-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a47e7-110">Request headers</span></span>
| <span data-ttu-id="a47e7-111">Имя</span><span class="sxs-lookup"><span data-stu-id="a47e7-111">Name</span></span>       | <span data-ttu-id="a47e7-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a47e7-112">Type</span></span> | <span data-ttu-id="a47e7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a47e7-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a47e7-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="a47e7-114">Authorization</span></span>  | <span data-ttu-id="a47e7-115">string</span><span class="sxs-lookup"><span data-stu-id="a47e7-115">string</span></span>  | <span data-ttu-id="a47e7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a47e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a47e7-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a47e7-118">Request body</span></span>
<span data-ttu-id="a47e7-119">В теле запроса укажите описание объекта [ConversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a47e7-119">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a47e7-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="a47e7-120">Response</span></span>

<span data-ttu-id="a47e7-121">В случае успеха этот метод возвратит код отклика `201, Created` и объект [ConversationThread](../resources/conversationthread.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a47e7-121">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a47e7-122">Пример</span><span class="sxs-lookup"><span data-stu-id="a47e7-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a47e7-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="a47e7-123">Request</span></span>
<span data-ttu-id="a47e7-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a47e7-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
<span data-ttu-id="a47e7-125">В теле запроса укажите описание объекта [conversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a47e7-125">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a47e7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a47e7-126">Response</span></span>

<span data-ttu-id="a47e7-p103">В случае успеха этот метод возвратит код отклика `201, Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a47e7-p103">If successful, this method returns `201, Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
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
