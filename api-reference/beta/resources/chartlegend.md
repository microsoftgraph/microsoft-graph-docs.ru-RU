---
title: Тип ресурса ChartLegend
description: Представляет легенду в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 88330f98b2d652d347aae703ec91fd4de8678c9d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576397"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="8a331-103">Тип ресурса ChartLegend</span><span class="sxs-lookup"><span data-stu-id="8a331-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a331-104">Представляет легенду в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8a331-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8a331-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8a331-105">Methods</span></span>

| <span data-ttu-id="8a331-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8a331-106">Method</span></span>           | <span data-ttu-id="8a331-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a331-107">Return Type</span></span>    |<span data-ttu-id="8a331-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8a331-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a331-109">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="8a331-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="8a331-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="8a331-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="8a331-111">Чтение свойств и связей объекта chartLegend.</span><span class="sxs-lookup"><span data-stu-id="8a331-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="8a331-112">Update</span><span class="sxs-lookup"><span data-stu-id="8a331-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="8a331-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="8a331-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="8a331-114">Обновление объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="8a331-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a331-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a331-115">Properties</span></span>
| <span data-ttu-id="8a331-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a331-116">Property</span></span>     | <span data-ttu-id="8a331-117">Тип</span><span class="sxs-lookup"><span data-stu-id="8a331-117">Type</span></span>   |<span data-ttu-id="8a331-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8a331-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a331-119">overlay</span><span class="sxs-lookup"><span data-stu-id="8a331-119">overlay</span></span>|<span data-ttu-id="8a331-120">boolean</span><span class="sxs-lookup"><span data-stu-id="8a331-120">boolean</span></span>|<span data-ttu-id="8a331-121">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="8a331-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="8a331-122">position</span><span class="sxs-lookup"><span data-stu-id="8a331-122">position</span></span>|<span data-ttu-id="8a331-123">string</span><span class="sxs-lookup"><span data-stu-id="8a331-123">string</span></span>|<span data-ttu-id="8a331-124">Представляет положение легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="8a331-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="8a331-125">Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="8a331-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="8a331-126">visible</span><span class="sxs-lookup"><span data-stu-id="8a331-126">visible</span></span>|<span data-ttu-id="8a331-127">boolean</span><span class="sxs-lookup"><span data-stu-id="8a331-127">boolean</span></span>|<span data-ttu-id="8a331-128">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="8a331-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a331-129">Связи</span><span class="sxs-lookup"><span data-stu-id="8a331-129">Relationships</span></span>
| <span data-ttu-id="8a331-130">Связь</span><span class="sxs-lookup"><span data-stu-id="8a331-130">Relationship</span></span> | <span data-ttu-id="8a331-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8a331-131">Type</span></span>   |<span data-ttu-id="8a331-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8a331-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a331-133">format</span><span class="sxs-lookup"><span data-stu-id="8a331-133">format</span></span>|[<span data-ttu-id="8a331-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="8a331-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="8a331-p102">Представляет форматирование легенды диаграммы, включая заливку и шрифт. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a331-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a331-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a331-137">JSON representation</span></span>

<span data-ttu-id="8a331-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a331-138">Here is a JSON representation of the resource.</span></span>

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
