---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e1369ee83abb98d7d673fab4a8f37c2b4c13e317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029822"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="5e109-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5e109-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="5e109-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5e109-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="5e109-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5e109-105">Methods</span></span>

| <span data-ttu-id="5e109-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5e109-106">Method</span></span>           | <span data-ttu-id="5e109-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e109-107">Return Type</span></span>    |<span data-ttu-id="5e109-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5e109-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e109-109">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5e109-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="5e109-110">Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="5e109-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5e109-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5e109-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="5e109-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="5e109-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="5e109-113">Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="5e109-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5e109-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5e109-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5e109-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e109-115">Properties</span></span>
| <span data-ttu-id="5e109-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e109-116">Property</span></span>     | <span data-ttu-id="5e109-117">Тип</span><span class="sxs-lookup"><span data-stu-id="5e109-117">Type</span></span>   |<span data-ttu-id="5e109-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5e109-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e109-119">position</span><span class="sxs-lookup"><span data-stu-id="5e109-119">position</span></span>|<span data-ttu-id="5e109-120">string</span><span class="sxs-lookup"><span data-stu-id="5e109-120">string</span></span>|<span data-ttu-id="5e109-121">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="5e109-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="5e109-122">`None`Возможные значения:, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`,. `Callout`</span><span class="sxs-lookup"><span data-stu-id="5e109-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="5e109-123">separator</span><span class="sxs-lookup"><span data-stu-id="5e109-123">separator</span></span>|<span data-ttu-id="5e109-124">string</span><span class="sxs-lookup"><span data-stu-id="5e109-124">string</span></span>|<span data-ttu-id="5e109-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="5e109-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="5e109-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="5e109-126">showBubbleSize</span></span>|<span data-ttu-id="5e109-127">boolean</span><span class="sxs-lookup"><span data-stu-id="5e109-127">boolean</span></span>|<span data-ttu-id="5e109-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="5e109-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="5e109-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="5e109-129">showCategoryName</span></span>|<span data-ttu-id="5e109-130">boolean</span><span class="sxs-lookup"><span data-stu-id="5e109-130">boolean</span></span>|<span data-ttu-id="5e109-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="5e109-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="5e109-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="5e109-132">showLegendKey</span></span>|<span data-ttu-id="5e109-133">boolean</span><span class="sxs-lookup"><span data-stu-id="5e109-133">boolean</span></span>|<span data-ttu-id="5e109-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="5e109-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="5e109-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="5e109-135">showPercentage</span></span>|<span data-ttu-id="5e109-136">boolean</span><span class="sxs-lookup"><span data-stu-id="5e109-136">boolean</span></span>|<span data-ttu-id="5e109-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="5e109-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="5e109-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="5e109-138">showSeriesName</span></span>|<span data-ttu-id="5e109-139">boolean</span><span class="sxs-lookup"><span data-stu-id="5e109-139">boolean</span></span>|<span data-ttu-id="5e109-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="5e109-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="5e109-141">showValue</span><span class="sxs-lookup"><span data-stu-id="5e109-141">showValue</span></span>|<span data-ttu-id="5e109-142">boolean</span><span class="sxs-lookup"><span data-stu-id="5e109-142">boolean</span></span>|<span data-ttu-id="5e109-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="5e109-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e109-144">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e109-144">Relationships</span></span>
| <span data-ttu-id="5e109-145">Отношение</span><span class="sxs-lookup"><span data-stu-id="5e109-145">Relationship</span></span> | <span data-ttu-id="5e109-146">Тип</span><span class="sxs-lookup"><span data-stu-id="5e109-146">Type</span></span>   |<span data-ttu-id="5e109-147">Описание</span><span class="sxs-lookup"><span data-stu-id="5e109-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e109-148">format</span><span class="sxs-lookup"><span data-stu-id="5e109-148">format</span></span>|[<span data-ttu-id="5e109-149">Воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="5e109-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="5e109-150">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов.</span><span class="sxs-lookup"><span data-stu-id="5e109-150">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="5e109-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e109-151">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e109-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e109-152">JSON representation</span></span>

<span data-ttu-id="5e109-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e109-153">Here is a JSON representation of the resource.</span></span>

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
