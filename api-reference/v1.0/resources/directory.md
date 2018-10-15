# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="a3359-101">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="a3359-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="a3359-102">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a3359-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="a3359-103">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="a3359-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="a3359-104">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="a3359-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="a3359-105">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="a3359-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="a3359-106">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="a3359-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a3359-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a3359-107">Methods</span></span>

| <span data-ttu-id="a3359-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a3359-108">Method</span></span>         | <span data-ttu-id="a3359-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3359-109">Return Type</span></span> | <span data-ttu-id="a3359-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3359-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="a3359-111">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="a3359-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="a3359-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a3359-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="a3359-113">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="a3359-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="a3359-114">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="a3359-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="a3359-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a3359-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="a3359-116">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="a3359-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="a3359-117">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="a3359-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="a3359-118">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a3359-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a3359-119">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="a3359-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="a3359-120">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="a3359-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="a3359-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a3359-121">None</span></span> | <span data-ttu-id="a3359-122">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="a3359-122">Permanently deletes an item.</span></span> |
|<span data-ttu-id="a3359-123">[Перечисление удаленных элементов, принадлежащих пользователю](../api/directory_deleteditems_user_owned.md)</span><span class="sxs-lookup"><span data-stu-id="a3359-123">Added [List deleted items owned by a user](../api/directory_deleteditems_user_owned.md) action to directory (deleted items) resource</span></span> | <span data-ttu-id="a3359-124">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a3359-124">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a3359-125">Перечисляет элементы каталога, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="a3359-125">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a3359-126">Связи</span><span class="sxs-lookup"><span data-stu-id="a3359-126">Relationships</span></span>
| <span data-ttu-id="a3359-127">Связь</span><span class="sxs-lookup"><span data-stu-id="a3359-127">Relationship</span></span> | <span data-ttu-id="a3359-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a3359-128">Type</span></span>   |<span data-ttu-id="a3359-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a3359-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3359-130">deleteditems</span><span class="sxs-lookup"><span data-stu-id="a3359-130">deleteditems</span></span>|<span data-ttu-id="a3359-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a3359-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a3359-132">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="a3359-132">Recently deleted items.</span></span> <span data-ttu-id="a3359-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3359-133">Read-only.</span></span> <span data-ttu-id="a3359-134">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a3359-134">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3359-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3359-135">JSON representation</span></span>
<span data-ttu-id="a3359-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3359-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="a3359-137">Пример</span><span class="sxs-lookup"><span data-stu-id="a3359-137">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->