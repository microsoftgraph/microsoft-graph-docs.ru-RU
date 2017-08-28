# <a name="nameditem-resource-type"></a><span data-ttu-id="e2ec8-101">Тип ресурса NamedItem</span><span class="sxs-lookup"><span data-stu-id="e2ec8-101">NamedItem resource type</span></span>

<span data-ttu-id="e2ec8-p101">Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="e2ec8-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e2ec8-105">Methods</span></span>

| <span data-ttu-id="e2ec8-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e2ec8-106">Method</span></span>           | <span data-ttu-id="e2ec8-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e2ec8-107">Return Type</span></span>    |<span data-ttu-id="e2ec8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ec8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e2ec8-109">Add</span><span class="sxs-lookup"><span data-stu-id="e2ec8-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="e2ec8-110">NamedItem</span><span class="sxs-lookup"><span data-stu-id="e2ec8-110">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="e2ec8-111">Добавляет новое имя в определенную коллекцию.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="e2ec8-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="e2ec8-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="e2ec8-113">NamedItem</span><span class="sxs-lookup"><span data-stu-id="e2ec8-113">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="e2ec8-114">Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="e2ec8-115">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="e2ec8-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="e2ec8-116">NamedItem</span><span class="sxs-lookup"><span data-stu-id="e2ec8-116">NamedItem</span></span>](nameditem.md) |<span data-ttu-id="e2ec8-117">Чтение свойств и связей объекта namedItem.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="e2ec8-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="e2ec8-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="e2ec8-119">NamedItem</span><span class="sxs-lookup"><span data-stu-id="e2ec8-119">NamedItem</span></span>](nameditem.md)   |<span data-ttu-id="e2ec8-120">Обновление объекта NamedItem.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="e2ec8-121">Range</span><span class="sxs-lookup"><span data-stu-id="e2ec8-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="e2ec8-122">Range</span><span class="sxs-lookup"><span data-stu-id="e2ec8-122">Range</span></span>](range.md)|<span data-ttu-id="e2ec8-p102">Возвращает объект диапазона, связанный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="e2ec8-125">Список</span><span class="sxs-lookup"><span data-stu-id="e2ec8-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="e2ec8-126">Коллекция объектов [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="e2ec8-126">[NamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="e2ec8-127">Получение коллекции объектов namedItem.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="e2ec8-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2ec8-128">Properties</span></span>
| <span data-ttu-id="e2ec8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2ec8-129">Property</span></span>     | <span data-ttu-id="e2ec8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e2ec8-130">Type</span></span>   |<span data-ttu-id="e2ec8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ec8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2ec8-132">name</span><span class="sxs-lookup"><span data-stu-id="e2ec8-132">name</span></span>|<span data-ttu-id="e2ec8-133">string</span><span class="sxs-lookup"><span data-stu-id="e2ec8-133">string</span></span>|<span data-ttu-id="e2ec8-p103">Имя объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="e2ec8-136">comment</span><span class="sxs-lookup"><span data-stu-id="e2ec8-136">comment</span></span>|<span data-ttu-id="e2ec8-137">строка</span><span class="sxs-lookup"><span data-stu-id="e2ec8-137">string</span></span>|<span data-ttu-id="e2ec8-138">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="e2ec8-139">scope</span><span class="sxs-lookup"><span data-stu-id="e2ec8-139">scope</span></span>|<span data-ttu-id="e2ec8-140">string</span><span class="sxs-lookup"><span data-stu-id="e2ec8-140">string</span></span>|<span data-ttu-id="e2ec8-p104">Указывает, относится ли имя к книге или определенному листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="e2ec8-143">type</span><span class="sxs-lookup"><span data-stu-id="e2ec8-143">type</span></span>|<span data-ttu-id="e2ec8-144">string</span><span class="sxs-lookup"><span data-stu-id="e2ec8-144">string</span></span>|<span data-ttu-id="e2ec8-p105">Указывает тип ссылки, связанный с именем. Возможные значения: `String`, `Integer`, `Double`, `Boolean`, `Range`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-p105">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="e2ec8-148">value</span><span class="sxs-lookup"><span data-stu-id="e2ec8-148">value</span></span>|<span data-ttu-id="e2ec8-149">object</span><span class="sxs-lookup"><span data-stu-id="e2ec8-149">object</span></span>|<span data-ttu-id="e2ec8-p106">Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4,75 и т. д. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="e2ec8-153">visible</span><span class="sxs-lookup"><span data-stu-id="e2ec8-153">visible</span></span>|<span data-ttu-id="e2ec8-154">boolean</span><span class="sxs-lookup"><span data-stu-id="e2ec8-154">boolean</span></span>|<span data-ttu-id="e2ec8-155">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ec8-156">Связи</span><span class="sxs-lookup"><span data-stu-id="e2ec8-156">Relationships</span></span>
| <span data-ttu-id="e2ec8-157">Связь</span><span class="sxs-lookup"><span data-stu-id="e2ec8-157">Relationship</span></span>     | <span data-ttu-id="e2ec8-158">Тип</span><span class="sxs-lookup"><span data-stu-id="e2ec8-158">Type</span></span>   |<span data-ttu-id="e2ec8-159">Описание</span><span class="sxs-lookup"><span data-stu-id="e2ec8-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2ec8-160">worksheet</span><span class="sxs-lookup"><span data-stu-id="e2ec8-160">worksheet</span></span>|[<span data-ttu-id="e2ec8-161">worksheet</span><span class="sxs-lookup"><span data-stu-id="e2ec8-161">worksheet</span></span>](worksheet.md)|<span data-ttu-id="e2ec8-p107">Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2ec8-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2ec8-165">JSON representation</span></span>

<span data-ttu-id="e2ec8-166">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2ec8-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.range"},
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
