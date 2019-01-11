---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: add7ef03b4779cae799949c6eb5901fcd1e3ddaf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809011"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="08d70-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="08d70-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="08d70-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="08d70-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="08d70-105">Методы</span><span class="sxs-lookup"><span data-stu-id="08d70-105">Methods</span></span>

| <span data-ttu-id="08d70-106">Метод</span><span class="sxs-lookup"><span data-stu-id="08d70-106">Method</span></span>           | <span data-ttu-id="08d70-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08d70-107">Return Type</span></span>    |<span data-ttu-id="08d70-108">Описание</span><span class="sxs-lookup"><span data-stu-id="08d70-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08d70-109">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="08d70-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="08d70-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="08d70-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="08d70-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="08d70-111">Read properties and relationships of chartDataLabels object.</span></span>|
|<span data-ttu-id="08d70-112">[обновление](../api/chartdatalabels-update.md).</span><span class="sxs-lookup"><span data-stu-id="08d70-112">[Update](../api/chartdatalabels-update.md)</span></span> | [<span data-ttu-id="08d70-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="08d70-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="08d70-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="08d70-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="08d70-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="08d70-115">Properties</span></span>
| <span data-ttu-id="08d70-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="08d70-116">Property</span></span>     | <span data-ttu-id="08d70-117">Тип</span><span class="sxs-lookup"><span data-stu-id="08d70-117">Type</span></span>   |<span data-ttu-id="08d70-118">Описание</span><span class="sxs-lookup"><span data-stu-id="08d70-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08d70-119">position</span><span class="sxs-lookup"><span data-stu-id="08d70-119">position</span></span>|<span data-ttu-id="08d70-120">string</span><span class="sxs-lookup"><span data-stu-id="08d70-120">string</span></span>|<span data-ttu-id="08d70-121">DataLabelPosition значение, представляющее положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="08d70-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="08d70-122">Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="08d70-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="08d70-123">разделитель</span><span class="sxs-lookup"><span data-stu-id="08d70-123">separator</span></span>|<span data-ttu-id="08d70-124">string</span><span class="sxs-lookup"><span data-stu-id="08d70-124">string</span></span>|<span data-ttu-id="08d70-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="08d70-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="08d70-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="08d70-126">showBubbleSize</span></span>|<span data-ttu-id="08d70-127">boolean</span><span class="sxs-lookup"><span data-stu-id="08d70-127">boolean</span></span>|<span data-ttu-id="08d70-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="08d70-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="08d70-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="08d70-129">showCategoryName</span></span>|<span data-ttu-id="08d70-130">boolean</span><span class="sxs-lookup"><span data-stu-id="08d70-130">boolean</span></span>|<span data-ttu-id="08d70-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="08d70-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="08d70-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="08d70-132">showLegendKey</span></span>|<span data-ttu-id="08d70-133">boolean</span><span class="sxs-lookup"><span data-stu-id="08d70-133">boolean</span></span>|<span data-ttu-id="08d70-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="08d70-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="08d70-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="08d70-135">showPercentage</span></span>|<span data-ttu-id="08d70-136">boolean</span><span class="sxs-lookup"><span data-stu-id="08d70-136">boolean</span></span>|<span data-ttu-id="08d70-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="08d70-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="08d70-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="08d70-138">showSeriesName</span></span>|<span data-ttu-id="08d70-139">boolean</span><span class="sxs-lookup"><span data-stu-id="08d70-139">boolean</span></span>|<span data-ttu-id="08d70-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="08d70-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="08d70-141">showValue</span><span class="sxs-lookup"><span data-stu-id="08d70-141">showValue</span></span>|<span data-ttu-id="08d70-142">boolean</span><span class="sxs-lookup"><span data-stu-id="08d70-142">boolean</span></span>|<span data-ttu-id="08d70-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="08d70-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08d70-144">Связи</span><span class="sxs-lookup"><span data-stu-id="08d70-144">Relationships</span></span>
| <span data-ttu-id="08d70-145">Связь</span><span class="sxs-lookup"><span data-stu-id="08d70-145">Relationship</span></span> | <span data-ttu-id="08d70-146">Тип</span><span class="sxs-lookup"><span data-stu-id="08d70-146">Type</span></span>   |<span data-ttu-id="08d70-147">Описание</span><span class="sxs-lookup"><span data-stu-id="08d70-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08d70-148">format</span><span class="sxs-lookup"><span data-stu-id="08d70-148">format</span></span>|[<span data-ttu-id="08d70-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="08d70-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="08d70-p102">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08d70-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08d70-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08d70-152">JSON representation</span></span>

<span data-ttu-id="08d70-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08d70-153">Here is a JSON representation of the resource.</span></span>

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
