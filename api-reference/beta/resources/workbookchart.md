---
title: Тип ресурса Воркбукчарт
description: Представляет объект диаграммы в книге.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f28e89ae20d5675da303f11dc67b6e4b562b5340
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519409"
---
# <a name="workbookchart-resource-type"></a><span data-ttu-id="37439-103">Тип ресурса Воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="37439-103">workbookChart resource type</span></span>

<span data-ttu-id="37439-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37439-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37439-105">Представляет объект диаграммы в книге.</span><span class="sxs-lookup"><span data-stu-id="37439-105">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="37439-106">Методы</span><span class="sxs-lookup"><span data-stu-id="37439-106">Methods</span></span>

| <span data-ttu-id="37439-107">Метод</span><span class="sxs-lookup"><span data-stu-id="37439-107">Method</span></span>           | <span data-ttu-id="37439-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="37439-108">Return Type</span></span>    |<span data-ttu-id="37439-109">Описание</span><span class="sxs-lookup"><span data-stu-id="37439-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37439-110">Получение объекта Chart</span><span class="sxs-lookup"><span data-stu-id="37439-110">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="37439-111">воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="37439-111">workbookChart</span></span>](workbookchart.md) |<span data-ttu-id="37439-112">Чтение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="37439-112">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="37439-113">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="37439-113">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="37439-114">воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="37439-114">workbookChartSeries</span></span>](workbookchartseries.md)| <span data-ttu-id="37439-115">Создание объекта ChartSeries путем добавления в коллекцию рядов.</span><span class="sxs-lookup"><span data-stu-id="37439-115">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="37439-116">Список рядов</span><span class="sxs-lookup"><span data-stu-id="37439-116">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="37439-117">Коллекция [воркбукчартсериес](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="37439-117">[workbookChartSeries](workbookchartseries.md) collection</span></span>| <span data-ttu-id="37439-118">Получение коллекции объектов ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="37439-118">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="37439-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="37439-119">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="37439-120">воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="37439-120">workbookChart</span></span>](workbookchart.md)   |<span data-ttu-id="37439-121">Обновление объекта Chart.</span><span class="sxs-lookup"><span data-stu-id="37439-121">Update Chart object.</span></span> |
|[<span data-ttu-id="37439-122">Image</span><span class="sxs-lookup"><span data-stu-id="37439-122">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="37439-123">Строка изображения с кодировкой base64</span><span class="sxs-lookup"><span data-stu-id="37439-123">Image base64 encoded string</span></span>|<span data-ttu-id="37439-124">Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="37439-124">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|<span data-ttu-id="37439-125">[удаление](../api/chart-delete.md);</span><span class="sxs-lookup"><span data-stu-id="37439-125">[Delete](../api/chart-delete.md)</span></span>|<span data-ttu-id="37439-126">Нет</span><span class="sxs-lookup"><span data-stu-id="37439-126">None</span></span>|<span data-ttu-id="37439-127">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="37439-127">Deletes the chart object.</span></span>|
|[<span data-ttu-id="37439-128">Setdata</span><span class="sxs-lookup"><span data-stu-id="37439-128">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="37439-129">Нет</span><span class="sxs-lookup"><span data-stu-id="37439-129">None</span></span>|<span data-ttu-id="37439-130">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="37439-130">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="37439-131">Setposition</span><span class="sxs-lookup"><span data-stu-id="37439-131">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="37439-132">Нет</span><span class="sxs-lookup"><span data-stu-id="37439-132">None</span></span>|<span data-ttu-id="37439-133">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="37439-133">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="37439-134">Список</span><span class="sxs-lookup"><span data-stu-id="37439-134">List</span></span>](../api/chart-list.md) | <span data-ttu-id="37439-135">Коллекция [воркбукчарт](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="37439-135">[workbookChart](workbookchart.md) collection</span></span> |<span data-ttu-id="37439-136">Получение коллекции объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="37439-136">Get chart object collection.</span></span> |
|[<span data-ttu-id="37439-137">Itemat</span><span class="sxs-lookup"><span data-stu-id="37439-137">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="37439-138">воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="37439-138">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="37439-139">Возвращает диаграмму с учетом ее положения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="37439-139">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="37439-140">Add</span><span class="sxs-lookup"><span data-stu-id="37439-140">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="37439-141">воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="37439-141">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="37439-142">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="37439-142">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="37439-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="37439-143">Properties</span></span>
| <span data-ttu-id="37439-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="37439-144">Property</span></span>     | <span data-ttu-id="37439-145">Тип</span><span class="sxs-lookup"><span data-stu-id="37439-145">Type</span></span>   |<span data-ttu-id="37439-146">Описание</span><span class="sxs-lookup"><span data-stu-id="37439-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37439-147">height</span><span class="sxs-lookup"><span data-stu-id="37439-147">height</span></span>|<span data-ttu-id="37439-148">double</span><span class="sxs-lookup"><span data-stu-id="37439-148">double</span></span>|<span data-ttu-id="37439-149">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="37439-149">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="37439-150">id</span><span class="sxs-lookup"><span data-stu-id="37439-150">id</span></span>|<span data-ttu-id="37439-151">строка</span><span class="sxs-lookup"><span data-stu-id="37439-151">string</span></span>|<span data-ttu-id="37439-p101">Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="37439-154">left</span><span class="sxs-lookup"><span data-stu-id="37439-154">left</span></span>|<span data-ttu-id="37439-155">double</span><span class="sxs-lookup"><span data-stu-id="37439-155">double</span></span>|<span data-ttu-id="37439-156">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="37439-156">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="37439-157">name</span><span class="sxs-lookup"><span data-stu-id="37439-157">name</span></span>|<span data-ttu-id="37439-158">string</span><span class="sxs-lookup"><span data-stu-id="37439-158">string</span></span>|<span data-ttu-id="37439-159">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="37439-159">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="37439-160">top</span><span class="sxs-lookup"><span data-stu-id="37439-160">top</span></span>|<span data-ttu-id="37439-161">double</span><span class="sxs-lookup"><span data-stu-id="37439-161">double</span></span>|<span data-ttu-id="37439-162">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="37439-162">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="37439-163">width</span><span class="sxs-lookup"><span data-stu-id="37439-163">width</span></span>|<span data-ttu-id="37439-164">double</span><span class="sxs-lookup"><span data-stu-id="37439-164">double</span></span>|<span data-ttu-id="37439-165">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="37439-165">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37439-166">Связи</span><span class="sxs-lookup"><span data-stu-id="37439-166">Relationships</span></span>
| <span data-ttu-id="37439-167">Связь</span><span class="sxs-lookup"><span data-stu-id="37439-167">Relationship</span></span> | <span data-ttu-id="37439-168">Тип</span><span class="sxs-lookup"><span data-stu-id="37439-168">Type</span></span>   |<span data-ttu-id="37439-169">Описание</span><span class="sxs-lookup"><span data-stu-id="37439-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37439-170">axes</span><span class="sxs-lookup"><span data-stu-id="37439-170">axes</span></span>|[<span data-ttu-id="37439-171">воркбукчартаксес</span><span class="sxs-lookup"><span data-stu-id="37439-171">workbookChartAxes</span></span>](workbookchartaxes.md)|<span data-ttu-id="37439-p102">Представляет оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="37439-174">dataLabels</span><span class="sxs-lookup"><span data-stu-id="37439-174">dataLabels</span></span>|[<span data-ttu-id="37439-175">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="37439-175">workbookChartDataLabels</span></span>](workbookchartdatalabels.md)|<span data-ttu-id="37439-p103">Представляет метки данных на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="37439-178">format</span><span class="sxs-lookup"><span data-stu-id="37439-178">format</span></span>|[<span data-ttu-id="37439-179">воркбукчартареаформат</span><span class="sxs-lookup"><span data-stu-id="37439-179">workbookChartAreaFormat</span></span>](workbookchartareaformat.md)|<span data-ttu-id="37439-p104">Инкапсулирует свойства формата для области диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="37439-182">legend</span><span class="sxs-lookup"><span data-stu-id="37439-182">legend</span></span>|[<span data-ttu-id="37439-183">воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="37439-183">workbookChartLegend</span></span>](workbookchartlegend.md)|<span data-ttu-id="37439-p105">Представляет условные обозначения для диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="37439-186">series</span><span class="sxs-lookup"><span data-stu-id="37439-186">series</span></span>|<span data-ttu-id="37439-187">Коллекция [воркбукчартсериес](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="37439-187">[workbookChartSeries](workbookchartseries.md) collection</span></span>|<span data-ttu-id="37439-p106">Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="37439-190">title</span><span class="sxs-lookup"><span data-stu-id="37439-190">title</span></span>|[<span data-ttu-id="37439-191">воркбукчарттитле</span><span class="sxs-lookup"><span data-stu-id="37439-191">workbookChartTitle</span></span>](workbookcharttitle.md)|<span data-ttu-id="37439-p107">Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="37439-194">лист</span><span class="sxs-lookup"><span data-stu-id="37439-194">worksheet</span></span>|[<span data-ttu-id="37439-195">воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="37439-195">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="37439-196">Лист, содержащий текущую диаграмму.</span><span class="sxs-lookup"><span data-stu-id="37439-196">The worksheet containing the current chart.</span></span> <span data-ttu-id="37439-197">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37439-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37439-198">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37439-198">JSON representation</span></span>

<span data-ttu-id="37439-199">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37439-199">Here is a JSON representation of the resource.</span></span>

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
