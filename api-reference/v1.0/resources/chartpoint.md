# <a name="chartpoint-resource-type"></a><span data-ttu-id="7bed1-101">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="7bed1-101">ChartPoint resource type</span></span>

<span data-ttu-id="7bed1-102">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="7bed1-102">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7bed1-103">Методы</span><span class="sxs-lookup"><span data-stu-id="7bed1-103">Methods</span></span>

| <span data-ttu-id="7bed1-104">Метод</span><span class="sxs-lookup"><span data-stu-id="7bed1-104">Method</span></span>           | <span data-ttu-id="7bed1-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7bed1-105">Return Type</span></span>    |<span data-ttu-id="7bed1-106">Описание</span><span class="sxs-lookup"><span data-stu-id="7bed1-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7bed1-107">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="7bed1-107">Get ChartPoint</span></span>](../api/chartpoint_get.md) | [<span data-ttu-id="7bed1-108">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="7bed1-108">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="7bed1-109">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="7bed1-109">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="7bed1-110">Список</span><span class="sxs-lookup"><span data-stu-id="7bed1-110">List</span></span>](../api/chartpoint_list.md) | <span data-ttu-id="7bed1-111">Коллекция[WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="7bed1-111">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="7bed1-112">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="7bed1-112">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="7bed1-113">ItemAt</span><span class="sxs-lookup"><span data-stu-id="7bed1-113">Itemat</span></span>](../api/chartpointscollection_itemat.md)|[<span data-ttu-id="7bed1-114">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="7bed1-114">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="7bed1-115">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="7bed1-115">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="7bed1-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bed1-116">Properties</span></span>
| <span data-ttu-id="7bed1-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bed1-117">Property</span></span>     | <span data-ttu-id="7bed1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7bed1-118">Type</span></span>   |<span data-ttu-id="7bed1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7bed1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bed1-120">value</span><span class="sxs-lookup"><span data-stu-id="7bed1-120">value</span></span>|<span data-ttu-id="7bed1-121">Json</span><span class="sxs-lookup"><span data-stu-id="7bed1-121">Json</span></span>|<span data-ttu-id="7bed1-p101">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bed1-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="7bed1-124">id</span><span class="sxs-lookup"><span data-stu-id="7bed1-124">id</span></span>|<span data-ttu-id="7bed1-125">строка</span><span class="sxs-lookup"><span data-stu-id="7bed1-125">string</span></span>|<span data-ttu-id="7bed1-126">уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="7bed1-126">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bed1-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="7bed1-127">Relationships</span></span>
| <span data-ttu-id="7bed1-128">Связь</span><span class="sxs-lookup"><span data-stu-id="7bed1-128">Relationship</span></span> | <span data-ttu-id="7bed1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7bed1-129">Type</span></span>   |<span data-ttu-id="7bed1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7bed1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bed1-131">format</span><span class="sxs-lookup"><span data-stu-id="7bed1-131">format</span></span>|[<span data-ttu-id="7bed1-132">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="7bed1-132">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="7bed1-p102">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bed1-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bed1-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bed1-135">JSON representation</span></span>

<span data-ttu-id="7bed1-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bed1-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->