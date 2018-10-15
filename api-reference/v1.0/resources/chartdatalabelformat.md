# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="b6389-101">Тип ресурса ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="b6389-101">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="b6389-102">Инкапсулирует свойства формата для меток данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b6389-102">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="b6389-103">Методы</span><span class="sxs-lookup"><span data-stu-id="b6389-103">Methods</span></span>
<span data-ttu-id="b6389-104">Нет</span><span class="sxs-lookup"><span data-stu-id="b6389-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="b6389-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6389-105">Properties</span></span>
<span data-ttu-id="b6389-106">Нет</span><span class="sxs-lookup"><span data-stu-id="b6389-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b6389-107">Связи</span><span class="sxs-lookup"><span data-stu-id="b6389-107">Relationships</span></span>
| <span data-ttu-id="b6389-108">Связь</span><span class="sxs-lookup"><span data-stu-id="b6389-108">Relationship</span></span> | <span data-ttu-id="b6389-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b6389-109">Type</span></span>   |<span data-ttu-id="b6389-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b6389-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6389-111">fill</span><span class="sxs-lookup"><span data-stu-id="b6389-111">fill</span></span>|[<span data-ttu-id="b6389-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="b6389-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="b6389-p101">Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6389-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="b6389-115">font</span><span class="sxs-lookup"><span data-stu-id="b6389-115">font</span></span>|[<span data-ttu-id="b6389-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b6389-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b6389-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6389-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b6389-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6389-119">JSON representation</span></span>

<span data-ttu-id="b6389-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6389-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->