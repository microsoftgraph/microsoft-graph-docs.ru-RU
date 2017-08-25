# <a name="message-move"></a><span data-ttu-id="84556-101">message: move</span><span class="sxs-lookup"><span data-stu-id="84556-101">message: move</span></span>

<span data-ttu-id="84556-p101">Перемещение сообщения в папку. При этом в целевой папке создается новая копия сообщения.</span><span class="sxs-lookup"><span data-stu-id="84556-p101">Move a message to a folder. This creates a new copy of the message in the destination folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="84556-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84556-104">Permissions</span></span>
<span data-ttu-id="84556-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="84556-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="84556-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84556-107">Permission type</span></span>      | <span data-ttu-id="84556-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84556-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="84556-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84556-109">Delegated (work or school account)</span></span> | <span data-ttu-id="84556-110">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84556-110">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="84556-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84556-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84556-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84556-112">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="84556-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84556-113">Application</span></span> | <span data-ttu-id="84556-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="84556-114">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="84556-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84556-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/move
POST /users/{id | userPrincipalName}/messages/{id}/move
POST /me/mailFolders/{id}/messages/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/move
```
## <a name="request-headers"></a><span data-ttu-id="84556-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84556-116">Request headers</span></span>
| <span data-ttu-id="84556-117">Имя</span><span class="sxs-lookup"><span data-stu-id="84556-117">Name</span></span>       | <span data-ttu-id="84556-118">Тип</span><span class="sxs-lookup"><span data-stu-id="84556-118">Type</span></span> | <span data-ttu-id="84556-119">Описание</span><span class="sxs-lookup"><span data-stu-id="84556-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="84556-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="84556-120">Authorization</span></span>  | <span data-ttu-id="84556-121">string</span><span class="sxs-lookup"><span data-stu-id="84556-121">string</span></span>  | <span data-ttu-id="84556-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84556-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84556-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84556-124">Content-Type</span></span> | <span data-ttu-id="84556-125">string</span><span class="sxs-lookup"><span data-stu-id="84556-125">string</span></span>  | <span data-ttu-id="84556-p104">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84556-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84556-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84556-128">Request body</span></span>
<span data-ttu-id="84556-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="84556-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="84556-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="84556-130">Parameter</span></span>    | <span data-ttu-id="84556-131">Тип</span><span class="sxs-lookup"><span data-stu-id="84556-131">Type</span></span>   |<span data-ttu-id="84556-132">Описание</span><span class="sxs-lookup"><span data-stu-id="84556-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84556-133">DestinationId</span><span class="sxs-lookup"><span data-stu-id="84556-133">DestinationId</span></span>|<span data-ttu-id="84556-134">String</span><span class="sxs-lookup"><span data-stu-id="84556-134">String</span></span>|<span data-ttu-id="84556-135">Идентификатор целевой папки либо имя известной папки `Inbox`, `Drafts`, `SentItems` или `DeletedItems`.</span><span class="sxs-lookup"><span data-stu-id="84556-135">The destination folder ID, or the `Inbox`, `Drafts`, `SentItems`, or `DeletedItems` well-known folder name.</span></span>|

## <a name="response"></a><span data-ttu-id="84556-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="84556-136">Response</span></span>

<span data-ttu-id="84556-137">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Message](../resources/message.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84556-137">If successful, this method returns `201, Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84556-138">Пример</span><span class="sxs-lookup"><span data-stu-id="84556-138">Example</span></span>
<span data-ttu-id="84556-139">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="84556-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="84556-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="84556-140">Request</span></span>
<span data-ttu-id="84556-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84556-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="84556-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="84556-142">Response</span></span>
<span data-ttu-id="84556-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="84556-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
