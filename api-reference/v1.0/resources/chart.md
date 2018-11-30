---
title: Тип ресурса Chart
description: Представляет объект диаграммы в книге.
ms.openlocfilehash: bada94032dcc00e3f6294b20559f44044570f2ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025920"
---
# <a name="chart-resource-type"></a><span data-ttu-id="b164e-103">Тип ресурса Chart</span><span class="sxs-lookup"><span data-stu-id="b164e-103">Chart resource type</span></span>

<span data-ttu-id="b164e-104">Представляет объект диаграммы в книге.</span><span class="sxs-lookup"><span data-stu-id="b164e-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="b164e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b164e-105">Methods</span></span>

| <span data-ttu-id="b164e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b164e-106">Method</span></span>           | <span data-ttu-id="b164e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b164e-107">Return Type</span></span>    |<span data-ttu-id="b164e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b164e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b164e-109">Получение объекта Chart</span><span class="sxs-lookup"><span data-stu-id="b164e-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="b164e-110">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="b164e-110">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="b164e-111">Чтение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b164e-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="b164e-112">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="b164e-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="b164e-113">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="b164e-113">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="b164e-114">Создание объекта ChartSeries путем добавления в коллекцию рядов.</span><span class="sxs-lookup"><span data-stu-id="b164e-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="b164e-115">Список рядов</span><span class="sxs-lookup"><span data-stu-id="b164e-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="b164e-116">[WorkbookChartSeries](chartseries.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b164e-116">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="b164e-117">Получение коллекции объектов ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="b164e-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="b164e-118">Update</span><span class="sxs-lookup"><span data-stu-id="b164e-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="b164e-119">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="b164e-119">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="b164e-120">Обновление объекта Chart.</span><span class="sxs-lookup"><span data-stu-id="b164e-120">Update Chart object.</span></span> |
|[<span data-ttu-id="b164e-121">Image</span><span class="sxs-lookup"><span data-stu-id="b164e-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="b164e-122">Строка изображения с кодировкой base64</span><span class="sxs-lookup"><span data-stu-id="b164e-122">Image base64 encoded string</span></span>|<span data-ttu-id="b164e-123">Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="b164e-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="b164e-124">Delete</span><span class="sxs-lookup"><span data-stu-id="b164e-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="b164e-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b164e-125">None</span></span>|<span data-ttu-id="b164e-126">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b164e-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="b164e-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="b164e-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="b164e-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b164e-128">None</span></span>|<span data-ttu-id="b164e-129">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b164e-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="b164e-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="b164e-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="b164e-131">Нет</span><span class="sxs-lookup"><span data-stu-id="b164e-131">None</span></span>|<span data-ttu-id="b164e-132">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="b164e-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="b164e-133">List</span><span class="sxs-lookup"><span data-stu-id="b164e-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="b164e-134">[WorkbookChart](chart.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b164e-134">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="b164e-135">Получение коллекции объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="b164e-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="b164e-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="b164e-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="b164e-137">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="b164e-137">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="b164e-138">Возвращает диаграмму на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="b164e-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="b164e-139">Add</span><span class="sxs-lookup"><span data-stu-id="b164e-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="b164e-140">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="b164e-140">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="b164e-141">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="b164e-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="b164e-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="b164e-142">Properties</span></span>
| <span data-ttu-id="b164e-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="b164e-143">Property</span></span>     | <span data-ttu-id="b164e-144">Тип</span><span class="sxs-lookup"><span data-stu-id="b164e-144">Type</span></span>   |<span data-ttu-id="b164e-145">Описание</span><span class="sxs-lookup"><span data-stu-id="b164e-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b164e-146">height</span><span class="sxs-lookup"><span data-stu-id="b164e-146">height</span></span>|<span data-ttu-id="b164e-147">double</span><span class="sxs-lookup"><span data-stu-id="b164e-147">double</span></span>|<span data-ttu-id="b164e-148">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="b164e-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="b164e-149">id</span><span class="sxs-lookup"><span data-stu-id="b164e-149">id</span></span>|<span data-ttu-id="b164e-150">строка</span><span class="sxs-lookup"><span data-stu-id="b164e-150">string</span></span>|<span data-ttu-id="b164e-p101">Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="b164e-153">left</span><span class="sxs-lookup"><span data-stu-id="b164e-153">left</span></span>|<span data-ttu-id="b164e-154">double</span><span class="sxs-lookup"><span data-stu-id="b164e-154">double</span></span>|<span data-ttu-id="b164e-155">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="b164e-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="b164e-156">name</span><span class="sxs-lookup"><span data-stu-id="b164e-156">name</span></span>|<span data-ttu-id="b164e-157">строка</span><span class="sxs-lookup"><span data-stu-id="b164e-157">string</span></span>|<span data-ttu-id="b164e-158">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b164e-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="b164e-159">top</span><span class="sxs-lookup"><span data-stu-id="b164e-159">top</span></span>|<span data-ttu-id="b164e-160">double</span><span class="sxs-lookup"><span data-stu-id="b164e-160">double</span></span>|<span data-ttu-id="b164e-161">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="b164e-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="b164e-162">width</span><span class="sxs-lookup"><span data-stu-id="b164e-162">width</span></span>|<span data-ttu-id="b164e-163">double</span><span class="sxs-lookup"><span data-stu-id="b164e-163">double</span></span>|<span data-ttu-id="b164e-164">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="b164e-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b164e-165">Связи</span><span class="sxs-lookup"><span data-stu-id="b164e-165">Relationships</span></span>
| <span data-ttu-id="b164e-166">Связь</span><span class="sxs-lookup"><span data-stu-id="b164e-166">Relationship</span></span> | <span data-ttu-id="b164e-167">Тип</span><span class="sxs-lookup"><span data-stu-id="b164e-167">Type</span></span>   |<span data-ttu-id="b164e-168">Описание</span><span class="sxs-lookup"><span data-stu-id="b164e-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b164e-169">axes</span><span class="sxs-lookup"><span data-stu-id="b164e-169">axes</span></span>|[<span data-ttu-id="b164e-170">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="b164e-170">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="b164e-p102">Представляет оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="b164e-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="b164e-173">dataLabels</span></span>|[<span data-ttu-id="b164e-174">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="b164e-174">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="b164e-p103">Представляет метки данных на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="b164e-177">format</span><span class="sxs-lookup"><span data-stu-id="b164e-177">format</span></span>|[<span data-ttu-id="b164e-178">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="b164e-178">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="b164e-p104">Инкапсулирует свойства формата для области диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="b164e-181">legend</span><span class="sxs-lookup"><span data-stu-id="b164e-181">legend</span></span>|[<span data-ttu-id="b164e-182">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="b164e-182">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="b164e-p105">Представляет условные обозначения для диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="b164e-185">series</span><span class="sxs-lookup"><span data-stu-id="b164e-185">series</span></span>|<span data-ttu-id="b164e-186">[WorkbookChartSeries](chartseries.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b164e-186">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="b164e-p106">Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="b164e-189">title</span><span class="sxs-lookup"><span data-stu-id="b164e-189">title</span></span>|[<span data-ttu-id="b164e-190">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="b164e-190">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="b164e-p107">Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="b164e-193">лист</span><span class="sxs-lookup"><span data-stu-id="b164e-193">worksheet</span></span>|[<span data-ttu-id="b164e-194">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b164e-194">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="b164e-p108">Лист, содержащий текущую диаграмму. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b164e-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b164e-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b164e-197">JSON representation</span></span>

<span data-ttu-id="b164e-198">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b164e-198">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->