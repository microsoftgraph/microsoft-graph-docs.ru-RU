---
title: Тип ресурса Воркбукчарт
description: Представляет объект диаграммы в книге.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c180d6d2649f7c55868ffa04a5318c5c5f522ddd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007384"
---
# <a name="workbookchart-resource-type"></a><span data-ttu-id="b5133-103">Тип ресурса Воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="b5133-103">workbookChart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5133-104">Представляет объект диаграммы в книге.</span><span class="sxs-lookup"><span data-stu-id="b5133-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="b5133-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b5133-105">Methods</span></span>

| <span data-ttu-id="b5133-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b5133-106">Method</span></span>           | <span data-ttu-id="b5133-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b5133-107">Return Type</span></span>    |<span data-ttu-id="b5133-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b5133-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5133-109">Получение объекта Chart</span><span class="sxs-lookup"><span data-stu-id="b5133-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="b5133-110">Воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="b5133-110">workbookChart</span></span>](workbookchart.md) |<span data-ttu-id="b5133-111">Чтение свойств и связей объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b5133-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="b5133-112">Создание объекта ChartSeries</span><span class="sxs-lookup"><span data-stu-id="b5133-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="b5133-113">Воркбукчартсериес</span><span class="sxs-lookup"><span data-stu-id="b5133-113">workbookChartSeries</span></span>](workbookchartseries.md)| <span data-ttu-id="b5133-114">Создание объекта ChartSeries путем добавления в коллекцию рядов.</span><span class="sxs-lookup"><span data-stu-id="b5133-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="b5133-115">Список рядов</span><span class="sxs-lookup"><span data-stu-id="b5133-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="b5133-116">Коллекция [воркбукчартсериес](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="b5133-116">[workbookChartSeries](workbookchartseries.md) collection</span></span>| <span data-ttu-id="b5133-117">Получение коллекции объектов ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="b5133-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="b5133-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="b5133-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="b5133-119">Воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="b5133-119">workbookChart</span></span>](workbookchart.md)   |<span data-ttu-id="b5133-120">Обновление объекта Chart.</span><span class="sxs-lookup"><span data-stu-id="b5133-120">Update Chart object.</span></span> |
|[<span data-ttu-id="b5133-121">Image</span><span class="sxs-lookup"><span data-stu-id="b5133-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="b5133-122">Строка изображения с кодировкой base64</span><span class="sxs-lookup"><span data-stu-id="b5133-122">Image base64 encoded string</span></span>|<span data-ttu-id="b5133-123">Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.</span><span class="sxs-lookup"><span data-stu-id="b5133-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="b5133-124">Удаление</span><span class="sxs-lookup"><span data-stu-id="b5133-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="b5133-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b5133-125">None</span></span>|<span data-ttu-id="b5133-126">Удаляет объект диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b5133-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="b5133-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="b5133-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="b5133-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b5133-128">None</span></span>|<span data-ttu-id="b5133-129">Сбрасывает исходные данные для диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b5133-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="b5133-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="b5133-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="b5133-131">Нет</span><span class="sxs-lookup"><span data-stu-id="b5133-131">None</span></span>|<span data-ttu-id="b5133-132">Располагает диаграмму относительно ячеек на листе.</span><span class="sxs-lookup"><span data-stu-id="b5133-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="b5133-133">Список</span><span class="sxs-lookup"><span data-stu-id="b5133-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="b5133-134">Коллекция [воркбукчарт](workbookchart.md)</span><span class="sxs-lookup"><span data-stu-id="b5133-134">[workbookChart](workbookchart.md) collection</span></span> |<span data-ttu-id="b5133-135">Получение коллекции объектов диаграмм.</span><span class="sxs-lookup"><span data-stu-id="b5133-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="b5133-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="b5133-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="b5133-137">Воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="b5133-137">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="b5133-138">Возвращает диаграмму с учетом ее положения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="b5133-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="b5133-139">Add</span><span class="sxs-lookup"><span data-stu-id="b5133-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="b5133-140">Воркбукчарт</span><span class="sxs-lookup"><span data-stu-id="b5133-140">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="b5133-141">Создает диаграмму.</span><span class="sxs-lookup"><span data-stu-id="b5133-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5133-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5133-142">Properties</span></span>
| <span data-ttu-id="b5133-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5133-143">Property</span></span>     | <span data-ttu-id="b5133-144">Тип</span><span class="sxs-lookup"><span data-stu-id="b5133-144">Type</span></span>   |<span data-ttu-id="b5133-145">Описание</span><span class="sxs-lookup"><span data-stu-id="b5133-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5133-146">height</span><span class="sxs-lookup"><span data-stu-id="b5133-146">height</span></span>|<span data-ttu-id="b5133-147">double</span><span class="sxs-lookup"><span data-stu-id="b5133-147">double</span></span>|<span data-ttu-id="b5133-148">Обозначает высоту объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="b5133-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="b5133-149">id</span><span class="sxs-lookup"><span data-stu-id="b5133-149">id</span></span>|<span data-ttu-id="b5133-150">string</span><span class="sxs-lookup"><span data-stu-id="b5133-150">string</span></span>|<span data-ttu-id="b5133-p101">Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="b5133-153">left</span><span class="sxs-lookup"><span data-stu-id="b5133-153">left</span></span>|<span data-ttu-id="b5133-154">double</span><span class="sxs-lookup"><span data-stu-id="b5133-154">double</span></span>|<span data-ttu-id="b5133-155">Расстояние в пунктах от левого края диаграммы до начала листа.</span><span class="sxs-lookup"><span data-stu-id="b5133-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="b5133-156">name</span><span class="sxs-lookup"><span data-stu-id="b5133-156">name</span></span>|<span data-ttu-id="b5133-157">string</span><span class="sxs-lookup"><span data-stu-id="b5133-157">string</span></span>|<span data-ttu-id="b5133-158">Обозначает имя объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b5133-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="b5133-159">top</span><span class="sxs-lookup"><span data-stu-id="b5133-159">top</span></span>|<span data-ttu-id="b5133-160">double</span><span class="sxs-lookup"><span data-stu-id="b5133-160">double</span></span>|<span data-ttu-id="b5133-161">Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).</span><span class="sxs-lookup"><span data-stu-id="b5133-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="b5133-162">width</span><span class="sxs-lookup"><span data-stu-id="b5133-162">width</span></span>|<span data-ttu-id="b5133-163">double</span><span class="sxs-lookup"><span data-stu-id="b5133-163">double</span></span>|<span data-ttu-id="b5133-164">Представляет ширину объекта диаграммы (в пунктах).</span><span class="sxs-lookup"><span data-stu-id="b5133-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5133-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="b5133-165">Relationships</span></span>
| <span data-ttu-id="b5133-166">Отношение</span><span class="sxs-lookup"><span data-stu-id="b5133-166">Relationship</span></span> | <span data-ttu-id="b5133-167">Тип</span><span class="sxs-lookup"><span data-stu-id="b5133-167">Type</span></span>   |<span data-ttu-id="b5133-168">Описание</span><span class="sxs-lookup"><span data-stu-id="b5133-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5133-169">axes</span><span class="sxs-lookup"><span data-stu-id="b5133-169">axes</span></span>|[<span data-ttu-id="b5133-170">Воркбукчартаксес</span><span class="sxs-lookup"><span data-stu-id="b5133-170">workbookChartAxes</span></span>](workbookchartaxes.md)|<span data-ttu-id="b5133-p102">Представляет оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="b5133-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="b5133-173">dataLabels</span></span>|[<span data-ttu-id="b5133-174">Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="b5133-174">workbookChartDataLabels</span></span>](workbookchartdatalabels.md)|<span data-ttu-id="b5133-p103">Представляет метки данных на диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="b5133-177">format</span><span class="sxs-lookup"><span data-stu-id="b5133-177">format</span></span>|[<span data-ttu-id="b5133-178">Воркбукчартареаформат</span><span class="sxs-lookup"><span data-stu-id="b5133-178">workbookChartAreaFormat</span></span>](workbookchartareaformat.md)|<span data-ttu-id="b5133-p104">Инкапсулирует свойства формата для области диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="b5133-181">legend</span><span class="sxs-lookup"><span data-stu-id="b5133-181">legend</span></span>|[<span data-ttu-id="b5133-182">Воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="b5133-182">workbookChartLegend</span></span>](workbookchartlegend.md)|<span data-ttu-id="b5133-p105">Представляет условные обозначения для диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="b5133-185">series</span><span class="sxs-lookup"><span data-stu-id="b5133-185">series</span></span>|<span data-ttu-id="b5133-186">Коллекция [воркбукчартсериес](workbookchartseries.md)</span><span class="sxs-lookup"><span data-stu-id="b5133-186">[workbookChartSeries](workbookchartseries.md) collection</span></span>|<span data-ttu-id="b5133-p106">Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="b5133-189">title</span><span class="sxs-lookup"><span data-stu-id="b5133-189">title</span></span>|[<span data-ttu-id="b5133-190">Воркбукчарттитле</span><span class="sxs-lookup"><span data-stu-id="b5133-190">workbookChartTitle</span></span>](workbookcharttitle.md)|<span data-ttu-id="b5133-p107">Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="b5133-193">лист</span><span class="sxs-lookup"><span data-stu-id="b5133-193">worksheet</span></span>|[<span data-ttu-id="b5133-194">Воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="b5133-194">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="b5133-195">Лист, содержащий текущую диаграмму.</span><span class="sxs-lookup"><span data-stu-id="b5133-195">The worksheet containing the current chart.</span></span> <span data-ttu-id="b5133-196">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b5133-196">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5133-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5133-197">JSON representation</span></span>

<span data-ttu-id="b5133-198">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5133-198">Here is a JSON representation of the resource.</span></span>

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
