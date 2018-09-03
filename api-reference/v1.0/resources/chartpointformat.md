# <a name="chartpointformat-resource-type"></a><span data-ttu-id="d2b57-101">Тип ресурса ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="d2b57-101">ChartPointFormat resource type</span></span>

<span data-ttu-id="d2b57-102">Представляет объект форматирования для точек диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d2b57-102">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="d2b57-103">Методы</span><span class="sxs-lookup"><span data-stu-id="d2b57-103">Methods</span></span>
<span data-ttu-id="d2b57-104">Нет</span><span class="sxs-lookup"><span data-stu-id="d2b57-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="d2b57-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2b57-105">Properties</span></span>
<span data-ttu-id="d2b57-106">Нет</span><span class="sxs-lookup"><span data-stu-id="d2b57-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d2b57-107">Связи</span><span class="sxs-lookup"><span data-stu-id="d2b57-107">Relationships</span></span>
| <span data-ttu-id="d2b57-108">Связь</span><span class="sxs-lookup"><span data-stu-id="d2b57-108">Relationship</span></span> | <span data-ttu-id="d2b57-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d2b57-109">Type</span></span>   |<span data-ttu-id="d2b57-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2b57-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2b57-111">fill</span><span class="sxs-lookup"><span data-stu-id="d2b57-111">fill</span></span>|[<span data-ttu-id="d2b57-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d2b57-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="d2b57-p101">Представляет формат заливки диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2b57-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d2b57-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2b57-115">JSON representation</span></span>

<span data-ttu-id="d2b57-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2b57-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->