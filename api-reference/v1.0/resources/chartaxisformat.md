# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="41527-101">Тип ресурса ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="41527-101">ChartAxisFormat resource type</span></span>

<span data-ttu-id="41527-102">Инкапсулирует свойства формата для оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="41527-102">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="41527-103">Методы</span><span class="sxs-lookup"><span data-stu-id="41527-103">Methods</span></span>
<span data-ttu-id="41527-104">Нет</span><span class="sxs-lookup"><span data-stu-id="41527-104">None</span></span>
## <a name="properties"></a><span data-ttu-id="41527-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="41527-105">Properties</span></span>
<span data-ttu-id="41527-106">Нет</span><span class="sxs-lookup"><span data-stu-id="41527-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="41527-107">Связи</span><span class="sxs-lookup"><span data-stu-id="41527-107">Relationships</span></span>
| <span data-ttu-id="41527-108">Связь</span><span class="sxs-lookup"><span data-stu-id="41527-108">Relationship</span></span> | <span data-ttu-id="41527-109">Тип</span><span class="sxs-lookup"><span data-stu-id="41527-109">Type</span></span>   |<span data-ttu-id="41527-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41527-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41527-111">font</span><span class="sxs-lookup"><span data-stu-id="41527-111">font</span></span>|[<span data-ttu-id="41527-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="41527-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="41527-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для элемента оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41527-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="41527-115">line</span><span class="sxs-lookup"><span data-stu-id="41527-115">line</span></span>|[<span data-ttu-id="41527-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="41527-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="41527-p102">Представляет форматирование линий диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="41527-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="41527-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41527-119">JSON representation</span></span>

<span data-ttu-id="41527-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41527-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->