# <a name="charttitleformat-resource-type"></a><span data-ttu-id="98186-101">Тип ресурса ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="98186-101">ChartTitleFormat resource type</span></span>

<span data-ttu-id="98186-102">Инкапсулирует свойства формата для заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="98186-102">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="98186-103">Методы</span><span class="sxs-lookup"><span data-stu-id="98186-103">Methods</span></span>
<span data-ttu-id="98186-104">Нет</span><span class="sxs-lookup"><span data-stu-id="98186-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="98186-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="98186-105">Properties</span></span>
<span data-ttu-id="98186-106">Нет</span><span class="sxs-lookup"><span data-stu-id="98186-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="98186-107">Связи</span><span class="sxs-lookup"><span data-stu-id="98186-107">Relationships</span></span>
| <span data-ttu-id="98186-108">Связь</span><span class="sxs-lookup"><span data-stu-id="98186-108">Relationship</span></span> | <span data-ttu-id="98186-109">Тип</span><span class="sxs-lookup"><span data-stu-id="98186-109">Type</span></span>   |<span data-ttu-id="98186-110">Описание</span><span class="sxs-lookup"><span data-stu-id="98186-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98186-111">fill</span><span class="sxs-lookup"><span data-stu-id="98186-111">fill</span></span>|[<span data-ttu-id="98186-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="98186-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="98186-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98186-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="98186-115">font</span><span class="sxs-lookup"><span data-stu-id="98186-115">font</span></span>|[<span data-ttu-id="98186-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="98186-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="98186-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для текущего объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="98186-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="98186-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98186-119">JSON representation</span></span>

<span data-ttu-id="98186-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98186-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
