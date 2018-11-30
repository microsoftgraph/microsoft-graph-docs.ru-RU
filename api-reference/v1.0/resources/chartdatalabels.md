---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
ms.openlocfilehash: f8cb4310ab9ca2e59325fbc4bd255ae161cc7892
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024738"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="c763d-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="c763d-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="c763d-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c763d-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="c763d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c763d-105">Methods</span></span>

| <span data-ttu-id="c763d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c763d-106">Method</span></span>           | <span data-ttu-id="c763d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c763d-107">Return Type</span></span>    |<span data-ttu-id="c763d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c763d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c763d-109">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="c763d-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="c763d-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="c763d-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="c763d-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="c763d-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="c763d-112">Update</span><span class="sxs-lookup"><span data-stu-id="c763d-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="c763d-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="c763d-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="c763d-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="c763d-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c763d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="c763d-115">Properties</span></span>
| <span data-ttu-id="c763d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="c763d-116">Property</span></span>     | <span data-ttu-id="c763d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c763d-117">Type</span></span>   |<span data-ttu-id="c763d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c763d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c763d-119">position</span><span class="sxs-lookup"><span data-stu-id="c763d-119">position</span></span>|<span data-ttu-id="c763d-120">string</span><span class="sxs-lookup"><span data-stu-id="c763d-120">string</span></span>|<span data-ttu-id="c763d-121">DataLabelPosition значение, представляющее положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="c763d-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="c763d-122">Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="c763d-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="c763d-123">разделитель</span><span class="sxs-lookup"><span data-stu-id="c763d-123">separator</span></span>|<span data-ttu-id="c763d-124">string</span><span class="sxs-lookup"><span data-stu-id="c763d-124">string</span></span>|<span data-ttu-id="c763d-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="c763d-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="c763d-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="c763d-126">showBubbleSize</span></span>|<span data-ttu-id="c763d-127">boolean</span><span class="sxs-lookup"><span data-stu-id="c763d-127">boolean</span></span>|<span data-ttu-id="c763d-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="c763d-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="c763d-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="c763d-129">showCategoryName</span></span>|<span data-ttu-id="c763d-130">boolean</span><span class="sxs-lookup"><span data-stu-id="c763d-130">boolean</span></span>|<span data-ttu-id="c763d-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="c763d-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="c763d-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="c763d-132">showLegendKey</span></span>|<span data-ttu-id="c763d-133">boolean</span><span class="sxs-lookup"><span data-stu-id="c763d-133">boolean</span></span>|<span data-ttu-id="c763d-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="c763d-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="c763d-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="c763d-135">showPercentage</span></span>|<span data-ttu-id="c763d-136">boolean</span><span class="sxs-lookup"><span data-stu-id="c763d-136">boolean</span></span>|<span data-ttu-id="c763d-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="c763d-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="c763d-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="c763d-138">showSeriesName</span></span>|<span data-ttu-id="c763d-139">boolean</span><span class="sxs-lookup"><span data-stu-id="c763d-139">boolean</span></span>|<span data-ttu-id="c763d-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="c763d-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="c763d-141">showValue</span><span class="sxs-lookup"><span data-stu-id="c763d-141">showValue</span></span>|<span data-ttu-id="c763d-142">boolean</span><span class="sxs-lookup"><span data-stu-id="c763d-142">boolean</span></span>|<span data-ttu-id="c763d-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="c763d-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c763d-144">Связи</span><span class="sxs-lookup"><span data-stu-id="c763d-144">Relationships</span></span>
| <span data-ttu-id="c763d-145">Связь</span><span class="sxs-lookup"><span data-stu-id="c763d-145">Relationship</span></span> | <span data-ttu-id="c763d-146">Тип</span><span class="sxs-lookup"><span data-stu-id="c763d-146">Type</span></span>   |<span data-ttu-id="c763d-147">Описание</span><span class="sxs-lookup"><span data-stu-id="c763d-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c763d-148">format</span><span class="sxs-lookup"><span data-stu-id="c763d-148">format</span></span>|[<span data-ttu-id="c763d-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="c763d-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="c763d-p102">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c763d-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c763d-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c763d-152">JSON representation</span></span>

<span data-ttu-id="c763d-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c763d-153">Here is a JSON representation of the resource.</span></span>

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