---
title: Тип ресурса ChartDataLabels
description: Представляет коллекцию всех меток данных в точке диаграммы.
ms.openlocfilehash: d226c5edb3fecc3a2e27fae32060f786f790d7e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080019"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="eb002-103">Тип ресурса ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="eb002-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="eb002-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb002-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb002-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb002-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb002-106">Представляет коллекцию всех меток данных в точке диаграммы.</span><span class="sxs-lookup"><span data-stu-id="eb002-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="eb002-107">Методы</span><span class="sxs-lookup"><span data-stu-id="eb002-107">Methods</span></span>

| <span data-ttu-id="eb002-108">Метод</span><span class="sxs-lookup"><span data-stu-id="eb002-108">Method</span></span>           | <span data-ttu-id="eb002-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb002-109">Return Type</span></span>    |<span data-ttu-id="eb002-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb002-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb002-111">Получение объекта ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="eb002-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="eb002-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="eb002-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="eb002-113">Чтение свойств и связей объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="eb002-113">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="eb002-114">Update</span><span class="sxs-lookup"><span data-stu-id="eb002-114">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="eb002-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="eb002-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="eb002-116">Обновление объекта chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="eb002-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb002-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb002-117">Properties</span></span>
| <span data-ttu-id="eb002-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb002-118">Property</span></span>     | <span data-ttu-id="eb002-119">Тип</span><span class="sxs-lookup"><span data-stu-id="eb002-119">Type</span></span>   |<span data-ttu-id="eb002-120">Описание</span><span class="sxs-lookup"><span data-stu-id="eb002-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb002-121">position</span><span class="sxs-lookup"><span data-stu-id="eb002-121">position</span></span>|<span data-ttu-id="eb002-122">string</span><span class="sxs-lookup"><span data-stu-id="eb002-122">string</span></span>|<span data-ttu-id="eb002-p102">Значение DataLabelPosition, которое представляет положение метки данных. Возможные значения: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="eb002-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="eb002-125">разделитель</span><span class="sxs-lookup"><span data-stu-id="eb002-125">separator</span></span>|<span data-ttu-id="eb002-126">string</span><span class="sxs-lookup"><span data-stu-id="eb002-126">string</span></span>|<span data-ttu-id="eb002-127">Строка, представляющая разделитель для меток данных на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="eb002-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="eb002-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="eb002-128">showBubbleSize</span></span>|<span data-ttu-id="eb002-129">boolean</span><span class="sxs-lookup"><span data-stu-id="eb002-129">boolean</span></span>|<span data-ttu-id="eb002-130">Логическое значение, которое указывает, отображается ли размер пузырьков с метками данных.</span><span class="sxs-lookup"><span data-stu-id="eb002-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="eb002-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="eb002-131">showCategoryName</span></span>|<span data-ttu-id="eb002-132">boolean</span><span class="sxs-lookup"><span data-stu-id="eb002-132">boolean</span></span>|<span data-ttu-id="eb002-133">Логическое значение, которое указывает, отображается ли имя для категории меток данных.</span><span class="sxs-lookup"><span data-stu-id="eb002-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="eb002-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="eb002-134">showLegendKey</span></span>|<span data-ttu-id="eb002-135">boolean</span><span class="sxs-lookup"><span data-stu-id="eb002-135">boolean</span></span>|<span data-ttu-id="eb002-136">Логическое значение, которое указывает, отображаются ли условные обозначения для меток данных.</span><span class="sxs-lookup"><span data-stu-id="eb002-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="eb002-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="eb002-137">showPercentage</span></span>|<span data-ttu-id="eb002-138">boolean</span><span class="sxs-lookup"><span data-stu-id="eb002-138">boolean</span></span>|<span data-ttu-id="eb002-139">Логическое значение, которое указывает, отображается ли процентное соотношение меток данных.</span><span class="sxs-lookup"><span data-stu-id="eb002-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="eb002-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="eb002-140">showSeriesName</span></span>|<span data-ttu-id="eb002-141">boolean</span><span class="sxs-lookup"><span data-stu-id="eb002-141">boolean</span></span>|<span data-ttu-id="eb002-142">Логическое значение, которое указывает, отображается ли имя ряда для меток данных.</span><span class="sxs-lookup"><span data-stu-id="eb002-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="eb002-143">showValue</span><span class="sxs-lookup"><span data-stu-id="eb002-143">showValue</span></span>|<span data-ttu-id="eb002-144">boolean</span><span class="sxs-lookup"><span data-stu-id="eb002-144">boolean</span></span>|<span data-ttu-id="eb002-145">Логическое значение, которое указывает, отображается ли значение метки данных.</span><span class="sxs-lookup"><span data-stu-id="eb002-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb002-146">Связи</span><span class="sxs-lookup"><span data-stu-id="eb002-146">Relationships</span></span>
| <span data-ttu-id="eb002-147">Связь</span><span class="sxs-lookup"><span data-stu-id="eb002-147">Relationship</span></span> | <span data-ttu-id="eb002-148">Тип</span><span class="sxs-lookup"><span data-stu-id="eb002-148">Type</span></span>   |<span data-ttu-id="eb002-149">Описание</span><span class="sxs-lookup"><span data-stu-id="eb002-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb002-150">format</span><span class="sxs-lookup"><span data-stu-id="eb002-150">format</span></span>|[<span data-ttu-id="eb002-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="eb002-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="eb002-p103">Представляет формат меток данных диаграммы, включая форматирование заливки и шрифтов. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb002-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb002-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb002-154">JSON representation</span></span>

<span data-ttu-id="eb002-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb002-155">Here is a JSON representation of the resource.</span></span>

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