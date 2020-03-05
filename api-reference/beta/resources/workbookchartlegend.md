---
title: Тип ресурса Воркбукчартлеженд
description: Представляет легенду в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 60d37ab606668fbe6828293112997980c7e4580c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519311"
---
# <a name="workbookchartlegend-resource-type"></a><span data-ttu-id="3d955-103">Тип ресурса Воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="3d955-103">workbookChartLegend resource type</span></span>

<span data-ttu-id="3d955-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3d955-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d955-105">Представляет легенду в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="3d955-105">Represents the legend in a chart.</span></span>

## <a name="methods"></a><span data-ttu-id="3d955-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3d955-106">Methods</span></span>

| <span data-ttu-id="3d955-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3d955-107">Method</span></span>           | <span data-ttu-id="3d955-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3d955-108">Return Type</span></span>    |<span data-ttu-id="3d955-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3d955-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3d955-110">Получение Воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="3d955-110">Get workbookChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="3d955-111">воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="3d955-111">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="3d955-112">Чтение свойств и связей объекта chartLegend.</span><span class="sxs-lookup"><span data-stu-id="3d955-112">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="3d955-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="3d955-113">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="3d955-114">воркбукчартлеженд</span><span class="sxs-lookup"><span data-stu-id="3d955-114">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="3d955-115">Обновление объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="3d955-115">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3d955-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d955-116">Properties</span></span>
| <span data-ttu-id="3d955-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d955-117">Property</span></span>     | <span data-ttu-id="3d955-118">Тип</span><span class="sxs-lookup"><span data-stu-id="3d955-118">Type</span></span>   |<span data-ttu-id="3d955-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3d955-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d955-120">overlay</span><span class="sxs-lookup"><span data-stu-id="3d955-120">overlay</span></span>|<span data-ttu-id="3d955-121">boolean</span><span class="sxs-lookup"><span data-stu-id="3d955-121">boolean</span></span>|<span data-ttu-id="3d955-122">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3d955-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="3d955-123">position</span><span class="sxs-lookup"><span data-stu-id="3d955-123">position</span></span>|<span data-ttu-id="3d955-124">string</span><span class="sxs-lookup"><span data-stu-id="3d955-124">string</span></span>|<span data-ttu-id="3d955-125">Представляет расположение легенды на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="3d955-125">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="3d955-126">Допустимые значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="3d955-126">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="3d955-127">visible</span><span class="sxs-lookup"><span data-stu-id="3d955-127">visible</span></span>|<span data-ttu-id="3d955-128">boolean</span><span class="sxs-lookup"><span data-stu-id="3d955-128">boolean</span></span>|<span data-ttu-id="3d955-129">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="3d955-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d955-130">Связи</span><span class="sxs-lookup"><span data-stu-id="3d955-130">Relationships</span></span>
| <span data-ttu-id="3d955-131">Связь</span><span class="sxs-lookup"><span data-stu-id="3d955-131">Relationship</span></span> | <span data-ttu-id="3d955-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3d955-132">Type</span></span>   |<span data-ttu-id="3d955-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3d955-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3d955-134">format</span><span class="sxs-lookup"><span data-stu-id="3d955-134">format</span></span>|[<span data-ttu-id="3d955-135">воркбукчартлежендформат</span><span class="sxs-lookup"><span data-stu-id="3d955-135">workbookChartLegendFormat</span></span>](workbookchartlegendformat.md)|<span data-ttu-id="3d955-136">Представляет форматирование легенды диаграммы, включая заливку и шрифт.</span><span class="sxs-lookup"><span data-stu-id="3d955-136">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="3d955-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3d955-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d955-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3d955-138">JSON representation</span></span>

<span data-ttu-id="3d955-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d955-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"        
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
