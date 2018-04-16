# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="12929-101">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="12929-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="12929-102">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="12929-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="12929-103">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="12929-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="12929-104">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="12929-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="12929-105">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="12929-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="12929-106">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="12929-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="12929-107">Методы</span><span class="sxs-lookup"><span data-stu-id="12929-107">Methods</span></span>

| <span data-ttu-id="12929-108">Метод</span><span class="sxs-lookup"><span data-stu-id="12929-108">Method</span></span>         | <span data-ttu-id="12929-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12929-109">Return Type</span></span> | <span data-ttu-id="12929-110">Описание</span><span class="sxs-lookup"><span data-stu-id="12929-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="12929-111">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="12929-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="12929-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="12929-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="12929-113">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="12929-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="12929-114">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="12929-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="12929-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="12929-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="12929-116">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="12929-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="12929-117">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="12929-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="12929-118">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="12929-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="12929-119">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="12929-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="12929-120">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="12929-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="12929-121">None</span><span class="sxs-lookup"><span data-stu-id="12929-121">None</span></span> | <span data-ttu-id="12929-122">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="12929-122">Permanently deletes an item.</span></span> |

## <a name="properties"></a><span data-ttu-id="12929-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="12929-123">Properties</span></span>
| <span data-ttu-id="12929-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="12929-124">Property</span></span>   | <span data-ttu-id="12929-125">Тип</span><span class="sxs-lookup"><span data-stu-id="12929-125">Type</span></span> |<span data-ttu-id="12929-126">Описание</span><span class="sxs-lookup"><span data-stu-id="12929-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12929-127">id</span><span class="sxs-lookup"><span data-stu-id="12929-127">id</span></span>|<span data-ttu-id="12929-128">String</span><span class="sxs-lookup"><span data-stu-id="12929-128">String</span></span>| <span data-ttu-id="12929-129">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="12929-129">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span> <span data-ttu-id="12929-130">Ключ.</span><span class="sxs-lookup"><span data-stu-id="12929-130">Key</span></span> <span data-ttu-id="12929-131">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="12929-131">Not nullable.</span></span> <span data-ttu-id="12929-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12929-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12929-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="12929-133">Relationships</span></span>
| <span data-ttu-id="12929-134">Связь</span><span class="sxs-lookup"><span data-stu-id="12929-134">Relationship</span></span> | <span data-ttu-id="12929-135">Тип</span><span class="sxs-lookup"><span data-stu-id="12929-135">Type</span></span>   |<span data-ttu-id="12929-136">Описание</span><span class="sxs-lookup"><span data-stu-id="12929-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12929-137">deleteditems</span><span class="sxs-lookup"><span data-stu-id="12929-137">deleteditems</span></span>|<span data-ttu-id="12929-138">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="12929-138">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="12929-139">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="12929-139">Recently deleted items.</span></span> <span data-ttu-id="12929-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12929-140">Read-only.</span></span> <span data-ttu-id="12929-141">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="12929-141">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12929-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12929-142">JSON representation</span></span>
<span data-ttu-id="12929-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12929-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
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