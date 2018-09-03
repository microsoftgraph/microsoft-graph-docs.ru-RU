# <a name="chartareaformat-resource-type"></a><span data-ttu-id="59f39-101">Тип ресурса ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="59f39-101">ChartAreaFormat resource type</span></span>

<span data-ttu-id="59f39-102">Инкапсулирует свойства формата для всей области диаграммы.</span><span class="sxs-lookup"><span data-stu-id="59f39-102">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="59f39-103">Методы</span><span class="sxs-lookup"><span data-stu-id="59f39-103">Methods</span></span>
<span data-ttu-id="59f39-104">Нет</span><span class="sxs-lookup"><span data-stu-id="59f39-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="59f39-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="59f39-105">Properties</span></span>
<span data-ttu-id="59f39-106">Нет</span><span class="sxs-lookup"><span data-stu-id="59f39-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="59f39-107">Связи</span><span class="sxs-lookup"><span data-stu-id="59f39-107">Relationships</span></span>
| <span data-ttu-id="59f39-108">Связь</span><span class="sxs-lookup"><span data-stu-id="59f39-108">Relationship</span></span> | <span data-ttu-id="59f39-109">Тип</span><span class="sxs-lookup"><span data-stu-id="59f39-109">Type</span></span>   |<span data-ttu-id="59f39-110">Описание</span><span class="sxs-lookup"><span data-stu-id="59f39-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59f39-111">fill</span><span class="sxs-lookup"><span data-stu-id="59f39-111">fill</span></span>|[<span data-ttu-id="59f39-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="59f39-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="59f39-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59f39-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="59f39-115">font</span><span class="sxs-lookup"><span data-stu-id="59f39-115">font</span></span>|[<span data-ttu-id="59f39-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="59f39-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="59f39-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для текущего объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="59f39-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59f39-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59f39-119">JSON representation</span></span>

<span data-ttu-id="59f39-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59f39-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
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