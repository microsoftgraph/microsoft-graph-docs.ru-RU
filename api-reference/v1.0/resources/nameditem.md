# <a name="nameditem-resource-type"></a><span data-ttu-id="6ef9c-101">Тип ресурса NamedItem</span><span class="sxs-lookup"><span data-stu-id="6ef9c-101">NamedItem resource type</span></span>

<span data-ttu-id="6ef9c-p101">Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="6ef9c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6ef9c-105">Methods</span></span>

| <span data-ttu-id="6ef9c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6ef9c-106">Method</span></span>           | <span data-ttu-id="6ef9c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6ef9c-107">Return Type</span></span>    |<span data-ttu-id="6ef9c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef9c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ef9c-109">Add</span><span class="sxs-lookup"><span data-stu-id="6ef9c-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="6ef9c-110">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="6ef9c-110">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="6ef9c-111">Добавляет новое имя в коллекцию данной области.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="6ef9c-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="6ef9c-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="6ef9c-113">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="6ef9c-113">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="6ef9c-114">Добавляет новое имя в коллекцию данной области, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="6ef9c-115">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="6ef9c-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="6ef9c-116">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="6ef9c-116">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="6ef9c-117">Чтение свойств и связей объекта namedItem.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="6ef9c-118">Update</span><span class="sxs-lookup"><span data-stu-id="6ef9c-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="6ef9c-119">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="6ef9c-119">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="6ef9c-120">Обновление объекта NamedItem.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="6ef9c-121">Range</span><span class="sxs-lookup"><span data-stu-id="6ef9c-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="6ef9c-122">Range</span><span class="sxs-lookup"><span data-stu-id="6ef9c-122">Range</span></span>](range.md)|<span data-ttu-id="6ef9c-p102">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="6ef9c-125">List</span><span class="sxs-lookup"><span data-stu-id="6ef9c-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="6ef9c-126">Коллекция [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="6ef9c-126">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="6ef9c-127">Получение коллекции объектов namedItem.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="6ef9c-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ef9c-128">Properties</span></span>
| <span data-ttu-id="6ef9c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ef9c-129">Property</span></span>     | <span data-ttu-id="6ef9c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6ef9c-130">Type</span></span>   |<span data-ttu-id="6ef9c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef9c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ef9c-132">name</span><span class="sxs-lookup"><span data-stu-id="6ef9c-132">name</span></span>|<span data-ttu-id="6ef9c-133">string</span><span class="sxs-lookup"><span data-stu-id="6ef9c-133">string</span></span>|<span data-ttu-id="6ef9c-p103">Имя объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="6ef9c-136">comment</span><span class="sxs-lookup"><span data-stu-id="6ef9c-136">comment</span></span>|<span data-ttu-id="6ef9c-137">string</span><span class="sxs-lookup"><span data-stu-id="6ef9c-137">string</span></span>|<span data-ttu-id="6ef9c-138">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="6ef9c-139">scope</span><span class="sxs-lookup"><span data-stu-id="6ef9c-139">scope</span></span>|<span data-ttu-id="6ef9c-140">string</span><span class="sxs-lookup"><span data-stu-id="6ef9c-140">string</span></span>|<span data-ttu-id="6ef9c-p104">Указывает, относится ли имя к книге или определенному листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="6ef9c-143">type</span><span class="sxs-lookup"><span data-stu-id="6ef9c-143">type</span></span>|<span data-ttu-id="6ef9c-144">string</span><span class="sxs-lookup"><span data-stu-id="6ef9c-144">string</span></span>|<span data-ttu-id="6ef9c-145">Указывает, какой тип ссылки связан с именем.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-145">Indicates what type of reference is associated with the name. Possible values are: , , , , . Read-only.</span></span> <span data-ttu-id="6ef9c-146">Возможные значения: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-146">The possible values are `String`, `Integer`, `Double`, `Boolean`, `Range`, , , , , , , or .</span></span> <span data-ttu-id="6ef9c-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-147">Read-only.</span></span>|
|<span data-ttu-id="6ef9c-148">value</span><span class="sxs-lookup"><span data-stu-id="6ef9c-148">value</span></span>|<span data-ttu-id="6ef9c-149">Json</span><span class="sxs-lookup"><span data-stu-id="6ef9c-149">Json</span></span>|<span data-ttu-id="6ef9c-p106">Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4.75 и т. д. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="6ef9c-153">visible</span><span class="sxs-lookup"><span data-stu-id="6ef9c-153">visible</span></span>|<span data-ttu-id="6ef9c-154">boolean</span><span class="sxs-lookup"><span data-stu-id="6ef9c-154">boolean</span></span>|<span data-ttu-id="6ef9c-155">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ef9c-156">Связи</span><span class="sxs-lookup"><span data-stu-id="6ef9c-156">Relationships</span></span>
| <span data-ttu-id="6ef9c-157">Связь</span><span class="sxs-lookup"><span data-stu-id="6ef9c-157">Relationship</span></span>     | <span data-ttu-id="6ef9c-158">Тип</span><span class="sxs-lookup"><span data-stu-id="6ef9c-158">Type</span></span>   |<span data-ttu-id="6ef9c-159">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef9c-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ef9c-160">worksheet</span><span class="sxs-lookup"><span data-stu-id="6ef9c-160">worksheet</span></span>|[<span data-ttu-id="6ef9c-161">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="6ef9c-161">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="6ef9c-p107">Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ef9c-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ef9c-165">JSON representation</span></span>

<span data-ttu-id="6ef9c-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ef9c-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
