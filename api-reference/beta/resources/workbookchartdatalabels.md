---
title: Тип ресурса Воркбукчартдаталабелс
description: Представляет коллекцию всех меток данных в точке диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2e276a3d4e6f958930add9095e8c6c67972bed4f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519346"
---
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="e4906-103">Тип ресурса Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="e4906-103">workbookChartDataLabels resource type</span></span>

<span data-ttu-id="e4906-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e4906-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4906-105">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e4906-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="e4906-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e4906-106">Methods</span></span>

| <span data-ttu-id="e4906-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e4906-107">Method</span></span>           | <span data-ttu-id="e4906-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4906-108">Return Type</span></span>    |<span data-ttu-id="e4906-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e4906-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4906-110">Получение Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="e4906-110">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="e4906-111">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="e4906-111">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="e4906-112">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="e4906-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="e4906-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="e4906-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="e4906-114">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="e4906-114">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="e4906-115">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="e4906-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4906-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4906-116">Properties</span></span>
| <span data-ttu-id="e4906-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4906-117">Property</span></span>     | <span data-ttu-id="e4906-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e4906-118">Type</span></span>   |<span data-ttu-id="e4906-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e4906-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4906-120">position</span><span class="sxs-lookup"><span data-stu-id="e4906-120">position</span></span>|<span data-ttu-id="e4906-121">строка</span><span class="sxs-lookup"><span data-stu-id="e4906-121">string</span></span>|<span data-ttu-id="e4906-122">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="e4906-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="e4906-123">`None`Возможные значения:, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`,. `Callout`</span><span class="sxs-lookup"><span data-stu-id="e4906-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="e4906-124">separator</span><span class="sxs-lookup"><span data-stu-id="e4906-124">separator</span></span>|<span data-ttu-id="e4906-125">string</span><span class="sxs-lookup"><span data-stu-id="e4906-125">string</span></span>|<span data-ttu-id="e4906-126">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="e4906-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="e4906-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="e4906-127">showBubbleSize</span></span>|<span data-ttu-id="e4906-128">boolean</span><span class="sxs-lookup"><span data-stu-id="e4906-128">boolean</span></span>|<span data-ttu-id="e4906-129">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="e4906-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="e4906-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="e4906-130">showCategoryName</span></span>|<span data-ttu-id="e4906-131">boolean</span><span class="sxs-lookup"><span data-stu-id="e4906-131">boolean</span></span>|<span data-ttu-id="e4906-132">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="e4906-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="e4906-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="e4906-133">showLegendKey</span></span>|<span data-ttu-id="e4906-134">boolean</span><span class="sxs-lookup"><span data-stu-id="e4906-134">boolean</span></span>|<span data-ttu-id="e4906-135">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="e4906-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="e4906-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="e4906-136">showPercentage</span></span>|<span data-ttu-id="e4906-137">boolean</span><span class="sxs-lookup"><span data-stu-id="e4906-137">boolean</span></span>|<span data-ttu-id="e4906-138">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="e4906-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="e4906-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="e4906-139">showSeriesName</span></span>|<span data-ttu-id="e4906-140">boolean</span><span class="sxs-lookup"><span data-stu-id="e4906-140">boolean</span></span>|<span data-ttu-id="e4906-141">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="e4906-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="e4906-142">showValue</span><span class="sxs-lookup"><span data-stu-id="e4906-142">showValue</span></span>|<span data-ttu-id="e4906-143">boolean</span><span class="sxs-lookup"><span data-stu-id="e4906-143">boolean</span></span>|<span data-ttu-id="e4906-144">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="e4906-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4906-145">Связи</span><span class="sxs-lookup"><span data-stu-id="e4906-145">Relationships</span></span>
| <span data-ttu-id="e4906-146">Связь</span><span class="sxs-lookup"><span data-stu-id="e4906-146">Relationship</span></span> | <span data-ttu-id="e4906-147">Тип</span><span class="sxs-lookup"><span data-stu-id="e4906-147">Type</span></span>   |<span data-ttu-id="e4906-148">Описание</span><span class="sxs-lookup"><span data-stu-id="e4906-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4906-149">format</span><span class="sxs-lookup"><span data-stu-id="e4906-149">format</span></span>|[<span data-ttu-id="e4906-150">воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="e4906-150">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="e4906-151">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов.</span><span class="sxs-lookup"><span data-stu-id="e4906-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="e4906-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e4906-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4906-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4906-153">JSON representation</span></span>

<span data-ttu-id="e4906-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4906-154">Here is a JSON representation of the resource.</span></span>

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
