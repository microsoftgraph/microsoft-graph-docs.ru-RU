# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="207d8-101">Тип ресурса ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="207d8-101">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="207d8-102">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="207d8-102">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="207d8-103">Методы</span><span class="sxs-lookup"><span data-stu-id="207d8-103">Methods</span></span>
<span data-ttu-id="207d8-104">Нет</span><span class="sxs-lookup"><span data-stu-id="207d8-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="207d8-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="207d8-105">Properties</span></span>
<span data-ttu-id="207d8-106">Нет</span><span class="sxs-lookup"><span data-stu-id="207d8-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="207d8-107">Связи</span><span class="sxs-lookup"><span data-stu-id="207d8-107">Relationships</span></span>
| <span data-ttu-id="207d8-108">Связь</span><span class="sxs-lookup"><span data-stu-id="207d8-108">Relationship</span></span> | <span data-ttu-id="207d8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="207d8-109">Type</span></span>   |<span data-ttu-id="207d8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="207d8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="207d8-111">fill</span><span class="sxs-lookup"><span data-stu-id="207d8-111">fill</span></span>|[<span data-ttu-id="207d8-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="207d8-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="207d8-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="207d8-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="207d8-115">line</span><span class="sxs-lookup"><span data-stu-id="207d8-115">line</span></span>|[<span data-ttu-id="207d8-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="207d8-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="207d8-p102">Представляет форматирование линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="207d8-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="207d8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="207d8-119">JSON representation</span></span>

<span data-ttu-id="207d8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="207d8-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->