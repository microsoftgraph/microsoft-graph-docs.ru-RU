---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bda2c1849f154435608f311671026e224b0c7e3c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510339"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="5a936-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5a936-103">ChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a936-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5a936-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="5a936-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5a936-105">Methods</span></span>

| <span data-ttu-id="5a936-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5a936-106">Method</span></span>           | <span data-ttu-id="5a936-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a936-107">Return Type</span></span>    |<span data-ttu-id="5a936-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5a936-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a936-109">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5a936-109">[Get ChartDataLabels](../api/chartdatalabels-get.md)</span></span> | [<span data-ttu-id="5a936-110">chartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5a936-110">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="5a936-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5a936-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="5a936-112">Update</span><span class="sxs-lookup"><span data-stu-id="5a936-112">Update</span></span>](../api/chartdatalabels-update.md) | <span data-ttu-id="5a936-113">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="5a936-113">[ChartDataLabels](chartdatalabels.md)</span></span> |<span data-ttu-id="5a936-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="5a936-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a936-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a936-115">Properties</span></span>
| <span data-ttu-id="5a936-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a936-116">Property</span></span>     | <span data-ttu-id="5a936-117">Тип</span><span class="sxs-lookup"><span data-stu-id="5a936-117">Type</span></span>   |<span data-ttu-id="5a936-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5a936-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a936-119">position</span><span class="sxs-lookup"><span data-stu-id="5a936-119">position</span></span>|<span data-ttu-id="5a936-120">string</span><span class="sxs-lookup"><span data-stu-id="5a936-120">string</span></span>|<span data-ttu-id="5a936-p101">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="5a936-p101">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="5a936-123">разделитель</span><span class="sxs-lookup"><span data-stu-id="5a936-123">separator</span></span>|<span data-ttu-id="5a936-124">string</span><span class="sxs-lookup"><span data-stu-id="5a936-124">string</span></span>|<span data-ttu-id="5a936-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="5a936-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="5a936-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="5a936-126">showBubbleSize</span></span>|<span data-ttu-id="5a936-127">boolean</span><span class="sxs-lookup"><span data-stu-id="5a936-127">boolean</span></span>|<span data-ttu-id="5a936-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="5a936-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="5a936-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="5a936-129">showCategoryName</span></span>|<span data-ttu-id="5a936-130">boolean</span><span class="sxs-lookup"><span data-stu-id="5a936-130">boolean</span></span>|<span data-ttu-id="5a936-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="5a936-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="5a936-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="5a936-132">showLegendKey</span></span>|<span data-ttu-id="5a936-133">boolean</span><span class="sxs-lookup"><span data-stu-id="5a936-133">boolean</span></span>|<span data-ttu-id="5a936-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="5a936-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="5a936-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="5a936-135">showPercentage</span></span>|<span data-ttu-id="5a936-136">boolean</span><span class="sxs-lookup"><span data-stu-id="5a936-136">boolean</span></span>|<span data-ttu-id="5a936-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="5a936-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="5a936-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="5a936-138">showSeriesName</span></span>|<span data-ttu-id="5a936-139">boolean</span><span class="sxs-lookup"><span data-stu-id="5a936-139">boolean</span></span>|<span data-ttu-id="5a936-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="5a936-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="5a936-141">showValue</span><span class="sxs-lookup"><span data-stu-id="5a936-141">showValue</span></span>|<span data-ttu-id="5a936-142">boolean</span><span class="sxs-lookup"><span data-stu-id="5a936-142">boolean</span></span>|<span data-ttu-id="5a936-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="5a936-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a936-144">Связи</span><span class="sxs-lookup"><span data-stu-id="5a936-144">Relationships</span></span>
| <span data-ttu-id="5a936-145">Связь</span><span class="sxs-lookup"><span data-stu-id="5a936-145">Relationship</span></span> | <span data-ttu-id="5a936-146">Тип</span><span class="sxs-lookup"><span data-stu-id="5a936-146">Type</span></span>   |<span data-ttu-id="5a936-147">Описание</span><span class="sxs-lookup"><span data-stu-id="5a936-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a936-148">format</span><span class="sxs-lookup"><span data-stu-id="5a936-148">format</span></span>|[<span data-ttu-id="5a936-149">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="5a936-149">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="5a936-p102">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a936-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a936-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a936-152">JSON representation</span></span>

<span data-ttu-id="5a936-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a936-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
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
