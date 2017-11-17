# <a name="create-thread"></a><span data-ttu-id="4c413-101">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="4c413-101">Create thread</span></span>

<span data-ttu-id="4c413-102">Создание цепочки в указанной беседе.</span><span class="sxs-lookup"><span data-stu-id="4c413-102">Create a new thread in the specified conversation.</span></span> 

<span data-ttu-id="4c413-p101">Создание указанных цепочки и записи. Используйте [цепочку ответов](conversationthread_reply.md), чтобы размещать дальнейшие записи в этой цепочке. Кроме того, если вы получаете идентификатор записи, вы можете [ответить](post_reply.md) на эту запись в цепочке.</span><span class="sxs-lookup"><span data-stu-id="4c413-p101">A thread and post are created as specified. Use [reply thread](conversationthread_reply.md) to further post to that thread. Or, if you get the post ID, you can also [reply](post_reply.md) to that post in that thread.</span></span>

<span data-ttu-id="4c413-106">Примечание. Вы также можете [начать новую беседу, создав цепочку](group_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="4c413-106">Note: You can also [start a new conversation by first creating a thread](group_post_threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c413-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c413-107">Permissions</span></span>
<span data-ttu-id="4c413-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c413-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c413-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c413-110">Permission type</span></span>      | <span data-ttu-id="4c413-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c413-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c413-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c413-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4c413-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c413-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c413-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c413-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c413-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c413-115">Not supported.</span></span>    |
|<span data-ttu-id="4c413-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c413-116">Application</span></span> | <span data-ttu-id="4c413-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c413-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c413-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c413-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="4c413-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c413-119">Request headers</span></span>
| <span data-ttu-id="4c413-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4c413-120">Name</span></span>       | <span data-ttu-id="4c413-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4c413-121">Type</span></span> | <span data-ttu-id="4c413-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4c413-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c413-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c413-123">Authorization</span></span>  | <span data-ttu-id="4c413-124">string</span><span class="sxs-lookup"><span data-stu-id="4c413-124">string</span></span>  | <span data-ttu-id="4c413-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c413-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c413-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c413-127">Request body</span></span>
<span data-ttu-id="4c413-128">В теле запроса укажите описание объекта [ConversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c413-128">In the request body, supply a JSON representation of [ConversationThread](../resources/conversationthread.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4c413-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c413-129">Response</span></span>

<span data-ttu-id="4c413-130">В случае успеха этот метод возвратит код отклика `201 Created` и объект [ConversationThread](../resources/conversationthread.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c413-130">If successful, this method returns `201 Created` response code and [ConversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c413-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4c413-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c413-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c413-132">Request</span></span>
<span data-ttu-id="4c413-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c413-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="4c413-134">В теле запроса укажите описание объекта [conversationThread](../resources/conversationthread.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c413-134">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4c413-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c413-135">Response</span></span>

<span data-ttu-id="4c413-p104">В случае успеха этот метод возвратит код отклика `201 Created` и `id` новой цепочки в теле отклика. Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c413-p104">If successful, this method returns `201 Created` response code and the `id` of the new thread in the response body. Here is an example of the response.</span></span> 
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
