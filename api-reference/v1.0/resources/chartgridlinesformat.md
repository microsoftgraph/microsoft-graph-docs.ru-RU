# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="c5d48-101">Тип ресурса ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="c5d48-101">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="c5d48-102">Инкапсулирует свойства формата для линий сетки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c5d48-102">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="c5d48-103">Методы</span><span class="sxs-lookup"><span data-stu-id="c5d48-103">Methods</span></span>
<span data-ttu-id="c5d48-104">Нет</span><span class="sxs-lookup"><span data-stu-id="c5d48-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="c5d48-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c5d48-105">Properties</span></span>
<span data-ttu-id="c5d48-106">Нет</span><span class="sxs-lookup"><span data-stu-id="c5d48-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c5d48-107">Связи</span><span class="sxs-lookup"><span data-stu-id="c5d48-107">Relationships</span></span>
| <span data-ttu-id="c5d48-108">Связь</span><span class="sxs-lookup"><span data-stu-id="c5d48-108">Relationship</span></span> | <span data-ttu-id="c5d48-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c5d48-109">Type</span></span>   |<span data-ttu-id="c5d48-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c5d48-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5d48-111">line</span><span class="sxs-lookup"><span data-stu-id="c5d48-111">line</span></span>|[<span data-ttu-id="c5d48-112">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="c5d48-112">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="c5d48-p101">Представляет форматирование линий диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c5d48-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c5d48-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c5d48-115">JSON representation</span></span>

<span data-ttu-id="c5d48-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5d48-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->