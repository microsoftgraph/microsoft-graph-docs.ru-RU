---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 245d6cf538488c567df00129deb9b594ff22018a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811706"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="1528e-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="1528e-103">ChartPoint resource type</span></span>

<span data-ttu-id="1528e-104">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="1528e-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="1528e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1528e-105">Methods</span></span>

| <span data-ttu-id="1528e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1528e-106">Method</span></span>           | <span data-ttu-id="1528e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1528e-107">Return Type</span></span>    |<span data-ttu-id="1528e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1528e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1528e-109">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="1528e-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="1528e-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="1528e-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="1528e-111">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="1528e-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="1528e-112">List</span><span class="sxs-lookup"><span data-stu-id="1528e-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="1528e-113">[WorkbookChartPoint](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1528e-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="1528e-114">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="1528e-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="1528e-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="1528e-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="1528e-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="1528e-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="1528e-117">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="1528e-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="1528e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="1528e-118">Properties</span></span>
| <span data-ttu-id="1528e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="1528e-119">Property</span></span>     | <span data-ttu-id="1528e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1528e-120">Type</span></span>   |<span data-ttu-id="1528e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1528e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1528e-122">value</span><span class="sxs-lookup"><span data-stu-id="1528e-122">value</span></span>|<span data-ttu-id="1528e-123">Json</span><span class="sxs-lookup"><span data-stu-id="1528e-123">Json</span></span>|<span data-ttu-id="1528e-p101">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1528e-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="1528e-126">id</span><span class="sxs-lookup"><span data-stu-id="1528e-126">id</span></span>|<span data-ttu-id="1528e-127">строка</span><span class="sxs-lookup"><span data-stu-id="1528e-127">string</span></span>|<span data-ttu-id="1528e-128">Уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="1528e-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="1528e-129">Связи</span><span class="sxs-lookup"><span data-stu-id="1528e-129">Relationships</span></span>
| <span data-ttu-id="1528e-130">Связь</span><span class="sxs-lookup"><span data-stu-id="1528e-130">Relationship</span></span> | <span data-ttu-id="1528e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1528e-131">Type</span></span>   |<span data-ttu-id="1528e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1528e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1528e-133">format</span><span class="sxs-lookup"><span data-stu-id="1528e-133">format</span></span>|[<span data-ttu-id="1528e-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="1528e-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="1528e-p102">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1528e-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1528e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1528e-137">JSON representation</span></span>

<span data-ttu-id="1528e-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1528e-138">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
