<span data-ttu-id="cbd12-p101">Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.</span><span class="sxs-lookup"><span data-stu-id="cbd12-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

Удаление ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути. Обратите внимание, что при удалении элементов с помощью этого метода элементы перемещаются в корзину, а не удаляются безвозвратно.

## <span data-ttu-id="cbd12-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cbd12-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="cbd12-105">Для применения этого API требуется одна из указанных **областей**:</span><span class="sxs-lookup"><span data-stu-id="cbd12-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="cbd12-106">Files.ReadWrite.</span><span class="sxs-lookup"><span data-stu-id="cbd12-106">Files.ReadWrite</span></span>
* <span data-ttu-id="cbd12-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbd12-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="cbd12-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbd12-108">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="cbd12-109">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbd12-109">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="cbd12-110">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbd12-110">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="cbd12-111">Имя</span><span class="sxs-lookup"><span data-stu-id="cbd12-111">Name</span></span>          | <span data-ttu-id="cbd12-112">Тип</span><span class="sxs-lookup"><span data-stu-id="cbd12-112">Type</span></span>   | <span data-ttu-id="cbd12-113">Описание</span><span class="sxs-lookup"><span data-stu-id="cbd12-113">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cbd12-114">if-match</span><span class="sxs-lookup"><span data-stu-id="cbd12-114">if-match</span></span>      | <span data-ttu-id="cbd12-115">String</span><span class="sxs-lookup"><span data-stu-id="cbd12-115">String</span></span> | <span data-ttu-id="cbd12-116">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="cbd12-116">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <span data-ttu-id="cbd12-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbd12-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="cbd12-118">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbd12-118">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="cbd12-119">Пример</span><span class="sxs-lookup"><span data-stu-id="cbd12-119">Example</span></span>
<a id="example" class="xliff"></a>

<span data-ttu-id="cbd12-120">Ниже приведен пример, в котором показано, как вызвать этот API.</span><span class="sxs-lookup"><span data-stu-id="cbd12-120">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <span data-ttu-id="cbd12-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbd12-121">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="cbd12-122">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="cbd12-122">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
