# <a name="add-attachment"></a><span data-ttu-id="a6053-101">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="a6053-101">Add attachment</span></span>

<span data-ttu-id="a6053-p101">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="a6053-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="a6053-104">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="a6053-104">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="a6053-105">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a6053-105">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="a6053-106">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="a6053-106">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="a6053-107">ссылка на файл (ресурс [referenceAttachment](../resources/referenceAttachment.md)).</span><span class="sxs-lookup"><span data-stu-id="a6053-107">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="a6053-108">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="a6053-108">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a6053-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6053-109">Permissions</span></span>
<span data-ttu-id="a6053-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a6053-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6053-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6053-112">Permission type</span></span>      | <span data-ttu-id="a6053-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6053-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6053-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6053-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a6053-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6053-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6053-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6053-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6053-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6053-117">Not supported.</span></span>    |
|<span data-ttu-id="a6053-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6053-118">Application</span></span> | <span data-ttu-id="a6053-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6053-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6053-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6053-120">HTTP request</span></span>
<span data-ttu-id="a6053-121"><!-- { "blockType": "ignored" } --> Вложения для публикации ([post](../resources/post.md)) в цепочке ([thread](../resources/conversationthread.md)) беседы ([thread](../resources/conversation.md)) в группе.</span><span class="sxs-lookup"><span data-stu-id="a6053-121">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="a6053-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6053-122">Request headers</span></span>
| <span data-ttu-id="a6053-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6053-123">Header</span></span>       | <span data-ttu-id="a6053-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a6053-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a6053-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6053-125">Authorization</span></span>  | <span data-ttu-id="a6053-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6053-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6053-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6053-128">Request body</span></span>
<span data-ttu-id="a6053-129">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6053-129">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a6053-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6053-130">Response</span></span>

<span data-ttu-id="a6053-131">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a6053-131">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="a6053-132">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="a6053-132">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a6053-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6053-133">Request</span></span>
<span data-ttu-id="a6053-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6053-134">Here is an example of the request.</span></span>
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
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="a6053-135">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6053-135">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="a6053-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6053-136">Response</span></span>
<span data-ttu-id="a6053-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6053-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="a6053-140">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="a6053-140">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="a6053-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6053-141">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="a6053-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6053-142">Response</span></span>
<span data-ttu-id="a6053-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6053-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
