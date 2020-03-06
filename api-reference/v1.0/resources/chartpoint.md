---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: befa6f552fd343140d2aae10266c1445066266d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531833"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="e1f6d-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="e1f6d-103">ChartPoint resource type</span></span>

<span data-ttu-id="e1f6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1f6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1f6d-105">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="e1f6d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e1f6d-106">Methods</span></span>

| <span data-ttu-id="e1f6d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e1f6d-107">Method</span></span>           | <span data-ttu-id="e1f6d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e1f6d-108">Return Type</span></span>    |<span data-ttu-id="e1f6d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e1f6d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1f6d-110">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="e1f6d-110">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="e1f6d-111">воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="e1f6d-111">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="e1f6d-112">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="e1f6d-113">Список</span><span class="sxs-lookup"><span data-stu-id="e1f6d-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="e1f6d-114">Коллекция [воркбукчартпоинт](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="e1f6d-114">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="e1f6d-115">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="e1f6d-116">итемат</span><span class="sxs-lookup"><span data-stu-id="e1f6d-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="e1f6d-117">воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="e1f6d-117">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="e1f6d-118">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1f6d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1f6d-119">Properties</span></span>
| <span data-ttu-id="e1f6d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1f6d-120">Property</span></span>     | <span data-ttu-id="e1f6d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e1f6d-121">Type</span></span>   |<span data-ttu-id="e1f6d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e1f6d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1f6d-123">значение</span><span class="sxs-lookup"><span data-stu-id="e1f6d-123">value</span></span>|<span data-ttu-id="e1f6d-124">Json</span><span class="sxs-lookup"><span data-stu-id="e1f6d-124">Json</span></span>|<span data-ttu-id="e1f6d-125">Возвращает значение точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-125">Returns the value of a chart point.</span></span> <span data-ttu-id="e1f6d-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-126">Read-only.</span></span>|
|<span data-ttu-id="e1f6d-127">id</span><span class="sxs-lookup"><span data-stu-id="e1f6d-127">id</span></span>|<span data-ttu-id="e1f6d-128">string</span><span class="sxs-lookup"><span data-stu-id="e1f6d-128">string</span></span>|<span data-ttu-id="e1f6d-129">уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="e1f6d-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1f6d-130">Связи</span><span class="sxs-lookup"><span data-stu-id="e1f6d-130">Relationships</span></span>
| <span data-ttu-id="e1f6d-131">Связь</span><span class="sxs-lookup"><span data-stu-id="e1f6d-131">Relationship</span></span> | <span data-ttu-id="e1f6d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e1f6d-132">Type</span></span>   |<span data-ttu-id="e1f6d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e1f6d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1f6d-134">format</span><span class="sxs-lookup"><span data-stu-id="e1f6d-134">format</span></span>|[<span data-ttu-id="e1f6d-135">воркбукчартпоинтформат</span><span class="sxs-lookup"><span data-stu-id="e1f6d-135">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="e1f6d-136">Инкапсулирует свойства формата точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="e1f6d-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1f6d-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1f6d-138">JSON representation</span></span>

<span data-ttu-id="e1f6d-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1f6d-139">Here is a JSON representation of the resource.</span></span>

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
