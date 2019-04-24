---
title: Тип ресурса Chart
description: Представляет объект диаграммы в книге.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460942"
---
# <a name="chart-resource-type"></a><span data-ttu-id="a4e0f-103">Тип ресурса Chart</span><span class="sxs-lookup"><span data-stu-id="a4e0f-103">Chart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4e0f-104">Представляет объект диаграммы в книге.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="a4e0f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a4e0f-105">Methods</span></span>

| <span data-ttu-id="a4e0f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a4e0f-106">Method</span></span>           | <span data-ttu-id="a4e0f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4e0f-107">Return Type</span></span>    |<span data-ttu-id="a4e0f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e0f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4e0f-109">Получение объекта Chart</span><span class="sxs-lookup"><span data-stu-id="a4e0f-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="a4e0f-110">Chart</span><span class="sxs-lookup"><span data-stu-id="a4e0f-110">Chart</span></span>](chart.md) |<span data-ttu-id="a4e0f-111">Чтение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="a4e0f-112">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a4e0f-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="a4e0f-113">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a4e0f-113">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="a4e0f-114">Создание объекта ChartSeries путем добавления в коллекцию рядов.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="a4e0f-115">Список рядов</span><span class="sxs-lookup"><span data-stu-id="a4e0f-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="a4e0f-116">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="a4e0f-116">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="a4e0f-117">Получение коллекции объектов ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="a4e0f-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="a4e0f-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="a4e0f-119">Chart</span><span class="sxs-lookup"><span data-stu-id="a4e0f-119">Chart</span></span>](chart.md)   |<span data-ttu-id="a4e0f-120">Обновление объекта Chart.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-120">Update Chart object.</span></span> |
|[<span data-ttu-id="a4e0f-121">Image</span><span class="sxs-lookup"><span data-stu-id="a4e0f-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="a4e0f-122">Строка изображения с кодировкой base64</span><span class="sxs-lookup"><span data-stu-id="a4e0f-122">Image base64 encoded string</span></span>|<span data-ttu-id="a4e0f-123">Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="a4e0f-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="a4e0f-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="a4e0f-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a4e0f-125">None</span></span>|<span data-ttu-id="a4e0f-126">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="a4e0f-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="a4e0f-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="a4e0f-128">Нет</span><span class="sxs-lookup"><span data-stu-id="a4e0f-128">None</span></span>|<span data-ttu-id="a4e0f-129">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="a4e0f-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="a4e0f-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="a4e0f-131">Нет</span><span class="sxs-lookup"><span data-stu-id="a4e0f-131">None</span></span>|<span data-ttu-id="a4e0f-132">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="a4e0f-133">Список</span><span class="sxs-lookup"><span data-stu-id="a4e0f-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="a4e0f-134">Коллекция объектов [Chart](chart.md)</span><span class="sxs-lookup"><span data-stu-id="a4e0f-134">[Chart](chart.md) collection</span></span> |<span data-ttu-id="a4e0f-135">Получение коллекции объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="a4e0f-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="a4e0f-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="a4e0f-137">Диаграмма</span><span class="sxs-lookup"><span data-stu-id="a4e0f-137">Chart</span></span>](chart.md)|<span data-ttu-id="a4e0f-138">Возвращает диаграмму с учетом ее положения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="a4e0f-139">Add</span><span class="sxs-lookup"><span data-stu-id="a4e0f-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="a4e0f-140">Chart</span><span class="sxs-lookup"><span data-stu-id="a4e0f-140">Chart</span></span>](chart.md)|<span data-ttu-id="a4e0f-141">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4e0f-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4e0f-142">Properties</span></span>
| <span data-ttu-id="a4e0f-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4e0f-143">Property</span></span>     | <span data-ttu-id="a4e0f-144">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e0f-144">Type</span></span>   |<span data-ttu-id="a4e0f-145">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e0f-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4e0f-146">height</span><span class="sxs-lookup"><span data-stu-id="a4e0f-146">height</span></span>|<span data-ttu-id="a4e0f-147">double</span><span class="sxs-lookup"><span data-stu-id="a4e0f-147">double</span></span>|<span data-ttu-id="a4e0f-148">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="a4e0f-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="a4e0f-149">id</span><span class="sxs-lookup"><span data-stu-id="a4e0f-149">id</span></span>|<span data-ttu-id="a4e0f-150">строка</span><span class="sxs-lookup"><span data-stu-id="a4e0f-150">string</span></span>|<span data-ttu-id="a4e0f-p101">Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="a4e0f-153">left</span><span class="sxs-lookup"><span data-stu-id="a4e0f-153">left</span></span>|<span data-ttu-id="a4e0f-154">double</span><span class="sxs-lookup"><span data-stu-id="a4e0f-154">double</span></span>|<span data-ttu-id="a4e0f-155">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="a4e0f-156">name</span><span class="sxs-lookup"><span data-stu-id="a4e0f-156">name</span></span>|<span data-ttu-id="a4e0f-157">string</span><span class="sxs-lookup"><span data-stu-id="a4e0f-157">string</span></span>|<span data-ttu-id="a4e0f-158">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="a4e0f-159">top</span><span class="sxs-lookup"><span data-stu-id="a4e0f-159">top</span></span>|<span data-ttu-id="a4e0f-160">double</span><span class="sxs-lookup"><span data-stu-id="a4e0f-160">double</span></span>|<span data-ttu-id="a4e0f-161">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="a4e0f-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="a4e0f-162">width</span><span class="sxs-lookup"><span data-stu-id="a4e0f-162">width</span></span>|<span data-ttu-id="a4e0f-163">double</span><span class="sxs-lookup"><span data-stu-id="a4e0f-163">double</span></span>|<span data-ttu-id="a4e0f-164">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="a4e0f-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4e0f-165">Связи</span><span class="sxs-lookup"><span data-stu-id="a4e0f-165">Relationships</span></span>
| <span data-ttu-id="a4e0f-166">Отношение</span><span class="sxs-lookup"><span data-stu-id="a4e0f-166">Relationship</span></span> | <span data-ttu-id="a4e0f-167">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e0f-167">Type</span></span>   |<span data-ttu-id="a4e0f-168">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e0f-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4e0f-169">axes</span><span class="sxs-lookup"><span data-stu-id="a4e0f-169">axes</span></span>|[<span data-ttu-id="a4e0f-170">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="a4e0f-170">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="a4e0f-p102">Представляет оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="a4e0f-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="a4e0f-173">dataLabels</span></span>|[<span data-ttu-id="a4e0f-174">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="a4e0f-174">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="a4e0f-p103">Представляет метки данных на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="a4e0f-177">format</span><span class="sxs-lookup"><span data-stu-id="a4e0f-177">format</span></span>|[<span data-ttu-id="a4e0f-178">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="a4e0f-178">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="a4e0f-p104">Инкапсулирует свойства формата для области диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="a4e0f-181">legend</span><span class="sxs-lookup"><span data-stu-id="a4e0f-181">legend</span></span>|[<span data-ttu-id="a4e0f-182">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="a4e0f-182">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="a4e0f-p105">Представляет условные обозначения для диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="a4e0f-185">series</span><span class="sxs-lookup"><span data-stu-id="a4e0f-185">series</span></span>|<span data-ttu-id="a4e0f-186">Коллекция объектов [ChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="a4e0f-186">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="a4e0f-p106">Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="a4e0f-189">title</span><span class="sxs-lookup"><span data-stu-id="a4e0f-189">title</span></span>|[<span data-ttu-id="a4e0f-190">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="a4e0f-190">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="a4e0f-p107">Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="a4e0f-193">лист</span><span class="sxs-lookup"><span data-stu-id="a4e0f-193">worksheet</span></span>|[<span data-ttu-id="a4e0f-194">Worksheet</span><span class="sxs-lookup"><span data-stu-id="a4e0f-194">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="a4e0f-p108">Лист, содержащий текущую диаграмму. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4e0f-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4e0f-197">JSON representation</span></span>

<span data-ttu-id="a4e0f-198">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4e0f-198">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
