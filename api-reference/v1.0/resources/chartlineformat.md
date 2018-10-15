# <a name="chartlineformat-resource-type"></a><span data-ttu-id="b830e-101">Тип ресурса ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b830e-101">ChartLineFormat resource type</span></span>

<span data-ttu-id="b830e-102">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="b830e-102">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="b830e-103">Методы</span><span class="sxs-lookup"><span data-stu-id="b830e-103">Methods</span></span>

| <span data-ttu-id="b830e-104">Метод</span><span class="sxs-lookup"><span data-stu-id="b830e-104">Method</span></span>           | <span data-ttu-id="b830e-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b830e-105">Return Type</span></span>    |<span data-ttu-id="b830e-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b830e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b830e-107">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b830e-107">Get ChartLineFormat</span></span>](../api/chartlineformat_get.md) | [<span data-ttu-id="b830e-108">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b830e-108">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="b830e-109">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="b830e-109">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="b830e-110">Update</span><span class="sxs-lookup"><span data-stu-id="b830e-110">Update</span></span>](../api/chartlineformat_update.md) | [<span data-ttu-id="b830e-111">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b830e-111">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="b830e-112">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="b830e-112">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="b830e-113">Clear</span><span class="sxs-lookup"><span data-stu-id="b830e-113">Clear</span></span>](../api/chartlineformat_clear.md)|<span data-ttu-id="b830e-114">Нет</span><span class="sxs-lookup"><span data-stu-id="b830e-114">None</span></span>|<span data-ttu-id="b830e-115">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b830e-115">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="b830e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="b830e-116">Properties</span></span>
| <span data-ttu-id="b830e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="b830e-117">Property</span></span>     | <span data-ttu-id="b830e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="b830e-118">Type</span></span>   |<span data-ttu-id="b830e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b830e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b830e-120">color</span><span class="sxs-lookup"><span data-stu-id="b830e-120">color</span></span>|<span data-ttu-id="b830e-121">string</span><span class="sxs-lookup"><span data-stu-id="b830e-121">string</span></span>|<span data-ttu-id="b830e-122">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="b830e-122">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b830e-123">Связи</span><span class="sxs-lookup"><span data-stu-id="b830e-123">Relationships</span></span>
<span data-ttu-id="b830e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="b830e-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b830e-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b830e-125">JSON representation</span></span>

<span data-ttu-id="b830e-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b830e-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->