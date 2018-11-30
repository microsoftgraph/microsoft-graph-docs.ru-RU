---
title: Тип ресурса Chart
description: Представляет объект диаграммы в книге.
ms.openlocfilehash: 3305c674bf299fa68ce139ba16b3174965b694ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080933"
---
# <a name="chart-resource-type"></a><span data-ttu-id="18403-103">Тип ресурса Chart</span><span class="sxs-lookup"><span data-stu-id="18403-103">Chart resource type</span></span>

> <span data-ttu-id="18403-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18403-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18403-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18403-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18403-106">Представляет объект диаграммы в книге.</span><span class="sxs-lookup"><span data-stu-id="18403-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="18403-107">Методы</span><span class="sxs-lookup"><span data-stu-id="18403-107">Methods</span></span>

| <span data-ttu-id="18403-108">Метод</span><span class="sxs-lookup"><span data-stu-id="18403-108">Method</span></span>           | <span data-ttu-id="18403-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18403-109">Return Type</span></span>    |<span data-ttu-id="18403-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18403-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18403-111">Получение объекта Chart</span><span class="sxs-lookup"><span data-stu-id="18403-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="18403-112">Chart</span><span class="sxs-lookup"><span data-stu-id="18403-112">Chart</span></span>](chart.md) |<span data-ttu-id="18403-113">Чтение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="18403-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="18403-114">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="18403-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="18403-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="18403-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="18403-116">Создание объекта ChartSeries путем добавления в коллекцию рядов.</span><span class="sxs-lookup"><span data-stu-id="18403-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="18403-117">Список рядов</span><span class="sxs-lookup"><span data-stu-id="18403-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="18403-118">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="18403-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="18403-119">Получение коллекции объектов ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="18403-119">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="18403-120">Update</span><span class="sxs-lookup"><span data-stu-id="18403-120">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="18403-121">Chart</span><span class="sxs-lookup"><span data-stu-id="18403-121">Chart</span></span>](chart.md)   |<span data-ttu-id="18403-122">Обновление объекта Chart.</span><span class="sxs-lookup"><span data-stu-id="18403-122">Update Chart object.</span></span> |
|[<span data-ttu-id="18403-123">Image</span><span class="sxs-lookup"><span data-stu-id="18403-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="18403-124">Строка изображения с кодировкой base64</span><span class="sxs-lookup"><span data-stu-id="18403-124">Image base64 encoded string</span></span>|<span data-ttu-id="18403-125">Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="18403-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="18403-126">Delete</span><span class="sxs-lookup"><span data-stu-id="18403-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="18403-127">Нет</span><span class="sxs-lookup"><span data-stu-id="18403-127">None</span></span>|<span data-ttu-id="18403-128">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="18403-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="18403-129">Setdata</span><span class="sxs-lookup"><span data-stu-id="18403-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="18403-130">Нет</span><span class="sxs-lookup"><span data-stu-id="18403-130">None</span></span>|<span data-ttu-id="18403-131">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="18403-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="18403-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="18403-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="18403-133">Нет</span><span class="sxs-lookup"><span data-stu-id="18403-133">None</span></span>|<span data-ttu-id="18403-134">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="18403-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="18403-135">List</span><span class="sxs-lookup"><span data-stu-id="18403-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="18403-136">Коллекция объектов [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="18403-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="18403-137">Получение коллекции объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="18403-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="18403-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="18403-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="18403-139">Диаграмма</span><span class="sxs-lookup"><span data-stu-id="18403-139">Chart</span></span>](chart.md)|<span data-ttu-id="18403-140">Возвращает диаграмму с учетом ее положения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="18403-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="18403-141">Add</span><span class="sxs-lookup"><span data-stu-id="18403-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="18403-142">Chart</span><span class="sxs-lookup"><span data-stu-id="18403-142">Chart</span></span>](chart.md)|<span data-ttu-id="18403-143">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="18403-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="18403-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="18403-144">Properties</span></span>
| <span data-ttu-id="18403-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="18403-145">Property</span></span>     | <span data-ttu-id="18403-146">Тип</span><span class="sxs-lookup"><span data-stu-id="18403-146">Type</span></span>   |<span data-ttu-id="18403-147">Описание</span><span class="sxs-lookup"><span data-stu-id="18403-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18403-148">height</span><span class="sxs-lookup"><span data-stu-id="18403-148">height</span></span>|<span data-ttu-id="18403-149">double</span><span class="sxs-lookup"><span data-stu-id="18403-149">double</span></span>|<span data-ttu-id="18403-150">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="18403-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="18403-151">id</span><span class="sxs-lookup"><span data-stu-id="18403-151">id</span></span>|<span data-ttu-id="18403-152">строка</span><span class="sxs-lookup"><span data-stu-id="18403-152">string</span></span>|<span data-ttu-id="18403-p102">Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="18403-155">left</span><span class="sxs-lookup"><span data-stu-id="18403-155">left</span></span>|<span data-ttu-id="18403-156">double</span><span class="sxs-lookup"><span data-stu-id="18403-156">double</span></span>|<span data-ttu-id="18403-157">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="18403-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="18403-158">name</span><span class="sxs-lookup"><span data-stu-id="18403-158">name</span></span>|<span data-ttu-id="18403-159">строка</span><span class="sxs-lookup"><span data-stu-id="18403-159">string</span></span>|<span data-ttu-id="18403-160">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="18403-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="18403-161">top</span><span class="sxs-lookup"><span data-stu-id="18403-161">top</span></span>|<span data-ttu-id="18403-162">double</span><span class="sxs-lookup"><span data-stu-id="18403-162">double</span></span>|<span data-ttu-id="18403-163">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="18403-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="18403-164">width</span><span class="sxs-lookup"><span data-stu-id="18403-164">width</span></span>|<span data-ttu-id="18403-165">double</span><span class="sxs-lookup"><span data-stu-id="18403-165">double</span></span>|<span data-ttu-id="18403-166">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="18403-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18403-167">Связи</span><span class="sxs-lookup"><span data-stu-id="18403-167">Relationships</span></span>
| <span data-ttu-id="18403-168">Связь</span><span class="sxs-lookup"><span data-stu-id="18403-168">Relationship</span></span> | <span data-ttu-id="18403-169">Тип</span><span class="sxs-lookup"><span data-stu-id="18403-169">Type</span></span>   |<span data-ttu-id="18403-170">Описание</span><span class="sxs-lookup"><span data-stu-id="18403-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18403-171">axes</span><span class="sxs-lookup"><span data-stu-id="18403-171">axes</span></span>|[<span data-ttu-id="18403-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="18403-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="18403-p103">Представляет оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="18403-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="18403-175">dataLabels</span></span>|[<span data-ttu-id="18403-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="18403-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="18403-p104">Представляет метки данных на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="18403-179">format</span><span class="sxs-lookup"><span data-stu-id="18403-179">format</span></span>|[<span data-ttu-id="18403-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="18403-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="18403-p105">Инкапсулирует свойства формата для области диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="18403-183">legend</span><span class="sxs-lookup"><span data-stu-id="18403-183">legend</span></span>|[<span data-ttu-id="18403-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="18403-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="18403-p106">Представляет условные обозначения для диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="18403-187">series</span><span class="sxs-lookup"><span data-stu-id="18403-187">series</span></span>|<span data-ttu-id="18403-188">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="18403-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="18403-p107">Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="18403-191">title</span><span class="sxs-lookup"><span data-stu-id="18403-191">title</span></span>|[<span data-ttu-id="18403-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="18403-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="18403-p108">Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="18403-195">лист</span><span class="sxs-lookup"><span data-stu-id="18403-195">worksheet</span></span>|[<span data-ttu-id="18403-196">Worksheet</span><span class="sxs-lookup"><span data-stu-id="18403-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="18403-p109">Лист, содержащий текущую диаграмму. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18403-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18403-199">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18403-199">JSON representation</span></span>

<span data-ttu-id="18403-200">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18403-200">Here is a JSON representation of the resource.</span></span>

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