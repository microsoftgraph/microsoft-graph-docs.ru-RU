---
title: Тип ресурса ChartLegend
description: Представляет легенду в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8b05e4c130eebe3ffc23af2389feb2846ef1474e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069178"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="8cdf9-103">Тип ресурса ChartLegend</span><span class="sxs-lookup"><span data-stu-id="8cdf9-103">ChartLegend resource type</span></span>

<span data-ttu-id="8cdf9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cdf9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cdf9-105">Представляет легенду в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-105">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8cdf9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8cdf9-106">Methods</span></span>

| <span data-ttu-id="8cdf9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8cdf9-107">Method</span></span>           | <span data-ttu-id="8cdf9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8cdf9-108">Return Type</span></span>    |<span data-ttu-id="8cdf9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8cdf9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8cdf9-110">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="8cdf9-110">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="8cdf9-111">воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="8cdf9-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="8cdf9-112">Чтение свойств и связей объекта chartLegend.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-112">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="8cdf9-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="8cdf9-113">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="8cdf9-114">воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="8cdf9-114">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="8cdf9-115">Обновление объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-115">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8cdf9-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cdf9-116">Properties</span></span>
| <span data-ttu-id="8cdf9-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cdf9-117">Property</span></span>     | <span data-ttu-id="8cdf9-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8cdf9-118">Type</span></span>   |<span data-ttu-id="8cdf9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8cdf9-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cdf9-120">overlay</span><span class="sxs-lookup"><span data-stu-id="8cdf9-120">overlay</span></span>|<span data-ttu-id="8cdf9-121">boolean</span><span class="sxs-lookup"><span data-stu-id="8cdf9-121">boolean</span></span>|<span data-ttu-id="8cdf9-122">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="8cdf9-123">position</span><span class="sxs-lookup"><span data-stu-id="8cdf9-123">position</span></span>|<span data-ttu-id="8cdf9-124">string</span><span class="sxs-lookup"><span data-stu-id="8cdf9-124">string</span></span>|<span data-ttu-id="8cdf9-125">Представляет расположение легенды на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-125">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="8cdf9-126">Допустимые значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-126">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="8cdf9-127">visible</span><span class="sxs-lookup"><span data-stu-id="8cdf9-127">visible</span></span>|<span data-ttu-id="8cdf9-128">boolean</span><span class="sxs-lookup"><span data-stu-id="8cdf9-128">boolean</span></span>|<span data-ttu-id="8cdf9-129">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cdf9-130">Связи</span><span class="sxs-lookup"><span data-stu-id="8cdf9-130">Relationships</span></span>
| <span data-ttu-id="8cdf9-131">Связь</span><span class="sxs-lookup"><span data-stu-id="8cdf9-131">Relationship</span></span> | <span data-ttu-id="8cdf9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8cdf9-132">Type</span></span>   |<span data-ttu-id="8cdf9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8cdf9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cdf9-134">format</span><span class="sxs-lookup"><span data-stu-id="8cdf9-134">format</span></span>|[<span data-ttu-id="8cdf9-135">воркбукчартлежендформат</span><span class="sxs-lookup"><span data-stu-id="8cdf9-135">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="8cdf9-136">Представляет форматирование легенды диаграммы, включая заливку и шрифт.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-136">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="8cdf9-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8cdf9-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cdf9-138">JSON representation</span></span>

<span data-ttu-id="8cdf9-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cdf9-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

