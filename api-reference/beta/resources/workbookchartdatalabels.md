---
title: Тип ресурса Воркбукчартдаталабелс
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c3521274b93d33780539c04643c5c0225fdecef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348936"
---
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="f0cce-103">Тип ресурса Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="f0cce-103">workbookChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0cce-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f0cce-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="f0cce-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f0cce-105">Methods</span></span>

| <span data-ttu-id="f0cce-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f0cce-106">Method</span></span>           | <span data-ttu-id="f0cce-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f0cce-107">Return Type</span></span>    |<span data-ttu-id="f0cce-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f0cce-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0cce-109">Получение Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="f0cce-109">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="f0cce-110">Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="f0cce-110">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="f0cce-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="f0cce-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="f0cce-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="f0cce-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="f0cce-113">Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="f0cce-113">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="f0cce-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="f0cce-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f0cce-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0cce-115">Properties</span></span>
| <span data-ttu-id="f0cce-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0cce-116">Property</span></span>     | <span data-ttu-id="f0cce-117">Тип</span><span class="sxs-lookup"><span data-stu-id="f0cce-117">Type</span></span>   |<span data-ttu-id="f0cce-118">Описание</span><span class="sxs-lookup"><span data-stu-id="f0cce-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0cce-119">position</span><span class="sxs-lookup"><span data-stu-id="f0cce-119">position</span></span>|<span data-ttu-id="f0cce-120">string</span><span class="sxs-lookup"><span data-stu-id="f0cce-120">string</span></span>|<span data-ttu-id="f0cce-121">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="f0cce-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="f0cce-122">`None`Возможные значения:, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`,. `Callout`</span><span class="sxs-lookup"><span data-stu-id="f0cce-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="f0cce-123">separator</span><span class="sxs-lookup"><span data-stu-id="f0cce-123">separator</span></span>|<span data-ttu-id="f0cce-124">string</span><span class="sxs-lookup"><span data-stu-id="f0cce-124">string</span></span>|<span data-ttu-id="f0cce-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="f0cce-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="f0cce-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="f0cce-126">showBubbleSize</span></span>|<span data-ttu-id="f0cce-127">boolean</span><span class="sxs-lookup"><span data-stu-id="f0cce-127">boolean</span></span>|<span data-ttu-id="f0cce-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="f0cce-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="f0cce-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="f0cce-129">showCategoryName</span></span>|<span data-ttu-id="f0cce-130">boolean</span><span class="sxs-lookup"><span data-stu-id="f0cce-130">boolean</span></span>|<span data-ttu-id="f0cce-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="f0cce-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="f0cce-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="f0cce-132">showLegendKey</span></span>|<span data-ttu-id="f0cce-133">boolean</span><span class="sxs-lookup"><span data-stu-id="f0cce-133">boolean</span></span>|<span data-ttu-id="f0cce-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="f0cce-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="f0cce-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="f0cce-135">showPercentage</span></span>|<span data-ttu-id="f0cce-136">boolean</span><span class="sxs-lookup"><span data-stu-id="f0cce-136">boolean</span></span>|<span data-ttu-id="f0cce-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="f0cce-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="f0cce-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="f0cce-138">showSeriesName</span></span>|<span data-ttu-id="f0cce-139">boolean</span><span class="sxs-lookup"><span data-stu-id="f0cce-139">boolean</span></span>|<span data-ttu-id="f0cce-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="f0cce-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="f0cce-141">showValue</span><span class="sxs-lookup"><span data-stu-id="f0cce-141">showValue</span></span>|<span data-ttu-id="f0cce-142">boolean</span><span class="sxs-lookup"><span data-stu-id="f0cce-142">boolean</span></span>|<span data-ttu-id="f0cce-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="f0cce-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0cce-144">Отношения</span><span class="sxs-lookup"><span data-stu-id="f0cce-144">Relationships</span></span>
| <span data-ttu-id="f0cce-145">Отношение</span><span class="sxs-lookup"><span data-stu-id="f0cce-145">Relationship</span></span> | <span data-ttu-id="f0cce-146">Тип</span><span class="sxs-lookup"><span data-stu-id="f0cce-146">Type</span></span>   |<span data-ttu-id="f0cce-147">Описание</span><span class="sxs-lookup"><span data-stu-id="f0cce-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0cce-148">format</span><span class="sxs-lookup"><span data-stu-id="f0cce-148">format</span></span>|[<span data-ttu-id="f0cce-149">Воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="f0cce-149">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="f0cce-150">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов.</span><span class="sxs-lookup"><span data-stu-id="f0cce-150">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="f0cce-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0cce-151">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0cce-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0cce-152">JSON representation</span></span>

<span data-ttu-id="f0cce-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0cce-153">Here is a JSON representation of the resource.</span></span>

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
