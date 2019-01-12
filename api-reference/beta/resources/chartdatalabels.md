---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 16e2e3acafc98a4066b8620f41f15c7cae1667cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954682"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="348d7-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="348d7-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="348d7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="348d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="348d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="348d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="348d7-106">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="348d7-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="348d7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="348d7-107">Methods</span></span>

| <span data-ttu-id="348d7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="348d7-108">Method</span></span>           | <span data-ttu-id="348d7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="348d7-109">Return Type</span></span>    |<span data-ttu-id="348d7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="348d7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="348d7-111">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="348d7-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="348d7-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="348d7-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="348d7-113">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="348d7-113">Read properties and relationships of chartDataLabels object.</span></span>|
|<span data-ttu-id="348d7-114">[обновление](../api/chartdatalabels-update.md).</span><span class="sxs-lookup"><span data-stu-id="348d7-114">[Update](../api/chartdatalabels-update.md)</span></span> | [<span data-ttu-id="348d7-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="348d7-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="348d7-116">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="348d7-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="348d7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="348d7-117">Properties</span></span>
| <span data-ttu-id="348d7-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="348d7-118">Property</span></span>     | <span data-ttu-id="348d7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="348d7-119">Type</span></span>   |<span data-ttu-id="348d7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="348d7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="348d7-121">position</span><span class="sxs-lookup"><span data-stu-id="348d7-121">position</span></span>|<span data-ttu-id="348d7-122">string</span><span class="sxs-lookup"><span data-stu-id="348d7-122">string</span></span>|<span data-ttu-id="348d7-p102">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="348d7-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="348d7-125">разделитель</span><span class="sxs-lookup"><span data-stu-id="348d7-125">separator</span></span>|<span data-ttu-id="348d7-126">string</span><span class="sxs-lookup"><span data-stu-id="348d7-126">string</span></span>|<span data-ttu-id="348d7-127">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="348d7-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="348d7-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="348d7-128">showBubbleSize</span></span>|<span data-ttu-id="348d7-129">boolean</span><span class="sxs-lookup"><span data-stu-id="348d7-129">boolean</span></span>|<span data-ttu-id="348d7-130">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="348d7-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="348d7-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="348d7-131">showCategoryName</span></span>|<span data-ttu-id="348d7-132">boolean</span><span class="sxs-lookup"><span data-stu-id="348d7-132">boolean</span></span>|<span data-ttu-id="348d7-133">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="348d7-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="348d7-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="348d7-134">showLegendKey</span></span>|<span data-ttu-id="348d7-135">boolean</span><span class="sxs-lookup"><span data-stu-id="348d7-135">boolean</span></span>|<span data-ttu-id="348d7-136">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="348d7-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="348d7-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="348d7-137">showPercentage</span></span>|<span data-ttu-id="348d7-138">boolean</span><span class="sxs-lookup"><span data-stu-id="348d7-138">boolean</span></span>|<span data-ttu-id="348d7-139">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="348d7-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="348d7-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="348d7-140">showSeriesName</span></span>|<span data-ttu-id="348d7-141">boolean</span><span class="sxs-lookup"><span data-stu-id="348d7-141">boolean</span></span>|<span data-ttu-id="348d7-142">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="348d7-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="348d7-143">showValue</span><span class="sxs-lookup"><span data-stu-id="348d7-143">showValue</span></span>|<span data-ttu-id="348d7-144">boolean</span><span class="sxs-lookup"><span data-stu-id="348d7-144">boolean</span></span>|<span data-ttu-id="348d7-145">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="348d7-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="348d7-146">Связи</span><span class="sxs-lookup"><span data-stu-id="348d7-146">Relationships</span></span>
| <span data-ttu-id="348d7-147">Связь</span><span class="sxs-lookup"><span data-stu-id="348d7-147">Relationship</span></span> | <span data-ttu-id="348d7-148">Тип</span><span class="sxs-lookup"><span data-stu-id="348d7-148">Type</span></span>   |<span data-ttu-id="348d7-149">Описание</span><span class="sxs-lookup"><span data-stu-id="348d7-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="348d7-150">format</span><span class="sxs-lookup"><span data-stu-id="348d7-150">format</span></span>|[<span data-ttu-id="348d7-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="348d7-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="348d7-p103">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="348d7-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="348d7-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="348d7-154">JSON representation</span></span>

<span data-ttu-id="348d7-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="348d7-155">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
