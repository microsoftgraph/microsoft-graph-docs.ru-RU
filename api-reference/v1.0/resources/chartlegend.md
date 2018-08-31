# <a name="chartlegend-resource-type"></a><span data-ttu-id="b064e-101">Тип ресурса ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b064e-101">ChartLegend resource type</span></span>

<span data-ttu-id="b064e-102">Представляет легенду в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="b064e-102">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b064e-103">Методы</span><span class="sxs-lookup"><span data-stu-id="b064e-103">Methods</span></span>

| <span data-ttu-id="b064e-104">Метод</span><span class="sxs-lookup"><span data-stu-id="b064e-104">Method</span></span>           | <span data-ttu-id="b064e-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b064e-105">Return Type</span></span>    |<span data-ttu-id="b064e-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b064e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b064e-107">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b064e-107">Get ChartLegend</span></span>](../api/chartlegend_get.md) | [<span data-ttu-id="b064e-108">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="b064e-108">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b064e-109">Чтение свойств и связей объекта chartLegend.</span><span class="sxs-lookup"><span data-stu-id="b064e-109">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="b064e-110">Update</span><span class="sxs-lookup"><span data-stu-id="b064e-110">Update</span></span>](../api/chartlegend_update.md) | [<span data-ttu-id="b064e-111">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="b064e-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b064e-112">Обновление объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="b064e-112">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b064e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="b064e-113">Properties</span></span>
| <span data-ttu-id="b064e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="b064e-114">Property</span></span>     | <span data-ttu-id="b064e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="b064e-115">Type</span></span>   |<span data-ttu-id="b064e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="b064e-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b064e-117">overlay</span><span class="sxs-lookup"><span data-stu-id="b064e-117">overlay</span></span>|<span data-ttu-id="b064e-118">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="b064e-118">boolean</span></span>|<span data-ttu-id="b064e-119">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b064e-119">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="b064e-120">position</span><span class="sxs-lookup"><span data-stu-id="b064e-120">position</span></span>|<span data-ttu-id="b064e-121">string (строка)</span><span class="sxs-lookup"><span data-stu-id="b064e-121">string</span></span>|<span data-ttu-id="b064e-122">Представляет положение условного обозначения диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b064e-122">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="b064e-123">Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`,`Custom`.</span><span class="sxs-lookup"><span data-stu-id="b064e-123">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="b064e-124">visible</span><span class="sxs-lookup"><span data-stu-id="b064e-124">visible</span></span>|<span data-ttu-id="b064e-125">boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="b064e-125">boolean</span></span>|<span data-ttu-id="b064e-126">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="b064e-126">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b064e-127">Связи</span><span class="sxs-lookup"><span data-stu-id="b064e-127">Relationships</span></span>
| <span data-ttu-id="b064e-128">Связь</span><span class="sxs-lookup"><span data-stu-id="b064e-128">Relationship</span></span> | <span data-ttu-id="b064e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b064e-129">Type</span></span>   |<span data-ttu-id="b064e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b064e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b064e-131">format</span><span class="sxs-lookup"><span data-stu-id="b064e-131">format</span></span>|[<span data-ttu-id="b064e-132">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="b064e-132">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="b064e-p102">Представляет форматирование условного обозначения диаграммы, включая заливку и шрифт. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b064e-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b064e-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b064e-135">JSON representation</span></span>

<span data-ttu-id="b064e-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b064e-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->