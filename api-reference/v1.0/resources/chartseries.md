# <a name="chartseries-resource-type"></a><span data-ttu-id="a8ff0-101">Тип ресурса ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a8ff0-101">ChartSeries resource type</span></span>

<span data-ttu-id="a8ff0-102">Представляет ряд в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-102">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="a8ff0-103">Методы</span><span class="sxs-lookup"><span data-stu-id="a8ff0-103">Methods</span></span>

| <span data-ttu-id="a8ff0-104">Метод</span><span class="sxs-lookup"><span data-stu-id="a8ff0-104">Method</span></span>           | <span data-ttu-id="a8ff0-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8ff0-105">Return Type</span></span>    |<span data-ttu-id="a8ff0-106">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ff0-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8ff0-107">Получение объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a8ff0-107">Get ChartSeries</span></span>](../api/chartseries_get.md) | [<span data-ttu-id="a8ff0-108">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="a8ff0-108">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a8ff0-109">Чтение свойств и связей объекта chartSeries.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-109">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="a8ff0-110">Создание объекта ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a8ff0-110">Create ChartPoints</span></span>](../api/chartseries_post_points.md) |[<span data-ttu-id="a8ff0-111">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a8ff0-111">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="a8ff0-112">Создание объекта ChartPoints путем добавления в коллекцию точек.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-112">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="a8ff0-113">Список точек</span><span class="sxs-lookup"><span data-stu-id="a8ff0-113">List points</span></span>](../api/chartseries_list_points.md) |<span data-ttu-id="a8ff0-114">Коллекция объектов [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="a8ff0-114">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="a8ff0-115">Получение коллекции объектов ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-115">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="a8ff0-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="a8ff0-116">Update</span></span>](../api/chartseries_update.md) | [<span data-ttu-id="a8ff0-117">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="a8ff0-117">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a8ff0-118">Обновление объекта ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-118">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="a8ff0-119">Список</span><span class="sxs-lookup"><span data-stu-id="a8ff0-119">List</span></span>](../api/chartseries_list.md) | <span data-ttu-id="a8ff0-120">Коллекция [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="a8ff0-120">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="a8ff0-121">Получение коллекции объектов chartSeries.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-121">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="a8ff0-122">ItemAt</span><span class="sxs-lookup"><span data-stu-id="a8ff0-122">Itemat</span></span>](../api/chartseriescollection_itemat.md)|[<span data-ttu-id="a8ff0-123">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="a8ff0-123">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="a8ff0-124">Возвращает ряд на основании сведений о его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-124">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="a8ff0-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8ff0-125">Properties</span></span>
| <span data-ttu-id="a8ff0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8ff0-126">Property</span></span>     | <span data-ttu-id="a8ff0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a8ff0-127">Type</span></span>   |<span data-ttu-id="a8ff0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ff0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8ff0-129">name</span><span class="sxs-lookup"><span data-stu-id="a8ff0-129">name</span></span>|<span data-ttu-id="a8ff0-130">string (строка)</span><span class="sxs-lookup"><span data-stu-id="a8ff0-130">string</span></span>|<span data-ttu-id="a8ff0-131">Представляет имя ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-131">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8ff0-132">Связи</span><span class="sxs-lookup"><span data-stu-id="a8ff0-132">Relationships</span></span>
| <span data-ttu-id="a8ff0-133">Связь</span><span class="sxs-lookup"><span data-stu-id="a8ff0-133">Relationship</span></span> | <span data-ttu-id="a8ff0-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a8ff0-134">Type</span></span>   |<span data-ttu-id="a8ff0-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ff0-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8ff0-136">format</span><span class="sxs-lookup"><span data-stu-id="a8ff0-136">format</span></span>|[<span data-ttu-id="a8ff0-137">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="a8ff0-137">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="a8ff0-p101">Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="a8ff0-140">points</span><span class="sxs-lookup"><span data-stu-id="a8ff0-140">points</span></span>|<span data-ttu-id="a8ff0-141">Коллекция [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="a8ff0-141">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="a8ff0-p102">Представляет коллекцию всех точек в ряду. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8ff0-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8ff0-144">JSON representation</span></span>

<span data-ttu-id="a8ff0-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8ff0-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->