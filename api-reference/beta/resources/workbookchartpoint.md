---
title: Тип ресурса Воркбукчартпоинт
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e12cc2f9a700ef66ec47a72aa88a2c30f2c2c3f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33349003"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="a2db5-103">Тип ресурса Воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="a2db5-103">workbookChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2db5-104">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="a2db5-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="a2db5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a2db5-105">Methods</span></span>

| <span data-ttu-id="a2db5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a2db5-106">Method</span></span>           | <span data-ttu-id="a2db5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a2db5-107">Return Type</span></span>    |<span data-ttu-id="a2db5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a2db5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2db5-109">Получение Воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="a2db5-109">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="a2db5-110">Воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="a2db5-110">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="a2db5-111">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="a2db5-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="a2db5-112">Список</span><span class="sxs-lookup"><span data-stu-id="a2db5-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="a2db5-113">Коллекция [воркбукчартпоинт](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="a2db5-113">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="a2db5-114">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="a2db5-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="a2db5-115">Итемат</span><span class="sxs-lookup"><span data-stu-id="a2db5-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="a2db5-116">Воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="a2db5-116">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="a2db5-117">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="a2db5-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2db5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2db5-118">Properties</span></span>
| <span data-ttu-id="a2db5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2db5-119">Property</span></span>     | <span data-ttu-id="a2db5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a2db5-120">Type</span></span>   |<span data-ttu-id="a2db5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a2db5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2db5-122">значение</span><span class="sxs-lookup"><span data-stu-id="a2db5-122">value</span></span>|<span data-ttu-id="a2db5-123">Json</span><span class="sxs-lookup"><span data-stu-id="a2db5-123">Json</span></span>|<span data-ttu-id="a2db5-124">Возвращает значение точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a2db5-124">Returns the value of a chart point.</span></span> <span data-ttu-id="a2db5-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2db5-125">Read-only.</span></span>|
|<span data-ttu-id="a2db5-126">id</span><span class="sxs-lookup"><span data-stu-id="a2db5-126">id</span></span>|<span data-ttu-id="a2db5-127">string</span><span class="sxs-lookup"><span data-stu-id="a2db5-127">string</span></span>|<span data-ttu-id="a2db5-128">уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="a2db5-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2db5-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="a2db5-129">Relationships</span></span>
| <span data-ttu-id="a2db5-130">Отношение</span><span class="sxs-lookup"><span data-stu-id="a2db5-130">Relationship</span></span> | <span data-ttu-id="a2db5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a2db5-131">Type</span></span>   |<span data-ttu-id="a2db5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a2db5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2db5-133">format</span><span class="sxs-lookup"><span data-stu-id="a2db5-133">format</span></span>|[<span data-ttu-id="a2db5-134">Воркбукчартпоинтформат</span><span class="sxs-lookup"><span data-stu-id="a2db5-134">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="a2db5-135">Инкапсулирует свойства формата точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a2db5-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="a2db5-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2db5-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2db5-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2db5-137">JSON representation</span></span>

<span data-ttu-id="a2db5-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2db5-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
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
  "suppressions": []
}
-->
