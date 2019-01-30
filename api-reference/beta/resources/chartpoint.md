---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fd50e2e0b0f289f719dd6636eab16544e6a80f5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641969"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="dea6b-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="dea6b-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dea6b-104">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="dea6b-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="dea6b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="dea6b-105">Methods</span></span>

| <span data-ttu-id="dea6b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="dea6b-106">Method</span></span>           | <span data-ttu-id="dea6b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dea6b-107">Return Type</span></span>    |<span data-ttu-id="dea6b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dea6b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dea6b-109">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="dea6b-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="dea6b-110">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="dea6b-110">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="dea6b-111">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="dea6b-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="dea6b-112">List</span><span class="sxs-lookup"><span data-stu-id="dea6b-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="dea6b-113">Коллекция объектов [ChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="dea6b-113">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="dea6b-114">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="dea6b-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="dea6b-115">Itemat</span><span class="sxs-lookup"><span data-stu-id="dea6b-115">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="dea6b-116">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="dea6b-116">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="dea6b-117">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="dea6b-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="dea6b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="dea6b-118">Properties</span></span>
| <span data-ttu-id="dea6b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="dea6b-119">Property</span></span>     | <span data-ttu-id="dea6b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="dea6b-120">Type</span></span>   |<span data-ttu-id="dea6b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dea6b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dea6b-122">value</span><span class="sxs-lookup"><span data-stu-id="dea6b-122">value</span></span>|<span data-ttu-id="dea6b-123">object</span><span class="sxs-lookup"><span data-stu-id="dea6b-123">object</span></span>|<span data-ttu-id="dea6b-p101">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dea6b-p101">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dea6b-126">Связи</span><span class="sxs-lookup"><span data-stu-id="dea6b-126">Relationships</span></span>
| <span data-ttu-id="dea6b-127">Связь</span><span class="sxs-lookup"><span data-stu-id="dea6b-127">Relationship</span></span> | <span data-ttu-id="dea6b-128">Тип</span><span class="sxs-lookup"><span data-stu-id="dea6b-128">Type</span></span>   |<span data-ttu-id="dea6b-129">Описание</span><span class="sxs-lookup"><span data-stu-id="dea6b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dea6b-130">format</span><span class="sxs-lookup"><span data-stu-id="dea6b-130">format</span></span>|[<span data-ttu-id="dea6b-131">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="dea6b-131">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="dea6b-p102">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dea6b-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dea6b-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dea6b-134">JSON representation</span></span>

<span data-ttu-id="dea6b-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dea6b-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
