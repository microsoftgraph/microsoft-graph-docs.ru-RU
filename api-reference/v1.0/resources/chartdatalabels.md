---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 502f18fdf03eb28bde4b6f8620bb274f6f2052dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988438"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="5dd0d-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5dd0d-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="5dd0d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dd0d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5dd0d-105">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="5dd0d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5dd0d-106">Methods</span></span>

| <span data-ttu-id="5dd0d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5dd0d-107">Method</span></span>           | <span data-ttu-id="5dd0d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5dd0d-108">Return Type</span></span>    |<span data-ttu-id="5dd0d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd0d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5dd0d-110">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5dd0d-110">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="5dd0d-111">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="5dd0d-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5dd0d-112">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="5dd0d-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="5dd0d-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="5dd0d-114">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="5dd0d-114">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5dd0d-115">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5dd0d-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dd0d-116">Properties</span></span>
| <span data-ttu-id="5dd0d-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="5dd0d-117">Property</span></span>     | <span data-ttu-id="5dd0d-118">Тип</span><span class="sxs-lookup"><span data-stu-id="5dd0d-118">Type</span></span>   |<span data-ttu-id="5dd0d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd0d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dd0d-120">position</span><span class="sxs-lookup"><span data-stu-id="5dd0d-120">position</span></span>|<span data-ttu-id="5dd0d-121">string</span><span class="sxs-lookup"><span data-stu-id="5dd0d-121">string</span></span>|<span data-ttu-id="5dd0d-122">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="5dd0d-123">Возможные значения: `None` , `Center` ,,, `InsideEnd` `InsideBase` `OutsideEnd` , `Left` , `Right` ,,, `Top` `Bottom` `BestFit` , `Callout` .</span><span class="sxs-lookup"><span data-stu-id="5dd0d-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="5dd0d-124">separator</span><span class="sxs-lookup"><span data-stu-id="5dd0d-124">separator</span></span>|<span data-ttu-id="5dd0d-125">string</span><span class="sxs-lookup"><span data-stu-id="5dd0d-125">string</span></span>|<span data-ttu-id="5dd0d-126">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="5dd0d-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="5dd0d-127">showBubbleSize</span></span>|<span data-ttu-id="5dd0d-128">boolean</span><span class="sxs-lookup"><span data-stu-id="5dd0d-128">boolean</span></span>|<span data-ttu-id="5dd0d-129">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="5dd0d-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="5dd0d-130">showCategoryName</span></span>|<span data-ttu-id="5dd0d-131">boolean</span><span class="sxs-lookup"><span data-stu-id="5dd0d-131">boolean</span></span>|<span data-ttu-id="5dd0d-132">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="5dd0d-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="5dd0d-133">showLegendKey</span></span>|<span data-ttu-id="5dd0d-134">boolean</span><span class="sxs-lookup"><span data-stu-id="5dd0d-134">boolean</span></span>|<span data-ttu-id="5dd0d-135">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="5dd0d-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="5dd0d-136">showPercentage</span></span>|<span data-ttu-id="5dd0d-137">boolean</span><span class="sxs-lookup"><span data-stu-id="5dd0d-137">boolean</span></span>|<span data-ttu-id="5dd0d-138">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="5dd0d-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="5dd0d-139">showSeriesName</span></span>|<span data-ttu-id="5dd0d-140">boolean</span><span class="sxs-lookup"><span data-stu-id="5dd0d-140">boolean</span></span>|<span data-ttu-id="5dd0d-141">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="5dd0d-142">showValue</span><span class="sxs-lookup"><span data-stu-id="5dd0d-142">showValue</span></span>|<span data-ttu-id="5dd0d-143">boolean</span><span class="sxs-lookup"><span data-stu-id="5dd0d-143">boolean</span></span>|<span data-ttu-id="5dd0d-144">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dd0d-145">Связи</span><span class="sxs-lookup"><span data-stu-id="5dd0d-145">Relationships</span></span>
| <span data-ttu-id="5dd0d-146">Связь</span><span class="sxs-lookup"><span data-stu-id="5dd0d-146">Relationship</span></span> | <span data-ttu-id="5dd0d-147">Тип</span><span class="sxs-lookup"><span data-stu-id="5dd0d-147">Type</span></span>   |<span data-ttu-id="5dd0d-148">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd0d-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dd0d-149">format</span><span class="sxs-lookup"><span data-stu-id="5dd0d-149">format</span></span>|[<span data-ttu-id="5dd0d-150">воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="5dd0d-150">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="5dd0d-151">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="5dd0d-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dd0d-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5dd0d-153">JSON representation</span></span>

<span data-ttu-id="5dd0d-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dd0d-154">Here is a JSON representation of the resource.</span></span>

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

