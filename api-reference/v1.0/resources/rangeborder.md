# <a name="rangeborder-resource-type"></a><span data-ttu-id="78d24-101">Тип ресурса RangeBorder</span><span class="sxs-lookup"><span data-stu-id="78d24-101">RangeBorder resource type</span></span>

<span data-ttu-id="78d24-102">Представляет границу объекта.</span><span class="sxs-lookup"><span data-stu-id="78d24-102">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="78d24-103">Методы</span><span class="sxs-lookup"><span data-stu-id="78d24-103">Methods</span></span>

| <span data-ttu-id="78d24-104">Метод</span><span class="sxs-lookup"><span data-stu-id="78d24-104">Method</span></span>           | <span data-ttu-id="78d24-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78d24-105">Return Type</span></span>    |<span data-ttu-id="78d24-106">Описание</span><span class="sxs-lookup"><span data-stu-id="78d24-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78d24-107">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="78d24-107">Get RangeBorder</span></span>](../api/rangeborder_get.md) | [<span data-ttu-id="78d24-108">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="78d24-108">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="78d24-109">Чтение свойств и связей объекта rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="78d24-109">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="78d24-110">Update</span><span class="sxs-lookup"><span data-stu-id="78d24-110">Update</span></span>](../api/rangeborder_update.md) | [<span data-ttu-id="78d24-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="78d24-111">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="78d24-112">Обновление объекта RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="78d24-112">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="78d24-113">List</span><span class="sxs-lookup"><span data-stu-id="78d24-113">List</span></span>](../api/rangeborder_list.md) | <span data-ttu-id="78d24-114">Коллекция [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="78d24-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="78d24-115">Получение коллекции объектов rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="78d24-115">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="78d24-116">Itemat</span><span class="sxs-lookup"><span data-stu-id="78d24-116">Itemat</span></span>](../api/rangebordercollection_itemat.md)|[<span data-ttu-id="78d24-117">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="78d24-117">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="78d24-118">Возвращает объект границы по его индексу.</span><span class="sxs-lookup"><span data-stu-id="78d24-118">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="78d24-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="78d24-119">Properties</span></span>
| <span data-ttu-id="78d24-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="78d24-120">Property</span></span>     | <span data-ttu-id="78d24-121">Тип</span><span class="sxs-lookup"><span data-stu-id="78d24-121">Type</span></span>   |<span data-ttu-id="78d24-122">Описание</span><span class="sxs-lookup"><span data-stu-id="78d24-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78d24-123">color</span><span class="sxs-lookup"><span data-stu-id="78d24-123">color</span></span>|<span data-ttu-id="78d24-124">string (строка)</span><span class="sxs-lookup"><span data-stu-id="78d24-124">string</span></span>|<span data-ttu-id="78d24-125">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="78d24-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="78d24-126">id</span><span class="sxs-lookup"><span data-stu-id="78d24-126">id</span></span>|<span data-ttu-id="78d24-127">string (строка)</span><span class="sxs-lookup"><span data-stu-id="78d24-127">string</span></span>|<span data-ttu-id="78d24-128">Представляет идентификатор границы.</span><span class="sxs-lookup"><span data-stu-id="78d24-128">Represents border identifier. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="78d24-129">Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="78d24-129">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="78d24-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78d24-130">Read-only.</span></span>|
|<span data-ttu-id="78d24-131">sideIndex</span><span class="sxs-lookup"><span data-stu-id="78d24-131">sideIndex</span></span>|<span data-ttu-id="78d24-132">string (строка)</span><span class="sxs-lookup"><span data-stu-id="78d24-132">string</span></span>|<span data-ttu-id="78d24-133">Постоянное значение, указывающее определенную сторону границы.</span><span class="sxs-lookup"><span data-stu-id="78d24-133">Constant value that indicates the specific side of the border. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="78d24-134">Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="78d24-134">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="78d24-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78d24-135">Read-only.</span></span>|
|<span data-ttu-id="78d24-136">style</span><span class="sxs-lookup"><span data-stu-id="78d24-136">style</span></span>|<span data-ttu-id="78d24-137">string (строка)</span><span class="sxs-lookup"><span data-stu-id="78d24-137">string</span></span>|<span data-ttu-id="78d24-138">Одна из констант типа линии, определяющая тип линии границы.</span><span class="sxs-lookup"><span data-stu-id="78d24-138">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="78d24-139">Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="78d24-139">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="78d24-140">weight</span><span class="sxs-lookup"><span data-stu-id="78d24-140">weight</span></span>|<span data-ttu-id="78d24-141">string (строка)</span><span class="sxs-lookup"><span data-stu-id="78d24-141">string</span></span>|<span data-ttu-id="78d24-142">Задает толщину границы в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="78d24-142">Specifies the weight of the border around a range. Possible values are: , , , .</span></span> <span data-ttu-id="78d24-143">Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="78d24-143">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="78d24-144">Связи</span><span class="sxs-lookup"><span data-stu-id="78d24-144">Relationships</span></span>
<span data-ttu-id="78d24-145">Нет</span><span class="sxs-lookup"><span data-stu-id="78d24-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="78d24-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78d24-146">JSON representation</span></span>

<span data-ttu-id="78d24-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78d24-147">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->