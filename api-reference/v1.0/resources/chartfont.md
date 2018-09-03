# <a name="chartfont-resource-type"></a><span data-ttu-id="82820-101">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="82820-101">ChartFont resource type</span></span>

<span data-ttu-id="82820-102">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="82820-102">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="82820-103">Методы</span><span class="sxs-lookup"><span data-stu-id="82820-103">Methods</span></span>

| <span data-ttu-id="82820-104">Метод</span><span class="sxs-lookup"><span data-stu-id="82820-104">Method</span></span>           | <span data-ttu-id="82820-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="82820-105">Return Type</span></span>    |<span data-ttu-id="82820-106">Описание</span><span class="sxs-lookup"><span data-stu-id="82820-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82820-107">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="82820-107">Get ChartFont</span></span>](../api/chartfont_get.md) | [<span data-ttu-id="82820-108">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="82820-108">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="82820-109">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="82820-109">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="82820-110">Update</span><span class="sxs-lookup"><span data-stu-id="82820-110">Update</span></span>](../api/chartfont_update.md) | [<span data-ttu-id="82820-111">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="82820-111">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="82820-112">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="82820-112">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="82820-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="82820-113">Properties</span></span>
| <span data-ttu-id="82820-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="82820-114">Property</span></span>     | <span data-ttu-id="82820-115">Тип</span><span class="sxs-lookup"><span data-stu-id="82820-115">Type</span></span>   |<span data-ttu-id="82820-116">Описание</span><span class="sxs-lookup"><span data-stu-id="82820-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82820-117">bold</span><span class="sxs-lookup"><span data-stu-id="82820-117">bold</span></span>|<span data-ttu-id="82820-118">boolean</span><span class="sxs-lookup"><span data-stu-id="82820-118">boolean</span></span>|<span data-ttu-id="82820-119">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="82820-119">Represents the bold status of font.</span></span>|
|<span data-ttu-id="82820-120">color</span><span class="sxs-lookup"><span data-stu-id="82820-120">color</span></span>|<span data-ttu-id="82820-121">string</span><span class="sxs-lookup"><span data-stu-id="82820-121">string</span></span>|<span data-ttu-id="82820-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="82820-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="82820-125">italic</span><span class="sxs-lookup"><span data-stu-id="82820-125">italic</span></span>|<span data-ttu-id="82820-126">boolean</span><span class="sxs-lookup"><span data-stu-id="82820-126">boolean</span></span>|<span data-ttu-id="82820-127">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="82820-127">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="82820-128">name</span><span class="sxs-lookup"><span data-stu-id="82820-128">name</span></span>|<span data-ttu-id="82820-129">string</span><span class="sxs-lookup"><span data-stu-id="82820-129">string</span></span>|<span data-ttu-id="82820-130">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="82820-130">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="82820-131">size</span><span class="sxs-lookup"><span data-stu-id="82820-131">size</span></span>|<span data-ttu-id="82820-132">Double</span><span class="sxs-lookup"><span data-stu-id="82820-132">double</span></span>|<span data-ttu-id="82820-133">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="82820-133">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="82820-134">underline</span><span class="sxs-lookup"><span data-stu-id="82820-134">underline</span></span>|<span data-ttu-id="82820-135">string</span><span class="sxs-lookup"><span data-stu-id="82820-135">string</span></span>|<span data-ttu-id="82820-136">Тип подчеркивания, применяемый к шрифту.</span><span class="sxs-lookup"><span data-stu-id="82820-136">Type of underline applied to the font. Possible values are: , .</span></span> <span data-ttu-id="82820-137">Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="82820-137">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="82820-138">Связи</span><span class="sxs-lookup"><span data-stu-id="82820-138">Relationships</span></span>
<span data-ttu-id="82820-139">Нет</span><span class="sxs-lookup"><span data-stu-id="82820-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="82820-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="82820-140">JSON representation</span></span>

<span data-ttu-id="82820-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82820-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->