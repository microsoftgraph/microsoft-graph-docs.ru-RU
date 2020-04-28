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
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="89562-103">Тип ресурса Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="89562-103">workbookChartDataLabels resource type</span></span>

<span data-ttu-id="89562-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89562-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89562-105">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="89562-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="89562-106">Методы</span><span class="sxs-lookup"><span data-stu-id="89562-106">Methods</span></span>

| <span data-ttu-id="89562-107">Метод</span><span class="sxs-lookup"><span data-stu-id="89562-107">Method</span></span>           | <span data-ttu-id="89562-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89562-108">Return Type</span></span>    |<span data-ttu-id="89562-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89562-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89562-110">Получение Воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="89562-110">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="89562-111">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="89562-111">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="89562-112">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="89562-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="89562-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="89562-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="89562-114">воркбукчартдаталабелс</span><span class="sxs-lookup"><span data-stu-id="89562-114">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="89562-115">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="89562-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="89562-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="89562-116">Properties</span></span>
| <span data-ttu-id="89562-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="89562-117">Property</span></span>     | <span data-ttu-id="89562-118">Тип</span><span class="sxs-lookup"><span data-stu-id="89562-118">Type</span></span>   |<span data-ttu-id="89562-119">Описание</span><span class="sxs-lookup"><span data-stu-id="89562-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89562-120">position</span><span class="sxs-lookup"><span data-stu-id="89562-120">position</span></span>|<span data-ttu-id="89562-121">string</span><span class="sxs-lookup"><span data-stu-id="89562-121">string</span></span>|<span data-ttu-id="89562-122">Значение DataLabelPosition, которое представляет положение метки данных.</span><span class="sxs-lookup"><span data-stu-id="89562-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="89562-123">`None`Возможные значения:, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`,. `Callout`</span><span class="sxs-lookup"><span data-stu-id="89562-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="89562-124">separator</span><span class="sxs-lookup"><span data-stu-id="89562-124">separator</span></span>|<span data-ttu-id="89562-125">string</span><span class="sxs-lookup"><span data-stu-id="89562-125">string</span></span>|<span data-ttu-id="89562-126">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="89562-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="89562-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="89562-127">showBubbleSize</span></span>|<span data-ttu-id="89562-128">boolean</span><span class="sxs-lookup"><span data-stu-id="89562-128">boolean</span></span>|<span data-ttu-id="89562-129">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="89562-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="89562-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="89562-130">showCategoryName</span></span>|<span data-ttu-id="89562-131">boolean</span><span class="sxs-lookup"><span data-stu-id="89562-131">boolean</span></span>|<span data-ttu-id="89562-132">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="89562-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="89562-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="89562-133">showLegendKey</span></span>|<span data-ttu-id="89562-134">boolean</span><span class="sxs-lookup"><span data-stu-id="89562-134">boolean</span></span>|<span data-ttu-id="89562-135">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="89562-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="89562-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="89562-136">showPercentage</span></span>|<span data-ttu-id="89562-137">boolean</span><span class="sxs-lookup"><span data-stu-id="89562-137">boolean</span></span>|<span data-ttu-id="89562-138">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="89562-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="89562-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="89562-139">showSeriesName</span></span>|<span data-ttu-id="89562-140">boolean</span><span class="sxs-lookup"><span data-stu-id="89562-140">boolean</span></span>|<span data-ttu-id="89562-141">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="89562-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="89562-142">showValue</span><span class="sxs-lookup"><span data-stu-id="89562-142">showValue</span></span>|<span data-ttu-id="89562-143">boolean</span><span class="sxs-lookup"><span data-stu-id="89562-143">boolean</span></span>|<span data-ttu-id="89562-144">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="89562-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89562-145">Связи</span><span class="sxs-lookup"><span data-stu-id="89562-145">Relationships</span></span>
| <span data-ttu-id="89562-146">Связь</span><span class="sxs-lookup"><span data-stu-id="89562-146">Relationship</span></span> | <span data-ttu-id="89562-147">Тип</span><span class="sxs-lookup"><span data-stu-id="89562-147">Type</span></span>   |<span data-ttu-id="89562-148">Описание</span><span class="sxs-lookup"><span data-stu-id="89562-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89562-149">format</span><span class="sxs-lookup"><span data-stu-id="89562-149">format</span></span>|[<span data-ttu-id="89562-150">воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="89562-150">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="89562-151">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов.</span><span class="sxs-lookup"><span data-stu-id="89562-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="89562-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89562-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89562-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89562-153">JSON representation</span></span>

<span data-ttu-id="89562-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89562-154">Here is a JSON representation of the resource.</span></span>

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
