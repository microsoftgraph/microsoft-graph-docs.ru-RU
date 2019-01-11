---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7e45db4129422c32af809d46c076b2f6d82eff89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876197"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="a135b-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="a135b-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="a135b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a135b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a135b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a135b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a135b-106">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a135b-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="a135b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a135b-107">Methods</span></span>

| <span data-ttu-id="a135b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a135b-108">Method</span></span>           | <span data-ttu-id="a135b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a135b-109">Return Type</span></span>    |<span data-ttu-id="a135b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a135b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a135b-111">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="a135b-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="a135b-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="a135b-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="a135b-113">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="a135b-113">Read properties and relationships of chartDataLabels object.</span></span>|
|<span data-ttu-id="a135b-114">[обновление](../api/chartdatalabels-update.md).</span><span class="sxs-lookup"><span data-stu-id="a135b-114">[Update](../api/chartdatalabels-update.md)</span></span> | [<span data-ttu-id="a135b-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="a135b-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="a135b-116">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="a135b-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a135b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="a135b-117">Properties</span></span>
| <span data-ttu-id="a135b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="a135b-118">Property</span></span>     | <span data-ttu-id="a135b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a135b-119">Type</span></span>   |<span data-ttu-id="a135b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a135b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a135b-121">position</span><span class="sxs-lookup"><span data-stu-id="a135b-121">position</span></span>|<span data-ttu-id="a135b-122">string</span><span class="sxs-lookup"><span data-stu-id="a135b-122">string</span></span>|<span data-ttu-id="a135b-p102">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="a135b-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="a135b-125">разделитель</span><span class="sxs-lookup"><span data-stu-id="a135b-125">separator</span></span>|<span data-ttu-id="a135b-126">string</span><span class="sxs-lookup"><span data-stu-id="a135b-126">string</span></span>|<span data-ttu-id="a135b-127">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="a135b-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="a135b-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="a135b-128">showBubbleSize</span></span>|<span data-ttu-id="a135b-129">boolean</span><span class="sxs-lookup"><span data-stu-id="a135b-129">boolean</span></span>|<span data-ttu-id="a135b-130">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="a135b-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="a135b-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="a135b-131">showCategoryName</span></span>|<span data-ttu-id="a135b-132">boolean</span><span class="sxs-lookup"><span data-stu-id="a135b-132">boolean</span></span>|<span data-ttu-id="a135b-133">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="a135b-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="a135b-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="a135b-134">showLegendKey</span></span>|<span data-ttu-id="a135b-135">boolean</span><span class="sxs-lookup"><span data-stu-id="a135b-135">boolean</span></span>|<span data-ttu-id="a135b-136">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="a135b-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="a135b-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="a135b-137">showPercentage</span></span>|<span data-ttu-id="a135b-138">boolean</span><span class="sxs-lookup"><span data-stu-id="a135b-138">boolean</span></span>|<span data-ttu-id="a135b-139">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="a135b-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="a135b-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="a135b-140">showSeriesName</span></span>|<span data-ttu-id="a135b-141">boolean</span><span class="sxs-lookup"><span data-stu-id="a135b-141">boolean</span></span>|<span data-ttu-id="a135b-142">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="a135b-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="a135b-143">showValue</span><span class="sxs-lookup"><span data-stu-id="a135b-143">showValue</span></span>|<span data-ttu-id="a135b-144">boolean</span><span class="sxs-lookup"><span data-stu-id="a135b-144">boolean</span></span>|<span data-ttu-id="a135b-145">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="a135b-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a135b-146">Связи</span><span class="sxs-lookup"><span data-stu-id="a135b-146">Relationships</span></span>
| <span data-ttu-id="a135b-147">Связь</span><span class="sxs-lookup"><span data-stu-id="a135b-147">Relationship</span></span> | <span data-ttu-id="a135b-148">Тип</span><span class="sxs-lookup"><span data-stu-id="a135b-148">Type</span></span>   |<span data-ttu-id="a135b-149">Описание</span><span class="sxs-lookup"><span data-stu-id="a135b-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a135b-150">format</span><span class="sxs-lookup"><span data-stu-id="a135b-150">format</span></span>|[<span data-ttu-id="a135b-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="a135b-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="a135b-p103">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a135b-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a135b-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a135b-154">JSON representation</span></span>

<span data-ttu-id="a135b-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a135b-155">Here is a JSON representation of the resource.</span></span>

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
