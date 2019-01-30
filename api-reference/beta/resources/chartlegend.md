---
title: Тип ресурса ChartLegend
description: Представляет легенду в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 13c054403eb93afce03775138c151e67bc2f57d7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640247"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="0a336-103">Тип ресурса ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0a336-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a336-104">Представляет легенду в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="0a336-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="0a336-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0a336-105">Methods</span></span>

| <span data-ttu-id="0a336-106">Метод</span><span class="sxs-lookup"><span data-stu-id="0a336-106">Method</span></span>           | <span data-ttu-id="0a336-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0a336-107">Return Type</span></span>    |<span data-ttu-id="0a336-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0a336-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a336-109">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0a336-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="0a336-110">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0a336-110">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="0a336-111">Чтение свойств и связей объекта chartLegend.</span><span class="sxs-lookup"><span data-stu-id="0a336-111">Read properties and relationships of chartLegend object.</span></span>|
|<span data-ttu-id="0a336-112">[обновление](../api/chartlegend-update.md).</span><span class="sxs-lookup"><span data-stu-id="0a336-112">[Update](../api/chartlegend-update.md)</span></span> | [<span data-ttu-id="0a336-113">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0a336-113">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="0a336-114">Обновление объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="0a336-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0a336-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a336-115">Properties</span></span>
| <span data-ttu-id="0a336-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a336-116">Property</span></span>     | <span data-ttu-id="0a336-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0a336-117">Type</span></span>   |<span data-ttu-id="0a336-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0a336-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a336-119">overlay</span><span class="sxs-lookup"><span data-stu-id="0a336-119">overlay</span></span>|<span data-ttu-id="0a336-120">boolean</span><span class="sxs-lookup"><span data-stu-id="0a336-120">boolean</span></span>|<span data-ttu-id="0a336-121">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="0a336-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="0a336-122">position</span><span class="sxs-lookup"><span data-stu-id="0a336-122">position</span></span>|<span data-ttu-id="0a336-123">строка</span><span class="sxs-lookup"><span data-stu-id="0a336-123">string</span></span>|<span data-ttu-id="0a336-p101">Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="0a336-p101">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="0a336-126">visible</span><span class="sxs-lookup"><span data-stu-id="0a336-126">visible</span></span>|<span data-ttu-id="0a336-127">boolean</span><span class="sxs-lookup"><span data-stu-id="0a336-127">boolean</span></span>|<span data-ttu-id="0a336-128">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="0a336-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a336-129">Связи</span><span class="sxs-lookup"><span data-stu-id="0a336-129">Relationships</span></span>
| <span data-ttu-id="0a336-130">Связь</span><span class="sxs-lookup"><span data-stu-id="0a336-130">Relationship</span></span> | <span data-ttu-id="0a336-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a336-131">Type</span></span>   |<span data-ttu-id="0a336-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a336-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a336-133">format</span><span class="sxs-lookup"><span data-stu-id="0a336-133">format</span></span>|[<span data-ttu-id="0a336-134">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="0a336-134">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="0a336-p102">Представляет форматирование легенды диаграммы, включая заливку и шрифт. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a336-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a336-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a336-137">JSON representation</span></span>

<span data-ttu-id="0a336-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a336-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlegend.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
