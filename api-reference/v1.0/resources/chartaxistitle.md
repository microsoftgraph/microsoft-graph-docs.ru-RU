# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="7195b-101">Тип ресурса ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="7195b-101">ChartAxisTitle resource type</span></span>

<span data-ttu-id="7195b-102">Представляет название оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7195b-102">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="7195b-103">Методы</span><span class="sxs-lookup"><span data-stu-id="7195b-103">Methods</span></span>

| <span data-ttu-id="7195b-104">Метод</span><span class="sxs-lookup"><span data-stu-id="7195b-104">Method</span></span>           | <span data-ttu-id="7195b-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7195b-105">Return Type</span></span>    |<span data-ttu-id="7195b-106">Описание</span><span class="sxs-lookup"><span data-stu-id="7195b-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7195b-107">Получение объекта ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="7195b-107">Get ChartAxisTitle</span></span>](../api/chartaxistitle_get.md) | [<span data-ttu-id="7195b-108">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="7195b-108">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="7195b-109">Чтение свойств и связей объекта chartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="7195b-109">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="7195b-110">Обновление</span><span class="sxs-lookup"><span data-stu-id="7195b-110">Update</span></span>](../api/chartaxistitle_update.md) | [<span data-ttu-id="7195b-111">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="7195b-111">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="7195b-112">Обновление объекта ChartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="7195b-112">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7195b-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="7195b-113">Properties</span></span>
| <span data-ttu-id="7195b-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="7195b-114">Property</span></span>     | <span data-ttu-id="7195b-115">Тип</span><span class="sxs-lookup"><span data-stu-id="7195b-115">Type</span></span>   |<span data-ttu-id="7195b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="7195b-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7195b-117">text</span><span class="sxs-lookup"><span data-stu-id="7195b-117">text</span></span>|<span data-ttu-id="7195b-118">строка</span><span class="sxs-lookup"><span data-stu-id="7195b-118">string</span></span>|<span data-ttu-id="7195b-119">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="7195b-119">Represents the axis title.</span></span>|
|<span data-ttu-id="7195b-120">visible</span><span class="sxs-lookup"><span data-stu-id="7195b-120">visible</span></span>|<span data-ttu-id="7195b-121">boolean</span><span class="sxs-lookup"><span data-stu-id="7195b-121">boolean</span></span>|<span data-ttu-id="7195b-122">Логическое значение, которое определяет видимость названия оси.</span><span class="sxs-lookup"><span data-stu-id="7195b-122">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7195b-123">Связи</span><span class="sxs-lookup"><span data-stu-id="7195b-123">Relationships</span></span>
| <span data-ttu-id="7195b-124">Связь</span><span class="sxs-lookup"><span data-stu-id="7195b-124">Relationship</span></span> | <span data-ttu-id="7195b-125">Тип</span><span class="sxs-lookup"><span data-stu-id="7195b-125">Type</span></span>   |<span data-ttu-id="7195b-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7195b-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7195b-127">format</span><span class="sxs-lookup"><span data-stu-id="7195b-127">format</span></span>|[<span data-ttu-id="7195b-128">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="7195b-128">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="7195b-p101">Представляет форматирование для названия оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7195b-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7195b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7195b-131">JSON representation</span></span>

<span data-ttu-id="7195b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7195b-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->