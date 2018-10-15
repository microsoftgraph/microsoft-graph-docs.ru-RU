# <a name="chartaxis-resource-type"></a><span data-ttu-id="636dc-101">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="636dc-101">ChartAxis resource type</span></span>

<span data-ttu-id="636dc-102">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="636dc-102">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="636dc-103">Методы</span><span class="sxs-lookup"><span data-stu-id="636dc-103">Methods</span></span>

| <span data-ttu-id="636dc-104">Метод</span><span class="sxs-lookup"><span data-stu-id="636dc-104">Method</span></span>           | <span data-ttu-id="636dc-105">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="636dc-105">Return Type</span></span>    |<span data-ttu-id="636dc-106">Описание</span><span class="sxs-lookup"><span data-stu-id="636dc-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="636dc-107">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="636dc-107">Get ChartAxis</span></span>](../api/chartaxis_get.md) | [<span data-ttu-id="636dc-108">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="636dc-108">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="636dc-109">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="636dc-109">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="636dc-110">Update</span><span class="sxs-lookup"><span data-stu-id="636dc-110">Update</span></span>](../api/chartaxis_update.md) | [<span data-ttu-id="636dc-111">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="636dc-111">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="636dc-112">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="636dc-112">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="636dc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="636dc-113">Properties</span></span>
| <span data-ttu-id="636dc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="636dc-114">Property</span></span>     | <span data-ttu-id="636dc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="636dc-115">Type</span></span>   |<span data-ttu-id="636dc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="636dc-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="636dc-117">id</span><span class="sxs-lookup"><span data-stu-id="636dc-117">id</span></span>       |<span data-ttu-id="636dc-118">string</span><span class="sxs-lookup"><span data-stu-id="636dc-118">string</span></span>   | <span data-ttu-id="636dc-119">Уникальный идентификационный код.</span><span class="sxs-lookup"><span data-stu-id="636dc-119">Unique Identifier</span></span> <span data-ttu-id="636dc-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="636dc-120">Read-only.</span></span>|
|<span data-ttu-id="636dc-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="636dc-121">majorUnit</span></span>|<span data-ttu-id="636dc-122">Json</span><span class="sxs-lookup"><span data-stu-id="636dc-122">Json</span></span>|<span data-ttu-id="636dc-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="636dc-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="636dc-126">maximum</span><span class="sxs-lookup"><span data-stu-id="636dc-126">maximum</span></span>|<span data-ttu-id="636dc-127">Json</span><span class="sxs-lookup"><span data-stu-id="636dc-127">Json</span></span>|<span data-ttu-id="636dc-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="636dc-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="636dc-131">minimum</span><span class="sxs-lookup"><span data-stu-id="636dc-131">minimum</span></span>|<span data-ttu-id="636dc-132">Json</span><span class="sxs-lookup"><span data-stu-id="636dc-132">Json</span></span>|<span data-ttu-id="636dc-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="636dc-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="636dc-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="636dc-136">minorUnit</span></span>|<span data-ttu-id="636dc-137">Json</span><span class="sxs-lookup"><span data-stu-id="636dc-137">Json</span></span>|<span data-ttu-id="636dc-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="636dc-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="636dc-141">Связи</span><span class="sxs-lookup"><span data-stu-id="636dc-141">Relationships</span></span>
| <span data-ttu-id="636dc-142">Связь</span><span class="sxs-lookup"><span data-stu-id="636dc-142">Relationship</span></span> | <span data-ttu-id="636dc-143">Тип</span><span class="sxs-lookup"><span data-stu-id="636dc-143">Type</span></span>   |<span data-ttu-id="636dc-144">Описание</span><span class="sxs-lookup"><span data-stu-id="636dc-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="636dc-145">format</span><span class="sxs-lookup"><span data-stu-id="636dc-145">format</span></span>|[<span data-ttu-id="636dc-146">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="636dc-146">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="636dc-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="636dc-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="636dc-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="636dc-149">majorGridlines</span></span>|[<span data-ttu-id="636dc-150">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="636dc-150">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="636dc-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="636dc-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="636dc-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="636dc-153">minorGridlines</span></span>|[<span data-ttu-id="636dc-154">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="636dc-154">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="636dc-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="636dc-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="636dc-157">title</span><span class="sxs-lookup"><span data-stu-id="636dc-157">title</span></span>|[<span data-ttu-id="636dc-158">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="636dc-158">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="636dc-p109">Представляет название оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="636dc-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="636dc-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="636dc-161">JSON representation</span></span>

<span data-ttu-id="636dc-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="636dc-162">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->