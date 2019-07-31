---
title: Тип ресурса Воркбукчартдаталабелс
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c5e469f5d95065fa3b5a161d510ca023e17f807a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007293"
---
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="3769c-103">Тип ресурса Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="3769c-103">workbookChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3769c-104">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3769c-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="3769c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3769c-105">Methods</span></span>

| <span data-ttu-id="3769c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3769c-106">Method</span></span>           | <span data-ttu-id="3769c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3769c-107">Return Type</span></span>    |<span data-ttu-id="3769c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3769c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3769c-109">Получение Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="3769c-109">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="3769c-110">Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="3769c-110">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="3769c-111">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="3769c-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="3769c-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="3769c-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="3769c-113">Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="3769c-113">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="3769c-114">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="3769c-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3769c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="3769c-115">Properties</span></span>
| <span data-ttu-id="3769c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="3769c-116">Property</span></span>     | <span data-ttu-id="3769c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="3769c-117">Type</span></span>   |<span data-ttu-id="3769c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="3769c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3769c-119">position</span><span class="sxs-lookup"><span data-stu-id="3769c-119">position</span></span>|<span data-ttu-id="3769c-120">string</span><span class="sxs-lookup"><span data-stu-id="3769c-120">string</span></span>|<span data-ttu-id="3769c-121">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="3769c-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="3769c-122">`None`Возможные значения:, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`,. `Callout`</span><span class="sxs-lookup"><span data-stu-id="3769c-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="3769c-123">separator</span><span class="sxs-lookup"><span data-stu-id="3769c-123">separator</span></span>|<span data-ttu-id="3769c-124">string</span><span class="sxs-lookup"><span data-stu-id="3769c-124">string</span></span>|<span data-ttu-id="3769c-125">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="3769c-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="3769c-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="3769c-126">showBubbleSize</span></span>|<span data-ttu-id="3769c-127">boolean</span><span class="sxs-lookup"><span data-stu-id="3769c-127">boolean</span></span>|<span data-ttu-id="3769c-128">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="3769c-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="3769c-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="3769c-129">showCategoryName</span></span>|<span data-ttu-id="3769c-130">boolean</span><span class="sxs-lookup"><span data-stu-id="3769c-130">boolean</span></span>|<span data-ttu-id="3769c-131">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="3769c-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="3769c-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="3769c-132">showLegendKey</span></span>|<span data-ttu-id="3769c-133">boolean</span><span class="sxs-lookup"><span data-stu-id="3769c-133">boolean</span></span>|<span data-ttu-id="3769c-134">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="3769c-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="3769c-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="3769c-135">showPercentage</span></span>|<span data-ttu-id="3769c-136">boolean</span><span class="sxs-lookup"><span data-stu-id="3769c-136">boolean</span></span>|<span data-ttu-id="3769c-137">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="3769c-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="3769c-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="3769c-138">showSeriesName</span></span>|<span data-ttu-id="3769c-139">boolean</span><span class="sxs-lookup"><span data-stu-id="3769c-139">boolean</span></span>|<span data-ttu-id="3769c-140">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="3769c-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="3769c-141">showValue</span><span class="sxs-lookup"><span data-stu-id="3769c-141">showValue</span></span>|<span data-ttu-id="3769c-142">boolean</span><span class="sxs-lookup"><span data-stu-id="3769c-142">boolean</span></span>|<span data-ttu-id="3769c-143">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="3769c-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3769c-144">Отношения</span><span class="sxs-lookup"><span data-stu-id="3769c-144">Relationships</span></span>
| <span data-ttu-id="3769c-145">Отношение</span><span class="sxs-lookup"><span data-stu-id="3769c-145">Relationship</span></span> | <span data-ttu-id="3769c-146">Тип</span><span class="sxs-lookup"><span data-stu-id="3769c-146">Type</span></span>   |<span data-ttu-id="3769c-147">Описание</span><span class="sxs-lookup"><span data-stu-id="3769c-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3769c-148">format</span><span class="sxs-lookup"><span data-stu-id="3769c-148">format</span></span>|[<span data-ttu-id="3769c-149">Воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="3769c-149">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="3769c-150">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов.</span><span class="sxs-lookup"><span data-stu-id="3769c-150">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="3769c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3769c-151">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3769c-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3769c-152">JSON representation</span></span>

<span data-ttu-id="3769c-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3769c-153">Here is a JSON representation of the resource.</span></span>

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
