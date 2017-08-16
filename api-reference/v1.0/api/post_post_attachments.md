# <a name="add-attachment"></a><span data-ttu-id="8105c-101">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="8105c-101">Add attachment</span></span>

<span data-ttu-id="8105c-p101">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="8105c-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8105c-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="8105c-104">Prerequisites</span></span>
<span data-ttu-id="8105c-105">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="8105c-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="8105c-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8105c-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8105c-107">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8105c-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8105c-108">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="8105c-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="8105c-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8105c-109">Request headers</span></span>
| <span data-ttu-id="8105c-110">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8105c-110">Header</span></span>       | <span data-ttu-id="8105c-111">Значение</span><span class="sxs-lookup"><span data-stu-id="8105c-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8105c-112">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8105c-112">Authorization</span></span>  | <span data-ttu-id="8105c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8105c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8105c-115">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8105c-115">Request body</span></span>
<span data-ttu-id="8105c-116">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8105c-116">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8105c-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="8105c-117">Response</span></span>

<span data-ttu-id="8105c-118">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8105c-118">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="8105c-119">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="8105c-119">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8105c-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="8105c-120">Request</span></span>
<span data-ttu-id="8105c-121">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8105c-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="8105c-122">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8105c-122">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="8105c-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="8105c-123">Response</span></span>
<span data-ttu-id="8105c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8105c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="8105c-127">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="8105c-127">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="8105c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8105c-128">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="8105c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8105c-129">Response</span></span>
<span data-ttu-id="8105c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8105c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
