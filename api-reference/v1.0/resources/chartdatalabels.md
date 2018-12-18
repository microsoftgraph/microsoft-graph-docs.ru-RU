---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
ms.openlocfilehash: 39c95d0849d398df7d57f676cc392c157e6f43f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339055"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="8d2cf-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8d2cf-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="8d2cf-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="8d2cf-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8d2cf-105">Methods</span></span>

| <span data-ttu-id="8d2cf-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8d2cf-106">Method</span></span>           | <span data-ttu-id="8d2cf-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8d2cf-107">Return Type</span></span>    |<span data-ttu-id="8d2cf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8d2cf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d2cf-109">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8d2cf-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="8d2cf-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8d2cf-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="8d2cf-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-111">Read properties and relationships of chartDataLabels object.</span></span>|
|<span data-ttu-id="8d2cf-112">[обновление](../api/chartdatalabels-update.md).</span><span class="sxs-lookup"><span data-stu-id="8d2cf-112">[Update](../api/chartdatalabels-update.md)</span></span> | [<span data-ttu-id="8d2cf-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8d2cf-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="8d2cf-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d2cf-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d2cf-115">Properties</span></span>
| <span data-ttu-id="8d2cf-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d2cf-116">Property</span></span>     | <span data-ttu-id="8d2cf-117">Тип</span><span class="sxs-lookup"><span data-stu-id="8d2cf-117">Type</span></span>   |<span data-ttu-id="8d2cf-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8d2cf-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d2cf-119">position</span><span class="sxs-lookup"><span data-stu-id="8d2cf-119">position</span></span>|<span data-ttu-id="8d2cf-120">string</span><span class="sxs-lookup"><span data-stu-id="8d2cf-120">string</span></span>|<span data-ttu-id="8d2cf-121">DataLabelPosition значение, представляющее положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="8d2cf-122">Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="8d2cf-123">разделитель</span><span class="sxs-lookup"><span data-stu-id="8d2cf-123">separator</span></span>|<span data-ttu-id="8d2cf-124">string</span><span class="sxs-lookup"><span data-stu-id="8d2cf-124">string</span></span>|<span data-ttu-id="8d2cf-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="8d2cf-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="8d2cf-126">showBubbleSize</span></span>|<span data-ttu-id="8d2cf-127">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2cf-127">boolean</span></span>|<span data-ttu-id="8d2cf-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="8d2cf-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="8d2cf-129">showCategoryName</span></span>|<span data-ttu-id="8d2cf-130">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2cf-130">boolean</span></span>|<span data-ttu-id="8d2cf-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="8d2cf-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="8d2cf-132">showLegendKey</span></span>|<span data-ttu-id="8d2cf-133">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2cf-133">boolean</span></span>|<span data-ttu-id="8d2cf-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="8d2cf-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="8d2cf-135">showPercentage</span></span>|<span data-ttu-id="8d2cf-136">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2cf-136">boolean</span></span>|<span data-ttu-id="8d2cf-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="8d2cf-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="8d2cf-138">showSeriesName</span></span>|<span data-ttu-id="8d2cf-139">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2cf-139">boolean</span></span>|<span data-ttu-id="8d2cf-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="8d2cf-141">showValue</span><span class="sxs-lookup"><span data-stu-id="8d2cf-141">showValue</span></span>|<span data-ttu-id="8d2cf-142">boolean</span><span class="sxs-lookup"><span data-stu-id="8d2cf-142">boolean</span></span>|<span data-ttu-id="8d2cf-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d2cf-144">Связи</span><span class="sxs-lookup"><span data-stu-id="8d2cf-144">Relationships</span></span>
| <span data-ttu-id="8d2cf-145">Связь</span><span class="sxs-lookup"><span data-stu-id="8d2cf-145">Relationship</span></span> | <span data-ttu-id="8d2cf-146">Тип</span><span class="sxs-lookup"><span data-stu-id="8d2cf-146">Type</span></span>   |<span data-ttu-id="8d2cf-147">Описание</span><span class="sxs-lookup"><span data-stu-id="8d2cf-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d2cf-148">format</span><span class="sxs-lookup"><span data-stu-id="8d2cf-148">format</span></span>|[<span data-ttu-id="8d2cf-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="8d2cf-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="8d2cf-p102">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d2cf-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d2cf-152">JSON representation</span></span>

<span data-ttu-id="8d2cf-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d2cf-153">Here is a JSON representation of the resource.</span></span>

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