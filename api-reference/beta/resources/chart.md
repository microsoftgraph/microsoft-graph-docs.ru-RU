---
title: Тип ресурса Chart
description: Представляет объект диаграммы в книге.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 09d5fd376cfdcd03517cc989708bbf17bcf49a72
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970677"
---
# <a name="chart-resource-type"></a><span data-ttu-id="def7d-103">Тип ресурса Chart</span><span class="sxs-lookup"><span data-stu-id="def7d-103">Chart resource type</span></span>

> <span data-ttu-id="def7d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="def7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="def7d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="def7d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="def7d-106">Представляет объект диаграммы в книге.</span><span class="sxs-lookup"><span data-stu-id="def7d-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="def7d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="def7d-107">Methods</span></span>

| <span data-ttu-id="def7d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="def7d-108">Method</span></span>           | <span data-ttu-id="def7d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="def7d-109">Return Type</span></span>    |<span data-ttu-id="def7d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="def7d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="def7d-111">Получение объекта Chart</span><span class="sxs-lookup"><span data-stu-id="def7d-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="def7d-112">Chart</span><span class="sxs-lookup"><span data-stu-id="def7d-112">Chart</span></span>](chart.md) |<span data-ttu-id="def7d-113">Чтение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="def7d-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="def7d-114">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="def7d-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="def7d-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="def7d-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="def7d-116">Создание объекта ChartSeries путем добавления в коллекцию рядов.</span><span class="sxs-lookup"><span data-stu-id="def7d-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="def7d-117">Список рядов</span><span class="sxs-lookup"><span data-stu-id="def7d-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="def7d-118">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="def7d-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="def7d-119">Получение коллекции объектов ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="def7d-119">Get a ChartSeries object collection.</span></span>|
|<span data-ttu-id="def7d-120">[обновление](../api/chart-update.md).</span><span class="sxs-lookup"><span data-stu-id="def7d-120">[Update](../api/chart-update.md)</span></span> | [<span data-ttu-id="def7d-121">Chart</span><span class="sxs-lookup"><span data-stu-id="def7d-121">Chart</span></span>](chart.md)   |<span data-ttu-id="def7d-122">Обновление объекта Chart.</span><span class="sxs-lookup"><span data-stu-id="def7d-122">Update Chart object.</span></span> |
|[<span data-ttu-id="def7d-123">Image</span><span class="sxs-lookup"><span data-stu-id="def7d-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="def7d-124">Строка изображения с кодировкой base64</span><span class="sxs-lookup"><span data-stu-id="def7d-124">Image base64 encoded string</span></span>|<span data-ttu-id="def7d-125">Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="def7d-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="def7d-126">Delete</span><span class="sxs-lookup"><span data-stu-id="def7d-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="def7d-127">Нет</span><span class="sxs-lookup"><span data-stu-id="def7d-127">None</span></span>|<span data-ttu-id="def7d-128">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="def7d-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="def7d-129">Setdata</span><span class="sxs-lookup"><span data-stu-id="def7d-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="def7d-130">Нет</span><span class="sxs-lookup"><span data-stu-id="def7d-130">None</span></span>|<span data-ttu-id="def7d-131">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="def7d-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="def7d-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="def7d-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="def7d-133">Нет</span><span class="sxs-lookup"><span data-stu-id="def7d-133">None</span></span>|<span data-ttu-id="def7d-134">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="def7d-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="def7d-135">List</span><span class="sxs-lookup"><span data-stu-id="def7d-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="def7d-136">Коллекция объектов [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="def7d-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="def7d-137">Получение коллекции объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="def7d-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="def7d-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="def7d-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="def7d-139">Диаграмма</span><span class="sxs-lookup"><span data-stu-id="def7d-139">Chart</span></span>](chart.md)|<span data-ttu-id="def7d-140">Возвращает диаграмму с учетом ее положения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="def7d-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="def7d-141">Add</span><span class="sxs-lookup"><span data-stu-id="def7d-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="def7d-142">Chart</span><span class="sxs-lookup"><span data-stu-id="def7d-142">Chart</span></span>](chart.md)|<span data-ttu-id="def7d-143">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="def7d-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="def7d-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="def7d-144">Properties</span></span>
| <span data-ttu-id="def7d-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="def7d-145">Property</span></span>     | <span data-ttu-id="def7d-146">Тип</span><span class="sxs-lookup"><span data-stu-id="def7d-146">Type</span></span>   |<span data-ttu-id="def7d-147">Описание</span><span class="sxs-lookup"><span data-stu-id="def7d-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="def7d-148">height</span><span class="sxs-lookup"><span data-stu-id="def7d-148">height</span></span>|<span data-ttu-id="def7d-149">double</span><span class="sxs-lookup"><span data-stu-id="def7d-149">double</span></span>|<span data-ttu-id="def7d-150">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="def7d-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="def7d-151">id</span><span class="sxs-lookup"><span data-stu-id="def7d-151">id</span></span>|<span data-ttu-id="def7d-152">строка</span><span class="sxs-lookup"><span data-stu-id="def7d-152">string</span></span>|<span data-ttu-id="def7d-p102">Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="def7d-155">left</span><span class="sxs-lookup"><span data-stu-id="def7d-155">left</span></span>|<span data-ttu-id="def7d-156">double</span><span class="sxs-lookup"><span data-stu-id="def7d-156">double</span></span>|<span data-ttu-id="def7d-157">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="def7d-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="def7d-158">name</span><span class="sxs-lookup"><span data-stu-id="def7d-158">name</span></span>|<span data-ttu-id="def7d-159">строка</span><span class="sxs-lookup"><span data-stu-id="def7d-159">string</span></span>|<span data-ttu-id="def7d-160">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="def7d-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="def7d-161">top</span><span class="sxs-lookup"><span data-stu-id="def7d-161">top</span></span>|<span data-ttu-id="def7d-162">double</span><span class="sxs-lookup"><span data-stu-id="def7d-162">double</span></span>|<span data-ttu-id="def7d-163">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="def7d-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="def7d-164">width</span><span class="sxs-lookup"><span data-stu-id="def7d-164">width</span></span>|<span data-ttu-id="def7d-165">double</span><span class="sxs-lookup"><span data-stu-id="def7d-165">double</span></span>|<span data-ttu-id="def7d-166">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="def7d-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="def7d-167">Связи</span><span class="sxs-lookup"><span data-stu-id="def7d-167">Relationships</span></span>
| <span data-ttu-id="def7d-168">Связь</span><span class="sxs-lookup"><span data-stu-id="def7d-168">Relationship</span></span> | <span data-ttu-id="def7d-169">Тип</span><span class="sxs-lookup"><span data-stu-id="def7d-169">Type</span></span>   |<span data-ttu-id="def7d-170">Описание</span><span class="sxs-lookup"><span data-stu-id="def7d-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="def7d-171">axes</span><span class="sxs-lookup"><span data-stu-id="def7d-171">axes</span></span>|[<span data-ttu-id="def7d-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="def7d-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="def7d-p103">Представляет оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="def7d-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="def7d-175">dataLabels</span></span>|[<span data-ttu-id="def7d-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="def7d-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="def7d-p104">Представляет метки данных на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="def7d-179">format</span><span class="sxs-lookup"><span data-stu-id="def7d-179">format</span></span>|[<span data-ttu-id="def7d-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="def7d-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="def7d-p105">Инкапсулирует свойства формата для области диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="def7d-183">legend</span><span class="sxs-lookup"><span data-stu-id="def7d-183">legend</span></span>|[<span data-ttu-id="def7d-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="def7d-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="def7d-p106">Представляет условные обозначения для диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="def7d-187">series</span><span class="sxs-lookup"><span data-stu-id="def7d-187">series</span></span>|<span data-ttu-id="def7d-188">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="def7d-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="def7d-p107">Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="def7d-191">title</span><span class="sxs-lookup"><span data-stu-id="def7d-191">title</span></span>|[<span data-ttu-id="def7d-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="def7d-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="def7d-p108">Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="def7d-195">worksheet</span><span class="sxs-lookup"><span data-stu-id="def7d-195">worksheet</span></span>|[<span data-ttu-id="def7d-196">Worksheet</span><span class="sxs-lookup"><span data-stu-id="def7d-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="def7d-p109">Лист, содержащий текущую диаграмму. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="def7d-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="def7d-199">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="def7d-199">JSON representation</span></span>

<span data-ttu-id="def7d-200">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="def7d-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
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
