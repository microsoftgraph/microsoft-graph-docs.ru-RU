# <a name="chartaxes-resource-type"></a><span data-ttu-id="b8bdb-101">Тип ресурса ChartAxes</span><span class="sxs-lookup"><span data-stu-id="b8bdb-101">ChartAxes resource type</span></span>

<span data-ttu-id="b8bdb-102">Представляет оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b8bdb-102">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="b8bdb-103">Методы</span><span class="sxs-lookup"><span data-stu-id="b8bdb-103">Methods</span></span>
<span data-ttu-id="b8bdb-104">Нет</span><span class="sxs-lookup"><span data-stu-id="b8bdb-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="b8bdb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8bdb-105">Properties</span></span>
<span data-ttu-id="b8bdb-106">Нет</span><span class="sxs-lookup"><span data-stu-id="b8bdb-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b8bdb-107">Связи</span><span class="sxs-lookup"><span data-stu-id="b8bdb-107">Relationships</span></span>
| <span data-ttu-id="b8bdb-108">Связь</span><span class="sxs-lookup"><span data-stu-id="b8bdb-108">Relationship</span></span> | <span data-ttu-id="b8bdb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8bdb-109">Type</span></span>   |<span data-ttu-id="b8bdb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8bdb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8bdb-111">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="b8bdb-111">categoryAxis</span></span>|[<span data-ttu-id="b8bdb-112">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="b8bdb-112">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="b8bdb-p101">Представляет ось категорий на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8bdb-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="b8bdb-115">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="b8bdb-115">seriesAxis</span></span>|[<span data-ttu-id="b8bdb-116">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="b8bdb-116">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="b8bdb-p102">Представляет ось ряда данных для объемной диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8bdb-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="b8bdb-119">valueAxis</span><span class="sxs-lookup"><span data-stu-id="b8bdb-119">valueAxis</span></span>|[<span data-ttu-id="b8bdb-120">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="b8bdb-120">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="b8bdb-p103">Представляет ось значений для оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8bdb-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8bdb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8bdb-123">JSON representation</span></span>

<span data-ttu-id="b8bdb-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8bdb-124">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->