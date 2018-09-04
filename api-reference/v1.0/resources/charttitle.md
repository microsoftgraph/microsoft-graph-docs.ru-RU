# <a name="charttitle-resource-type"></a><span data-ttu-id="d80a3-101">Тип ресурса ChartTitle</span><span class="sxs-lookup"><span data-stu-id="d80a3-101">ChartTitle resource type</span></span>

<span data-ttu-id="d80a3-102">Представляет объект заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d80a3-102">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="d80a3-103">Методы</span><span class="sxs-lookup"><span data-stu-id="d80a3-103">Methods</span></span>

| <span data-ttu-id="d80a3-104">Метод</span><span class="sxs-lookup"><span data-stu-id="d80a3-104">Method</span></span>           | <span data-ttu-id="d80a3-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d80a3-105">Return Type</span></span>    |<span data-ttu-id="d80a3-106">Описание</span><span class="sxs-lookup"><span data-stu-id="d80a3-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d80a3-107">Get ChartTitle</span><span class="sxs-lookup"><span data-stu-id="d80a3-107">Get ChartTitle</span></span>](../api/charttitle_get.md) | [<span data-ttu-id="d80a3-108">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="d80a3-108">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="d80a3-109">Чтение свойств и связей объекта chartTitle.</span><span class="sxs-lookup"><span data-stu-id="d80a3-109">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="d80a3-110">Update</span><span class="sxs-lookup"><span data-stu-id="d80a3-110">Update</span></span>](../api/charttitle_update.md) | [<span data-ttu-id="d80a3-111">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="d80a3-111">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="d80a3-112">Обновление объекта ChartTitle.</span><span class="sxs-lookup"><span data-stu-id="d80a3-112">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d80a3-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="d80a3-113">Properties</span></span>
| <span data-ttu-id="d80a3-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="d80a3-114">Property</span></span>     | <span data-ttu-id="d80a3-115">Тип</span><span class="sxs-lookup"><span data-stu-id="d80a3-115">Type</span></span>   |<span data-ttu-id="d80a3-116">Описание</span><span class="sxs-lookup"><span data-stu-id="d80a3-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d80a3-117">overlay</span><span class="sxs-lookup"><span data-stu-id="d80a3-117">overlay</span></span>|<span data-ttu-id="d80a3-118">boolean</span><span class="sxs-lookup"><span data-stu-id="d80a3-118">boolean</span></span>|<span data-ttu-id="d80a3-119">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="d80a3-119">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="d80a3-120">text</span><span class="sxs-lookup"><span data-stu-id="d80a3-120">text</span></span>|<span data-ttu-id="d80a3-121">string</span><span class="sxs-lookup"><span data-stu-id="d80a3-121">string</span></span>|<span data-ttu-id="d80a3-122">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d80a3-122">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="d80a3-123">visible</span><span class="sxs-lookup"><span data-stu-id="d80a3-123">visible</span></span>|<span data-ttu-id="d80a3-124">boolean</span><span class="sxs-lookup"><span data-stu-id="d80a3-124">boolean</span></span>|<span data-ttu-id="d80a3-125">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d80a3-125">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d80a3-126">Связи</span><span class="sxs-lookup"><span data-stu-id="d80a3-126">Relationships</span></span>
| <span data-ttu-id="d80a3-127">Связь</span><span class="sxs-lookup"><span data-stu-id="d80a3-127">Relationship</span></span> | <span data-ttu-id="d80a3-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d80a3-128">Type</span></span>   |<span data-ttu-id="d80a3-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d80a3-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d80a3-130">format</span><span class="sxs-lookup"><span data-stu-id="d80a3-130">format</span></span>|[<span data-ttu-id="d80a3-131">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="d80a3-131">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="d80a3-p101">Представляет форматирование названия диаграммы, включая формат заливки и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d80a3-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d80a3-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d80a3-134">JSON representation</span></span>

<span data-ttu-id="d80a3-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d80a3-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->