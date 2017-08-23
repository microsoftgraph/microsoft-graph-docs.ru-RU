# <a name="move-a-driveitem"></a><span data-ttu-id="c55be-101">Перемещение ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="c55be-101">Move a DriveItem</span></span>

<span data-ttu-id="c55be-p101">Чтобы переместить ресурс DriveItem в новый родительский элемент, веб-приложению требуется обновить элемент **parentReference** из DriveItem. Это особый случай, касающийся метода [Обновление](item_update.md). Приложение может объединять процедуры перемещения элемента в новый контейнер и обновления других свойств элемента в один запрос.</span><span class="sxs-lookup"><span data-stu-id="c55be-p101">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move. This is a special case of the [Update](item_update.md) method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="c55be-105">С помощью этого запроса невозможно перемещать элементы между объектами [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="c55be-105">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="c55be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c55be-106">Permissions</span></span>
<span data-ttu-id="c55be-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c55be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c55be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c55be-109">Permission type</span></span>      | <span data-ttu-id="c55be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c55be-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="c55be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c55be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c55be-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c55be-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c55be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c55be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c55be-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c55be-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="c55be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c55be-115">Application</span></span> | <span data-ttu-id="c55be-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c55be-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c55be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c55be-117">HTTP request</span></span>

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="c55be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c55be-118">Request headers</span></span>

| <span data-ttu-id="c55be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c55be-119">Name</span></span>          | <span data-ttu-id="c55be-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c55be-120">Type</span></span>   | <span data-ttu-id="c55be-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c55be-121">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c55be-122">if-match</span><span class="sxs-lookup"><span data-stu-id="c55be-122">if-match</span></span>      | <span data-ttu-id="c55be-123">String</span><span class="sxs-lookup"><span data-stu-id="c55be-123">String</span></span> | <span data-ttu-id="c55be-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="c55be-124">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c55be-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c55be-125">Request body</span></span>
<span data-ttu-id="c55be-p103">В тексте запроса предоставьте новое значение для поля свойства **parentReference**. Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в другие значения свойств. Чтобы производительность была максимальной, не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c55be-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="c55be-p104">**Примечание.** При перемещении элементов в корень OneDrive не следует использовать синтаксис `"id:" "root"`. Нужно использовать действительный идентификатор корневой папки или путь `{"path": "/drive/root"}` для родительской ссылки.</span><span class="sxs-lookup"><span data-stu-id="c55be-p104">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="c55be-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="c55be-131">Response</span></span>

<span data-ttu-id="c55be-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c55be-132">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c55be-133">Пример</span><span class="sxs-lookup"><span data-stu-id="c55be-133">Example</span></span>
<span data-ttu-id="c55be-134">В этом примере элемент, определяемый идентификатором элемента {item-id}, перемещается в папку **Документы** в OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="c55be-134">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a><span data-ttu-id="c55be-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c55be-135">Response</span></span>

<span data-ttu-id="c55be-136">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c55be-136">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
