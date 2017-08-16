# <a name="message-move"></a><span data-ttu-id="0bdcc-101">message: move</span><span class="sxs-lookup"><span data-stu-id="0bdcc-101">message: move</span></span>

<span data-ttu-id="0bdcc-p101">Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bdcc-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0bdcc-104">Prerequisites</span></span>
<span data-ttu-id="0bdcc-105">Для применения этого API требуется следующая **область**: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="0bdcc-105">One of the following **scopes** is required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="0bdcc-106">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bdcc-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="0bdcc-107">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bdcc-107">Request headers</span></span>
| <span data-ttu-id="0bdcc-108">Имя</span><span class="sxs-lookup"><span data-stu-id="0bdcc-108">Name</span></span>       | <span data-ttu-id="0bdcc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0bdcc-109">Type</span></span> | <span data-ttu-id="0bdcc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0bdcc-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0bdcc-111">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bdcc-111">Authorization</span></span>  | <span data-ttu-id="0bdcc-112">string</span><span class="sxs-lookup"><span data-stu-id="0bdcc-112">string</span></span>  | <span data-ttu-id="0bdcc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0bdcc-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0bdcc-115">Content-Type</span></span> | <span data-ttu-id="0bdcc-116">string</span><span class="sxs-lookup"><span data-stu-id="0bdcc-116">string</span></span>  | <span data-ttu-id="0bdcc-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bdcc-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0bdcc-119">Request body</span></span>
<span data-ttu-id="0bdcc-120">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-120">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0bdcc-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="0bdcc-121">Parameter</span></span>    | <span data-ttu-id="0bdcc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0bdcc-122">Type</span></span>   |<span data-ttu-id="0bdcc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0bdcc-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bdcc-124">DestinationId</span><span class="sxs-lookup"><span data-stu-id="0bdcc-124">DestinationId</span></span>|<span data-ttu-id="0bdcc-125">String</span><span class="sxs-lookup"><span data-stu-id="0bdcc-125">String</span></span>|<span data-ttu-id="0bdcc-126">Идентификатор целевой папки либо имя известной папки `Inbox`, `Drafts`, `SentItems` или `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-126">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="0bdcc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdcc-127">Response</span></span>

<span data-ttu-id="0bdcc-128">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-128">If successful, this method returns `201, Created` response code and [message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bdcc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0bdcc-129">Example</span></span>
<span data-ttu-id="0bdcc-130">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0bdcc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdcc-131">Request</span></span>
<span data-ttu-id="0bdcc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_move"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/move
Content-type: application/json
Content-length: 44

{
  "DestinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="0bdcc-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdcc-133">Response</span></span>
<span data-ttu-id="0bdcc-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0bdcc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
