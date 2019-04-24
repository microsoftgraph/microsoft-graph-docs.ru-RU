---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fd50e2e0b0f289f719dd6636eab16544e6a80f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460921"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="74f5a-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="74f5a-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74f5a-104">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="74f5a-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="74f5a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="74f5a-105">Methods</span></span>

| <span data-ttu-id="74f5a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="74f5a-106">Method</span></span>           | <span data-ttu-id="74f5a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74f5a-107">Return Type</span></span>    |<span data-ttu-id="74f5a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="74f5a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74f5a-109">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="74f5a-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="74f5a-110">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="74f5a-110">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="74f5a-111">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="74f5a-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="74f5a-112">Список</span><span class="sxs-lookup"><span data-stu-id="74f5a-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="74f5a-113">Коллекция объектов [ChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="74f5a-113">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="74f5a-114">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="74f5a-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="74f5a-115">Itemat</span><span class="sxs-lookup"><span data-stu-id="74f5a-115">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="74f5a-116">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="74f5a-116">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="74f5a-117">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="74f5a-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="74f5a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="74f5a-118">Properties</span></span>
| <span data-ttu-id="74f5a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="74f5a-119">Property</span></span>     | <span data-ttu-id="74f5a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="74f5a-120">Type</span></span>   |<span data-ttu-id="74f5a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="74f5a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74f5a-122">значение</span><span class="sxs-lookup"><span data-stu-id="74f5a-122">value</span></span>|<span data-ttu-id="74f5a-123">object</span><span class="sxs-lookup"><span data-stu-id="74f5a-123">object</span></span>|<span data-ttu-id="74f5a-p101">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74f5a-p101">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74f5a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="74f5a-126">Relationships</span></span>
| <span data-ttu-id="74f5a-127">Отношение</span><span class="sxs-lookup"><span data-stu-id="74f5a-127">Relationship</span></span> | <span data-ttu-id="74f5a-128">Тип</span><span class="sxs-lookup"><span data-stu-id="74f5a-128">Type</span></span>   |<span data-ttu-id="74f5a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="74f5a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74f5a-130">format</span><span class="sxs-lookup"><span data-stu-id="74f5a-130">format</span></span>|[<span data-ttu-id="74f5a-131">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="74f5a-131">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="74f5a-p102">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74f5a-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74f5a-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74f5a-134">JSON representation</span></span>

<span data-ttu-id="74f5a-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74f5a-135">Here is a JSON representation of the resource.</span></span>

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
