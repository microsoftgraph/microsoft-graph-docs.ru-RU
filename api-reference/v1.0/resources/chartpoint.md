---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 208f4eb90763210639540c9fd15bdaec89b7466c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988382"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="6f113-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="6f113-103">ChartPoint resource type</span></span>

<span data-ttu-id="6f113-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f113-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f113-105">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="6f113-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="6f113-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6f113-106">Methods</span></span>

| <span data-ttu-id="6f113-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6f113-107">Method</span></span>           | <span data-ttu-id="6f113-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6f113-108">Return Type</span></span>    |<span data-ttu-id="6f113-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6f113-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6f113-110">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="6f113-110">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="6f113-111">воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="6f113-111">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="6f113-112">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="6f113-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="6f113-113">Список</span><span class="sxs-lookup"><span data-stu-id="6f113-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="6f113-114">Коллекция [воркбукчартпоинт](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="6f113-114">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="6f113-115">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="6f113-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="6f113-116">итемат</span><span class="sxs-lookup"><span data-stu-id="6f113-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="6f113-117">воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="6f113-117">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="6f113-118">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="6f113-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="6f113-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f113-119">Properties</span></span>
| <span data-ttu-id="6f113-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f113-120">Property</span></span>     | <span data-ttu-id="6f113-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6f113-121">Type</span></span>   |<span data-ttu-id="6f113-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6f113-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f113-123">значение</span><span class="sxs-lookup"><span data-stu-id="6f113-123">value</span></span>|<span data-ttu-id="6f113-124">Json</span><span class="sxs-lookup"><span data-stu-id="6f113-124">Json</span></span>|<span data-ttu-id="6f113-125">Возвращает значение точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6f113-125">Returns the value of a chart point.</span></span> <span data-ttu-id="6f113-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f113-126">Read-only.</span></span>|
|<span data-ttu-id="6f113-127">id</span><span class="sxs-lookup"><span data-stu-id="6f113-127">id</span></span>|<span data-ttu-id="6f113-128">string</span><span class="sxs-lookup"><span data-stu-id="6f113-128">string</span></span>|<span data-ttu-id="6f113-129">уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="6f113-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f113-130">Связи</span><span class="sxs-lookup"><span data-stu-id="6f113-130">Relationships</span></span>
| <span data-ttu-id="6f113-131">Связь</span><span class="sxs-lookup"><span data-stu-id="6f113-131">Relationship</span></span> | <span data-ttu-id="6f113-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6f113-132">Type</span></span>   |<span data-ttu-id="6f113-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6f113-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f113-134">format</span><span class="sxs-lookup"><span data-stu-id="6f113-134">format</span></span>|[<span data-ttu-id="6f113-135">воркбукчартпоинтформат</span><span class="sxs-lookup"><span data-stu-id="6f113-135">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="6f113-136">Инкапсулирует свойства формата точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6f113-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="6f113-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f113-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f113-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f113-138">JSON representation</span></span>

<span data-ttu-id="6f113-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f113-139">Here is a JSON representation of the resource.</span></span>

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

