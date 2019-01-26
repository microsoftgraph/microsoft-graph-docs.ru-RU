---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f722dccd84d1861ff47e0aa073fe66f50372ad4f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576404"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="7c067-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="7c067-103">ChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c067-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7c067-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="7c067-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7c067-105">Methods</span></span>

| <span data-ttu-id="7c067-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7c067-106">Method</span></span>           | <span data-ttu-id="7c067-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c067-107">Return Type</span></span>    |<span data-ttu-id="7c067-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c067-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c067-109">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="7c067-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="7c067-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="7c067-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="7c067-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="7c067-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="7c067-112">Update</span><span class="sxs-lookup"><span data-stu-id="7c067-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="7c067-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="7c067-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="7c067-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="7c067-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7c067-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c067-115">Properties</span></span>
| <span data-ttu-id="7c067-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c067-116">Property</span></span>     | <span data-ttu-id="7c067-117">Тип</span><span class="sxs-lookup"><span data-stu-id="7c067-117">Type</span></span>   |<span data-ttu-id="7c067-118">Описание</span><span class="sxs-lookup"><span data-stu-id="7c067-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c067-119">position</span><span class="sxs-lookup"><span data-stu-id="7c067-119">position</span></span>|<span data-ttu-id="7c067-120">string</span><span class="sxs-lookup"><span data-stu-id="7c067-120">string</span></span>|<span data-ttu-id="7c067-121">DataLabelPosition значение, представляющее положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="7c067-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="7c067-122">Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="7c067-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="7c067-123">разделитель</span><span class="sxs-lookup"><span data-stu-id="7c067-123">separator</span></span>|<span data-ttu-id="7c067-124">string</span><span class="sxs-lookup"><span data-stu-id="7c067-124">string</span></span>|<span data-ttu-id="7c067-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="7c067-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="7c067-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="7c067-126">showBubbleSize</span></span>|<span data-ttu-id="7c067-127">boolean</span><span class="sxs-lookup"><span data-stu-id="7c067-127">boolean</span></span>|<span data-ttu-id="7c067-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="7c067-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="7c067-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="7c067-129">showCategoryName</span></span>|<span data-ttu-id="7c067-130">boolean</span><span class="sxs-lookup"><span data-stu-id="7c067-130">boolean</span></span>|<span data-ttu-id="7c067-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="7c067-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="7c067-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="7c067-132">showLegendKey</span></span>|<span data-ttu-id="7c067-133">boolean</span><span class="sxs-lookup"><span data-stu-id="7c067-133">boolean</span></span>|<span data-ttu-id="7c067-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="7c067-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="7c067-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="7c067-135">showPercentage</span></span>|<span data-ttu-id="7c067-136">boolean</span><span class="sxs-lookup"><span data-stu-id="7c067-136">boolean</span></span>|<span data-ttu-id="7c067-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="7c067-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="7c067-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="7c067-138">showSeriesName</span></span>|<span data-ttu-id="7c067-139">boolean</span><span class="sxs-lookup"><span data-stu-id="7c067-139">boolean</span></span>|<span data-ttu-id="7c067-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="7c067-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="7c067-141">showValue</span><span class="sxs-lookup"><span data-stu-id="7c067-141">showValue</span></span>|<span data-ttu-id="7c067-142">boolean</span><span class="sxs-lookup"><span data-stu-id="7c067-142">boolean</span></span>|<span data-ttu-id="7c067-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="7c067-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c067-144">Связи</span><span class="sxs-lookup"><span data-stu-id="7c067-144">Relationships</span></span>
| <span data-ttu-id="7c067-145">Связь</span><span class="sxs-lookup"><span data-stu-id="7c067-145">Relationship</span></span> | <span data-ttu-id="7c067-146">Тип</span><span class="sxs-lookup"><span data-stu-id="7c067-146">Type</span></span>   |<span data-ttu-id="7c067-147">Описание</span><span class="sxs-lookup"><span data-stu-id="7c067-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c067-148">format</span><span class="sxs-lookup"><span data-stu-id="7c067-148">format</span></span>|[<span data-ttu-id="7c067-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="7c067-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="7c067-p102">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c067-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c067-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c067-152">JSON representation</span></span>

<span data-ttu-id="7c067-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c067-153">Here is a JSON representation of the resource.</span></span>

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
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabels.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
