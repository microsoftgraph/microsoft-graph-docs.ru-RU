# <a name="add-attachment"></a><span data-ttu-id="10328-101">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="10328-101">Add attachment</span></span>

<span data-ttu-id="10328-p101">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="10328-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="10328-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10328-104">Permissions</span></span>
<span data-ttu-id="10328-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10328-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="10328-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10328-107">Permission type</span></span>      | <span data-ttu-id="10328-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10328-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10328-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10328-109">Delegated (work or school account)</span></span> | <span data-ttu-id="10328-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10328-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="10328-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10328-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10328-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10328-112">Not supported.</span></span>    |
|<span data-ttu-id="10328-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10328-113">Application</span></span> | <span data-ttu-id="10328-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10328-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10328-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10328-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="10328-116">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="10328-116">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="10328-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10328-117">Request headers</span></span>
| <span data-ttu-id="10328-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10328-118">Header</span></span>       | <span data-ttu-id="10328-119">Значение</span><span class="sxs-lookup"><span data-stu-id="10328-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="10328-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10328-120">Authorization</span></span>  | <span data-ttu-id="10328-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10328-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="10328-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10328-123">Request body</span></span>
<span data-ttu-id="10328-124">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10328-124">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="10328-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="10328-125">Response</span></span>

<span data-ttu-id="10328-126">В случае успеха этот метод возвращает код отклика `201, Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="10328-126">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="10328-127">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="10328-127">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="10328-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="10328-128">Request</span></span>
<span data-ttu-id="10328-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10328-129">Here is an example of the request.</span></span>
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

<span data-ttu-id="10328-130">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10328-130">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="10328-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="10328-131">Response</span></span>
<span data-ttu-id="10328-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10328-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="10328-135">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="10328-135">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="10328-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="10328-136">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="10328-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="10328-137">Response</span></span>
<span data-ttu-id="10328-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="10328-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
