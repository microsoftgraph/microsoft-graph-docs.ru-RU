# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="77a7a-101">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="77a7a-101">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="77a7a-102">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="77a7a-102">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="77a7a-103">Методы</span><span class="sxs-lookup"><span data-stu-id="77a7a-103">Methods</span></span>
<span data-ttu-id="77a7a-104">Нет</span><span class="sxs-lookup"><span data-stu-id="77a7a-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="77a7a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="77a7a-105">Properties</span></span>
<span data-ttu-id="77a7a-106">Нет</span><span class="sxs-lookup"><span data-stu-id="77a7a-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="77a7a-107">Связи</span><span class="sxs-lookup"><span data-stu-id="77a7a-107">Relationships</span></span>
| <span data-ttu-id="77a7a-108">Связь</span><span class="sxs-lookup"><span data-stu-id="77a7a-108">Relationship</span></span> | <span data-ttu-id="77a7a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="77a7a-109">Type</span></span>   |<span data-ttu-id="77a7a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77a7a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77a7a-111">font</span><span class="sxs-lookup"><span data-stu-id="77a7a-111">font</span></span>|[<span data-ttu-id="77a7a-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="77a7a-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="77a7a-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта названия оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77a7a-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77a7a-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77a7a-115">JSON representation</span></span>

<span data-ttu-id="77a7a-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77a7a-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->