# <a name="create-conversation-thread"></a><span data-ttu-id="2905c-101">Создание цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="2905c-101">Create conversation thread</span></span>

<span data-ttu-id="2905c-102">Начните групповой чат, создав цепочку.</span><span class="sxs-lookup"><span data-stu-id="2905c-102">Start a new group conversation by first creating a thread.</span></span> 

<span data-ttu-id="2905c-p101">В группе создаются беседа, цепочка беседы и запись. Размещать в цепочке дальнейшие записи можно с помощью ответов на [цепочки](conversationthread_reply.md) и [записи](post_reply.md).</span><span class="sxs-lookup"><span data-stu-id="2905c-p101">A new conversation, conversation thread, and post are created in the group. Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that thread.</span></span>

<span data-ttu-id="2905c-105">Примечание. Вы можете [создать цепочку в существующей беседе](conversation_post_threads.md).</span><span class="sxs-lookup"><span data-stu-id="2905c-105">Note: You can also [start a new thread in an existing conversation](conversation_post_threads.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2905c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2905c-106">Permissions</span></span>
<span data-ttu-id="2905c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2905c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2905c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2905c-109">Permission type</span></span>      | <span data-ttu-id="2905c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2905c-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="2905c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2905c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2905c-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2905c-112">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="2905c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2905c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2905c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2905c-114">Not supported.</span></span>    | 
|<span data-ttu-id="2905c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2905c-115">Application</span></span> | <span data-ttu-id="2905c-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2905c-116">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2905c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2905c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads
```
## <a name="request-headers"></a><span data-ttu-id="2905c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2905c-118">Request headers</span></span>
| <span data-ttu-id="2905c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2905c-119">Header</span></span>       | <span data-ttu-id="2905c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2905c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2905c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2905c-121">Authorization</span></span>  | <span data-ttu-id="2905c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2905c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2905c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2905c-124">Content-Type</span></span>  | <span data-ttu-id="2905c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2905c-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2905c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2905c-126">Request body</span></span>
<span data-ttu-id="2905c-127">Предоставьте в тексте запроса описание объекта [conversationThread](../resources/conversationthread.md), содержащего объект [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2905c-127">In the request body, supply a JSON representation of [conversationThread](../resources/conversationthread.md) object containing a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="2905c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2905c-128">Response</span></span>

<span data-ttu-id="2905c-129">В случае успеха этот метод возвращает код отклика `201, Created` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2905c-129">If successful, this method returns `201, Created` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2905c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2905c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2905c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2905c-131">Request</span></span>
<span data-ttu-id="2905c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2905c-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2905c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="2905c-133">Response</span></span>
<span data-ttu-id="2905c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2905c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
