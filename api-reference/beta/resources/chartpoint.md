---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e8ede39ef53bfc39574ebfc86c8138a70fc31ad6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573069"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="05410-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="05410-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05410-104">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="05410-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="05410-105">Методы</span><span class="sxs-lookup"><span data-stu-id="05410-105">Methods</span></span>

| <span data-ttu-id="05410-106">Метод</span><span class="sxs-lookup"><span data-stu-id="05410-106">Method</span></span>           | <span data-ttu-id="05410-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05410-107">Return Type</span></span>    |<span data-ttu-id="05410-108">Описание</span><span class="sxs-lookup"><span data-stu-id="05410-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="05410-109">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="05410-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="05410-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="05410-110">workbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="05410-111">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="05410-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="05410-112">List</span><span class="sxs-lookup"><span data-stu-id="05410-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="05410-113">[workbookChartPoint](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="05410-113">[workbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="05410-114">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="05410-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="05410-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="05410-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="05410-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="05410-116">workbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="05410-117">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="05410-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="05410-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="05410-118">Properties</span></span>
| <span data-ttu-id="05410-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="05410-119">Property</span></span>     | <span data-ttu-id="05410-120">Тип</span><span class="sxs-lookup"><span data-stu-id="05410-120">Type</span></span>   |<span data-ttu-id="05410-121">Описание</span><span class="sxs-lookup"><span data-stu-id="05410-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05410-122">value</span><span class="sxs-lookup"><span data-stu-id="05410-122">value</span></span>|<span data-ttu-id="05410-123">Json</span><span class="sxs-lookup"><span data-stu-id="05410-123">Json</span></span>|<span data-ttu-id="05410-p101">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05410-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="05410-126">id</span><span class="sxs-lookup"><span data-stu-id="05410-126">id</span></span>|<span data-ttu-id="05410-127">string</span><span class="sxs-lookup"><span data-stu-id="05410-127">string</span></span>|<span data-ttu-id="05410-128">Уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="05410-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="05410-129">Связи</span><span class="sxs-lookup"><span data-stu-id="05410-129">Relationships</span></span>
| <span data-ttu-id="05410-130">Связь</span><span class="sxs-lookup"><span data-stu-id="05410-130">Relationship</span></span> | <span data-ttu-id="05410-131">Тип</span><span class="sxs-lookup"><span data-stu-id="05410-131">Type</span></span>   |<span data-ttu-id="05410-132">Описание</span><span class="sxs-lookup"><span data-stu-id="05410-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05410-133">format</span><span class="sxs-lookup"><span data-stu-id="05410-133">format</span></span>|[<span data-ttu-id="05410-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="05410-134">workbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="05410-p102">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05410-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05410-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05410-137">JSON representation</span></span>

<span data-ttu-id="05410-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05410-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
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
