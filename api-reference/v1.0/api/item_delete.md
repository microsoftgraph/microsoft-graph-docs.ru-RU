# <a name="delete-a-driveitem"></a><span data-ttu-id="0c44e-101">Удаление ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="0c44e-101">Delete a DriveItem</span></span>

<span data-ttu-id="0c44e-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="0c44e-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c44e-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c44e-104">Permissions</span></span>
<span data-ttu-id="0c44e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c44e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c44e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c44e-107">Permission type</span></span>      | <span data-ttu-id="0c44e-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c44e-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="0c44e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c44e-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0c44e-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c44e-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="0c44e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c44e-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c44e-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c44e-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="0c44e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c44e-113">Application</span></span> | <span data-ttu-id="0c44e-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c44e-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c44e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c44e-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="0c44e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c44e-116">Request headers</span></span>

| <span data-ttu-id="0c44e-117">Имя</span><span class="sxs-lookup"><span data-stu-id="0c44e-117">Name</span></span>          | <span data-ttu-id="0c44e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="0c44e-118">Type</span></span>   | <span data-ttu-id="0c44e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0c44e-119">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0c44e-120">if-match</span><span class="sxs-lookup"><span data-stu-id="0c44e-120">if-match</span></span>      | <span data-ttu-id="0c44e-121">String</span><span class="sxs-lookup"><span data-stu-id="0c44e-121">String</span></span> | <span data-ttu-id="0c44e-122">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="0c44e-122">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c44e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c44e-123">Request body</span></span>
<span data-ttu-id="0c44e-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c44e-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="0c44e-125">Пример</span><span class="sxs-lookup"><span data-stu-id="0c44e-125">Example</span></span>

<span data-ttu-id="0c44e-126">Ниже приведен пример, в котором показано, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="0c44e-126">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="0c44e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c44e-127">Response</span></span>

<span data-ttu-id="0c44e-128">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="0c44e-128">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete item"
}-->
