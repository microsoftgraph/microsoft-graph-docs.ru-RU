---
title: Тип ресурса Воркбукчартпоинт
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: df7f7254251f2b424af0ffc8a6fca725285393cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993016"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="8a53f-103">Тип ресурса Воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="8a53f-103">workbookChartPoint resource type</span></span>

<span data-ttu-id="8a53f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a53f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a53f-105">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8a53f-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8a53f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8a53f-106">Methods</span></span>

| <span data-ttu-id="8a53f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8a53f-107">Method</span></span>           | <span data-ttu-id="8a53f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a53f-108">Return Type</span></span>    |<span data-ttu-id="8a53f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a53f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a53f-110">Получение Воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="8a53f-110">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="8a53f-111">воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="8a53f-111">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="8a53f-112">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="8a53f-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="8a53f-113">Список</span><span class="sxs-lookup"><span data-stu-id="8a53f-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="8a53f-114">Коллекция [воркбукчартпоинт](workbookchartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="8a53f-114">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="8a53f-115">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="8a53f-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="8a53f-116">итемат</span><span class="sxs-lookup"><span data-stu-id="8a53f-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="8a53f-117">воркбукчартпоинт</span><span class="sxs-lookup"><span data-stu-id="8a53f-117">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="8a53f-118">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="8a53f-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a53f-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a53f-119">Properties</span></span>
| <span data-ttu-id="8a53f-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a53f-120">Property</span></span>     | <span data-ttu-id="8a53f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8a53f-121">Type</span></span>   |<span data-ttu-id="8a53f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8a53f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a53f-123">значение</span><span class="sxs-lookup"><span data-stu-id="8a53f-123">value</span></span>|<span data-ttu-id="8a53f-124">Json</span><span class="sxs-lookup"><span data-stu-id="8a53f-124">Json</span></span>|<span data-ttu-id="8a53f-125">Возвращает значение точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="8a53f-125">Returns the value of a chart point.</span></span> <span data-ttu-id="8a53f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a53f-126">Read-only.</span></span>|
|<span data-ttu-id="8a53f-127">id</span><span class="sxs-lookup"><span data-stu-id="8a53f-127">id</span></span>|<span data-ttu-id="8a53f-128">string</span><span class="sxs-lookup"><span data-stu-id="8a53f-128">string</span></span>|<span data-ttu-id="8a53f-129">уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="8a53f-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a53f-130">Связи</span><span class="sxs-lookup"><span data-stu-id="8a53f-130">Relationships</span></span>
| <span data-ttu-id="8a53f-131">Связь</span><span class="sxs-lookup"><span data-stu-id="8a53f-131">Relationship</span></span> | <span data-ttu-id="8a53f-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8a53f-132">Type</span></span>   |<span data-ttu-id="8a53f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8a53f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a53f-134">format</span><span class="sxs-lookup"><span data-stu-id="8a53f-134">format</span></span>|[<span data-ttu-id="8a53f-135">воркбукчартпоинтформат</span><span class="sxs-lookup"><span data-stu-id="8a53f-135">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="8a53f-136">Инкапсулирует свойства формата точки диаграммы.</span><span class="sxs-lookup"><span data-stu-id="8a53f-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="8a53f-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a53f-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a53f-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a53f-138">JSON representation</span></span>

<span data-ttu-id="8a53f-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a53f-139">Here is a JSON representation of the resource.</span></span>

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


