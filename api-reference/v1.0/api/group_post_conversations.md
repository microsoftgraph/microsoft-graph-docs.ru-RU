# <a name="create-conversation"></a><span data-ttu-id="fcf11-101">Создание объекта Conversation</span><span class="sxs-lookup"><span data-stu-id="fcf11-101">Create Conversation</span></span>

<span data-ttu-id="fcf11-102">Создание беседы путем включения цепочки и записи.</span><span class="sxs-lookup"><span data-stu-id="fcf11-102">Create a new conversation by including a thread and a post.</span></span> 

<span data-ttu-id="fcf11-103">Размещать в беседе дальнейшие записи можно с помощью [ответов на цепочки](conversationthread_reply.md) и [ответов на записи](post_reply.md).</span><span class="sxs-lookup"><span data-stu-id="fcf11-103">Use [reply thread](conversationthread_reply.md) or [reply post](post_reply.md) to further post to that conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="fcf11-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf11-104">Permissions</span></span>
<span data-ttu-id="fcf11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fcf11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fcf11-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcf11-107">Permission type</span></span>      | <span data-ttu-id="fcf11-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcf11-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fcf11-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcf11-109">Delegated (work or school account)</span></span> | <span data-ttu-id="fcf11-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf11-110">Group.ReadWrite.All</span></span>    | 
|<span data-ttu-id="fcf11-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcf11-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fcf11-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcf11-112">Not supported.</span></span>    | 
|<span data-ttu-id="fcf11-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcf11-113">Application</span></span> | <span data-ttu-id="fcf11-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf11-114">Group.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fcf11-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcf11-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations
```
## <a name="request-headers"></a><span data-ttu-id="fcf11-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcf11-116">Request headers</span></span>
| <span data-ttu-id="fcf11-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcf11-117">Header</span></span>       | <span data-ttu-id="fcf11-118">Значение</span><span class="sxs-lookup"><span data-stu-id="fcf11-118">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fcf11-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcf11-119">Authorization</span></span>  | <span data-ttu-id="fcf11-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcf11-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fcf11-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcf11-122">Content-Type</span></span>  | <span data-ttu-id="fcf11-123">application/json</span><span class="sxs-lookup"><span data-stu-id="fcf11-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fcf11-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcf11-124">Request body</span></span>
<span data-ttu-id="fcf11-125">Предоставьте в тексте запроса описание объекта [conversation](../resources/conversation.md), содержащего объекты [conversationThread](../resources/conversationThread.md) и [post](../resources/post.md), в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcf11-125">In the request body, supply a JSON representation of [conversation](../resources/conversation.md) object containing a [conversationThread](../resources/conversationThread.md) and a [post](../resources/post.md).</span></span>

## <a name="response"></a><span data-ttu-id="fcf11-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcf11-126">Response</span></span>

<span data-ttu-id="fcf11-127">В случае успеха этот метод возвращает код отклика `201, Created` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fcf11-127">If successful, this method returns `201, Created` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcf11-128">Пример</span><span class="sxs-lookup"><span data-stu-id="fcf11-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcf11-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcf11-129">Request</span></span>
<span data-ttu-id="fcf11-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcf11-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_conversation_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations
Content-type: application/json

{
  "topic": "New Conversation Topic",
  "threads": [{
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
  }]
}
```
##### <a name="response"></a><span data-ttu-id="fcf11-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fcf11-131">Response</span></span>
<span data-ttu-id="fcf11-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fcf11-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->