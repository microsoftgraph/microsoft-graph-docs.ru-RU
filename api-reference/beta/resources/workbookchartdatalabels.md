---
title: Тип ресурса Воркбукчартдаталабелс
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 28dc0d70f057569cd240770e15964b13c7982bae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979289"
---
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="c0950-103">Тип ресурса Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="c0950-103">workbookChartDataLabels resource type</span></span>

<span data-ttu-id="c0950-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0950-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0950-105">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c0950-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="c0950-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c0950-106">Methods</span></span>

| <span data-ttu-id="c0950-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c0950-107">Method</span></span>           | <span data-ttu-id="c0950-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0950-108">Return Type</span></span>    |<span data-ttu-id="c0950-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c0950-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c0950-110">Получение Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="c0950-110">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="c0950-111">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="c0950-111">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="c0950-112">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="c0950-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="c0950-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="c0950-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="c0950-114">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="c0950-114">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="c0950-115">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="c0950-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c0950-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0950-116">Properties</span></span>
| <span data-ttu-id="c0950-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0950-117">Property</span></span>     | <span data-ttu-id="c0950-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c0950-118">Type</span></span>   |<span data-ttu-id="c0950-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c0950-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0950-120">position</span><span class="sxs-lookup"><span data-stu-id="c0950-120">position</span></span>|<span data-ttu-id="c0950-121">string</span><span class="sxs-lookup"><span data-stu-id="c0950-121">string</span></span>|<span data-ttu-id="c0950-122">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="c0950-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="c0950-123">Возможные значения: `None` , `Center` ,,, `InsideEnd` `InsideBase` `OutsideEnd` , `Left` , `Right` ,,, `Top` `Bottom` `BestFit` , `Callout` .</span><span class="sxs-lookup"><span data-stu-id="c0950-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="c0950-124">separator</span><span class="sxs-lookup"><span data-stu-id="c0950-124">separator</span></span>|<span data-ttu-id="c0950-125">string</span><span class="sxs-lookup"><span data-stu-id="c0950-125">string</span></span>|<span data-ttu-id="c0950-126">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="c0950-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="c0950-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="c0950-127">showBubbleSize</span></span>|<span data-ttu-id="c0950-128">boolean</span><span class="sxs-lookup"><span data-stu-id="c0950-128">boolean</span></span>|<span data-ttu-id="c0950-129">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="c0950-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="c0950-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="c0950-130">showCategoryName</span></span>|<span data-ttu-id="c0950-131">boolean</span><span class="sxs-lookup"><span data-stu-id="c0950-131">boolean</span></span>|<span data-ttu-id="c0950-132">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="c0950-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="c0950-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="c0950-133">showLegendKey</span></span>|<span data-ttu-id="c0950-134">boolean</span><span class="sxs-lookup"><span data-stu-id="c0950-134">boolean</span></span>|<span data-ttu-id="c0950-135">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="c0950-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="c0950-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="c0950-136">showPercentage</span></span>|<span data-ttu-id="c0950-137">boolean</span><span class="sxs-lookup"><span data-stu-id="c0950-137">boolean</span></span>|<span data-ttu-id="c0950-138">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="c0950-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="c0950-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="c0950-139">showSeriesName</span></span>|<span data-ttu-id="c0950-140">boolean</span><span class="sxs-lookup"><span data-stu-id="c0950-140">boolean</span></span>|<span data-ttu-id="c0950-141">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="c0950-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="c0950-142">showValue</span><span class="sxs-lookup"><span data-stu-id="c0950-142">showValue</span></span>|<span data-ttu-id="c0950-143">boolean</span><span class="sxs-lookup"><span data-stu-id="c0950-143">boolean</span></span>|<span data-ttu-id="c0950-144">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="c0950-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0950-145">Связи</span><span class="sxs-lookup"><span data-stu-id="c0950-145">Relationships</span></span>
| <span data-ttu-id="c0950-146">Связь</span><span class="sxs-lookup"><span data-stu-id="c0950-146">Relationship</span></span> | <span data-ttu-id="c0950-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c0950-147">Type</span></span>   |<span data-ttu-id="c0950-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c0950-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0950-149">format</span><span class="sxs-lookup"><span data-stu-id="c0950-149">format</span></span>|[<span data-ttu-id="c0950-150">воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="c0950-150">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="c0950-151">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов.</span><span class="sxs-lookup"><span data-stu-id="c0950-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="c0950-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0950-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0950-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0950-153">JSON representation</span></span>

<span data-ttu-id="c0950-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0950-154">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


