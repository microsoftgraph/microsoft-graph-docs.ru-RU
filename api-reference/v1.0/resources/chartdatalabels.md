# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="8bbdd-101">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8bbdd-101">ChartDataLabels resource type</span></span>

<span data-ttu-id="8bbdd-102">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-102">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="8bbdd-103">Методы</span><span class="sxs-lookup"><span data-stu-id="8bbdd-103">Methods</span></span>

| <span data-ttu-id="8bbdd-104">Метод</span><span class="sxs-lookup"><span data-stu-id="8bbdd-104">Method</span></span>           | <span data-ttu-id="8bbdd-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8bbdd-105">Return Type</span></span>    |<span data-ttu-id="8bbdd-106">Описание</span><span class="sxs-lookup"><span data-stu-id="8bbdd-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8bbdd-107">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8bbdd-107">Get ChartDataLabels</span></span>](../api/chartdatalabels_get.md) | [<span data-ttu-id="8bbdd-108">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8bbdd-108">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="8bbdd-109">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-109">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="8bbdd-110">Update</span><span class="sxs-lookup"><span data-stu-id="8bbdd-110">Update</span></span>](../api/chartdatalabels_update.md) | [<span data-ttu-id="8bbdd-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8bbdd-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="8bbdd-112">Обновление объекта ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-112">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8bbdd-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bbdd-113">Properties</span></span>
| <span data-ttu-id="8bbdd-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bbdd-114">Property</span></span>     | <span data-ttu-id="8bbdd-115">Тип</span><span class="sxs-lookup"><span data-stu-id="8bbdd-115">Type</span></span>   |<span data-ttu-id="8bbdd-116">Описание</span><span class="sxs-lookup"><span data-stu-id="8bbdd-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bbdd-117">position</span><span class="sxs-lookup"><span data-stu-id="8bbdd-117">position</span></span>|<span data-ttu-id="8bbdd-118">string</span><span class="sxs-lookup"><span data-stu-id="8bbdd-118">string</span></span>|<span data-ttu-id="8bbdd-119">DataLabelPosition значение, представляющее положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-119">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="8bbdd-120">Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-120">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="8bbdd-121">separator</span><span class="sxs-lookup"><span data-stu-id="8bbdd-121">separator</span></span>|<span data-ttu-id="8bbdd-122">string</span><span class="sxs-lookup"><span data-stu-id="8bbdd-122">string</span></span>|<span data-ttu-id="8bbdd-123">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-123">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="8bbdd-124">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="8bbdd-124">showBubbleSize</span></span>|<span data-ttu-id="8bbdd-125">boolean</span><span class="sxs-lookup"><span data-stu-id="8bbdd-125">boolean</span></span>|<span data-ttu-id="8bbdd-126">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-126">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="8bbdd-127">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="8bbdd-127">showCategoryName</span></span>|<span data-ttu-id="8bbdd-128">boolean</span><span class="sxs-lookup"><span data-stu-id="8bbdd-128">boolean</span></span>|<span data-ttu-id="8bbdd-129">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-129">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="8bbdd-130">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="8bbdd-130">showLegendKey</span></span>|<span data-ttu-id="8bbdd-131">boolean</span><span class="sxs-lookup"><span data-stu-id="8bbdd-131">boolean</span></span>|<span data-ttu-id="8bbdd-132">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-132">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="8bbdd-133">showPercentage</span><span class="sxs-lookup"><span data-stu-id="8bbdd-133">showPercentage</span></span>|<span data-ttu-id="8bbdd-134">boolean</span><span class="sxs-lookup"><span data-stu-id="8bbdd-134">boolean</span></span>|<span data-ttu-id="8bbdd-135">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-135">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="8bbdd-136">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="8bbdd-136">showSeriesName</span></span>|<span data-ttu-id="8bbdd-137">boolean</span><span class="sxs-lookup"><span data-stu-id="8bbdd-137">boolean</span></span>|<span data-ttu-id="8bbdd-138">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-138">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="8bbdd-139">showValue</span><span class="sxs-lookup"><span data-stu-id="8bbdd-139">showValue</span></span>|<span data-ttu-id="8bbdd-140">boolean</span><span class="sxs-lookup"><span data-stu-id="8bbdd-140">boolean</span></span>|<span data-ttu-id="8bbdd-141">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-141">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bbdd-142">Связи</span><span class="sxs-lookup"><span data-stu-id="8bbdd-142">Relationships</span></span>
| <span data-ttu-id="8bbdd-143">Связь</span><span class="sxs-lookup"><span data-stu-id="8bbdd-143">Relationship</span></span> | <span data-ttu-id="8bbdd-144">Тип</span><span class="sxs-lookup"><span data-stu-id="8bbdd-144">Type</span></span>   |<span data-ttu-id="8bbdd-145">Описание</span><span class="sxs-lookup"><span data-stu-id="8bbdd-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bbdd-146">format</span><span class="sxs-lookup"><span data-stu-id="8bbdd-146">format</span></span>|[<span data-ttu-id="8bbdd-147">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="8bbdd-147">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="8bbdd-p102">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bbdd-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bbdd-150">JSON representation</span></span>

<span data-ttu-id="8bbdd-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bbdd-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->