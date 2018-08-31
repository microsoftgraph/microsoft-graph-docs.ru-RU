# <a name="directoryobject-resource-type"></a><span data-ttu-id="12db0-101">Тип ресурса directoryObject</span><span class="sxs-lookup"><span data-stu-id="12db0-101">directoryObject resource type</span></span>

<span data-ttu-id="12db0-p101">Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов сущностей каталога.</span><span class="sxs-lookup"><span data-stu-id="12db0-p101">Represents an Azure Active Directory object. The **directoryObject** type is the base type for many other directory entity types.</span></span>

## <a name="methods"></a><span data-ttu-id="12db0-104">Методы</span><span class="sxs-lookup"><span data-stu-id="12db0-104">Methods</span></span>

| <span data-ttu-id="12db0-105">Метод</span><span class="sxs-lookup"><span data-stu-id="12db0-105">Method</span></span>       | <span data-ttu-id="12db0-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12db0-106">Return Type</span></span>  |<span data-ttu-id="12db0-107">Описание</span><span class="sxs-lookup"><span data-stu-id="12db0-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12db0-108">Get directoryObject</span><span class="sxs-lookup"><span data-stu-id="12db0-108">Get directoryObject</span></span>](../api/directoryobject_get.md) | [<span data-ttu-id="12db0-109">directoryObject</span><span class="sxs-lookup"><span data-stu-id="12db0-109">directoryObject</span></span>](directoryobject.md) |<span data-ttu-id="12db0-110">Чтение свойств объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="12db0-110">Read the properties  of a directory object.</span></span>|
|[<span data-ttu-id="12db0-111">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="12db0-111">Delete directoryObject</span></span>](../api/directoryobject_delete.md) | <span data-ttu-id="12db0-112">Нет</span><span class="sxs-lookup"><span data-stu-id="12db0-112">None</span></span> |<span data-ttu-id="12db0-113">Удаление объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="12db0-113">Delete a directory object.</span></span> |
|[<span data-ttu-id="12db0-114">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="12db0-114">checkMemberGroups</span></span>](../api/directoryobject_checkmembergroups.md)|<span data-ttu-id="12db0-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="12db0-115">String collection</span></span>|<span data-ttu-id="12db0-p102">Проверка членства в списке групп. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="12db0-p102">Check for membership in a list of groups. The check is transitive.</span></span>|
|[<span data-ttu-id="12db0-118">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="12db0-118">getMemberGroups</span></span>](../api/directoryobject_getmembergroups.md)|<span data-ttu-id="12db0-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="12db0-119">String collection</span></span>|<span data-ttu-id="12db0-p103">Возвращает все группы, в которых состоит пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="12db0-p103">Return all the groups that the user, group, or directory object is a member of. The check is transitive.</span></span>|
|[<span data-ttu-id="12db0-122">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="12db0-122">getMemberObjects</span></span>](../api/directoryobject_getmemberobjects.md)|<span data-ttu-id="12db0-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="12db0-123">String collection</span></span>| <span data-ttu-id="12db0-p104">Возвращает все группы и роли каталога, участником которых является пользователь, группа или объект каталога. Это транзитивная проверка.</span><span class="sxs-lookup"><span data-stu-id="12db0-p104">Return all of the groups and directory roles that the user, group, or directory object is a member of. The check is transitive.</span></span> |
|[<span data-ttu-id="12db0-126">getByIds</span><span class="sxs-lookup"><span data-stu-id="12db0-126">getByIds</span></span>](../api/directoryobject_getbyids.md) | <span data-ttu-id="12db0-127">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="12db0-127">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="12db0-128">Получение набора объектов каталога на основе указанных идентификаторов.</span><span class="sxs-lookup"><span data-stu-id="12db0-128">Get a set of directory objects based on a set of supplied ids.</span></span> |

## <a name="properties"></a><span data-ttu-id="12db0-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="12db0-129">Properties</span></span>

| <span data-ttu-id="12db0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12db0-130">Property</span></span>   | <span data-ttu-id="12db0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12db0-131">Type</span></span> |<span data-ttu-id="12db0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12db0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12db0-133">id</span><span class="sxs-lookup"><span data-stu-id="12db0-133">id</span></span>|<span data-ttu-id="12db0-134">String (строка)</span><span class="sxs-lookup"><span data-stu-id="12db0-134">String</span></span>|<span data-ttu-id="12db0-p105">Уникальный идентификатор GUID объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db0-p105">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12db0-139">Связи</span><span class="sxs-lookup"><span data-stu-id="12db0-139">Relationships</span></span>

<span data-ttu-id="12db0-140">Нет</span><span class="sxs-lookup"><span data-stu-id="12db0-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="12db0-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12db0-141">JSON representation</span></span>

<span data-ttu-id="12db0-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12db0-142">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
