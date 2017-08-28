# <a name="update-driveitem-properties"></a><span data-ttu-id="71dc6-101">Обновление свойств DriveItem</span><span class="sxs-lookup"><span data-stu-id="71dc6-101">Update DriveItem properties</span></span>

<span data-ttu-id="71dc6-102">Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.</span><span class="sxs-lookup"><span data-stu-id="71dc6-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="71dc6-103">Путем обновления также можно [переместить элемент](item_move.md) в другой родительский объект, изменив свойство **parentReference** этого элемента.</span><span class="sxs-lookup"><span data-stu-id="71dc6-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="71dc6-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71dc6-104">Permissions</span></span>
<span data-ttu-id="71dc6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71dc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71dc6-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71dc6-107">Permission type</span></span>      | <span data-ttu-id="71dc6-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71dc6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71dc6-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71dc6-109">Delegated (work or school account)</span></span> | <span data-ttu-id="71dc6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dc6-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="71dc6-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71dc6-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71dc6-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dc6-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="71dc6-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71dc6-113">Application</span></span> | <span data-ttu-id="71dc6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dc6-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71dc6-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71dc6-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="71dc6-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71dc6-116">Request headers</span></span>

| <span data-ttu-id="71dc6-117">Имя</span><span class="sxs-lookup"><span data-stu-id="71dc6-117">Name</span></span>          | <span data-ttu-id="71dc6-118">Тип</span><span class="sxs-lookup"><span data-stu-id="71dc6-118">Type</span></span>   | <span data-ttu-id="71dc6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="71dc6-119">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="71dc6-120">if-match</span><span class="sxs-lookup"><span data-stu-id="71dc6-120">if-match</span></span>      | <span data-ttu-id="71dc6-121">String</span><span class="sxs-lookup"><span data-stu-id="71dc6-121">String</span></span> | <span data-ttu-id="71dc6-122">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="71dc6-122">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71dc6-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71dc6-123">Request body</span></span>
<span data-ttu-id="71dc6-p102">Укажите в тексте запроса значения обновляемых свойств. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств. Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.</span><span class="sxs-lookup"><span data-stu-id="71dc6-p102">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="71dc6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="71dc6-127">Response</span></span>

<span data-ttu-id="71dc6-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71dc6-128">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71dc6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="71dc6-129">Example</span></span>
<span data-ttu-id="71dc6-130">В этом примере переименовывается ресурс driveItem.</span><span class="sxs-lookup"><span data-stu-id="71dc6-130">This example renames the driveItem.</span></span>

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

##### <a name="response"></a><span data-ttu-id="71dc6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="71dc6-131">Response</span></span>

<span data-ttu-id="71dc6-p103">Ниже приводится пример отклика. Для наглядности этот отклик сокращен.</span><span class="sxs-lookup"><span data-stu-id="71dc6-p103">The following example shows the response. This response is truncated for readability.</span></span>

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
