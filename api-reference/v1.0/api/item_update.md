# <a name="update-driveitem-properties"></a><span data-ttu-id="f7f26-101">Обновление свойств DriveItem</span><span class="sxs-lookup"><span data-stu-id="f7f26-101">Update DriveItem properties</span></span>

<span data-ttu-id="f7f26-102">Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.</span><span class="sxs-lookup"><span data-stu-id="f7f26-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="f7f26-103">Путем обновления также можно [переместить элемент](item_move.md) в другой родительский объект, изменив значение свойства **parentReference**.</span><span class="sxs-lookup"><span data-stu-id="f7f26-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7f26-104">Необходимые условия</span><span class="sxs-lookup"><span data-stu-id="f7f26-104">Prerequisites</span></span>
<span data-ttu-id="f7f26-105">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="f7f26-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="f7f26-106">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="f7f26-106">Files.ReadWrite</span></span>
* <span data-ttu-id="f7f26-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7f26-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="f7f26-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7f26-108">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f7f26-109">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7f26-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="f7f26-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7f26-110">Request headers</span></span>

| <span data-ttu-id="f7f26-111">Имя</span><span class="sxs-lookup"><span data-stu-id="f7f26-111">Name</span></span>          | <span data-ttu-id="f7f26-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f7f26-112">Type</span></span>   | <span data-ttu-id="f7f26-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f7f26-113">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f7f26-114">if-match</span><span class="sxs-lookup"><span data-stu-id="f7f26-114">if-match</span></span>      | <span data-ttu-id="f7f26-115">String</span><span class="sxs-lookup"><span data-stu-id="f7f26-115">String</span></span> | <span data-ttu-id="f7f26-116">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="f7f26-116">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7f26-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f7f26-117">Request body</span></span>
<span data-ttu-id="f7f26-p101">Укажите в тексте запроса значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.</span><span class="sxs-lookup"><span data-stu-id="f7f26-p101">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="f7f26-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7f26-121">Response</span></span>

<span data-ttu-id="f7f26-122">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f7f26-122">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7f26-123">Пример</span><span class="sxs-lookup"><span data-stu-id="f7f26-123">Example</span></span>
<span data-ttu-id="f7f26-124">В этом примере переименовывается ресурс driveItem.</span><span class="sxs-lookup"><span data-stu-id="f7f26-124">This example renames the driveItem.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-file-name.docx"
}
```

##### <a name="response"></a><span data-ttu-id="f7f26-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="f7f26-125">Response</span></span>

<span data-ttu-id="f7f26-p102">Ниже приводится пример отклика. Для наглядности этот отклик сокращен.</span><span class="sxs-lookup"><span data-stu-id="f7f26-p102">The following example shows the response. This response is truncated for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
    "name": "new-file-name.docx",
    "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update item"
}-->
