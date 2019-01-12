---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3318415094a36100851b1c604cba2507de31f558
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962508"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="8bb0b-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="8bb0b-103">ChartPoint resource type</span></span>

<span data-ttu-id="8bb0b-104">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8bb0b-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8bb0b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8bb0b-105">Methods</span></span>

| <span data-ttu-id="8bb0b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8bb0b-106">Method</span></span>           | <span data-ttu-id="8bb0b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8bb0b-107">Return Type</span></span>    |<span data-ttu-id="8bb0b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb0b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8bb0b-109">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="8bb0b-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="8bb0b-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8bb0b-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="8bb0b-111">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="8bb0b-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="8bb0b-112">List</span><span class="sxs-lookup"><span data-stu-id="8bb0b-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="8bb0b-113">[WorkbookChartPoint](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8bb0b-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="8bb0b-114">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="8bb0b-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="8bb0b-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="8bb0b-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="8bb0b-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8bb0b-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="8bb0b-117">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="8bb0b-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bb0b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bb0b-118">Properties</span></span>
| <span data-ttu-id="8bb0b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bb0b-119">Property</span></span>     | <span data-ttu-id="8bb0b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb0b-120">Type</span></span>   |<span data-ttu-id="8bb0b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb0b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bb0b-122">value</span><span class="sxs-lookup"><span data-stu-id="8bb0b-122">value</span></span>|<span data-ttu-id="8bb0b-123">Json</span><span class="sxs-lookup"><span data-stu-id="8bb0b-123">Json</span></span>|<span data-ttu-id="8bb0b-p101">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8bb0b-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="8bb0b-126">id</span><span class="sxs-lookup"><span data-stu-id="8bb0b-126">id</span></span>|<span data-ttu-id="8bb0b-127">строка</span><span class="sxs-lookup"><span data-stu-id="8bb0b-127">string</span></span>|<span data-ttu-id="8bb0b-128">Уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="8bb0b-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bb0b-129">Связи</span><span class="sxs-lookup"><span data-stu-id="8bb0b-129">Relationships</span></span>
| <span data-ttu-id="8bb0b-130">Связь</span><span class="sxs-lookup"><span data-stu-id="8bb0b-130">Relationship</span></span> | <span data-ttu-id="8bb0b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb0b-131">Type</span></span>   |<span data-ttu-id="8bb0b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb0b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bb0b-133">format</span><span class="sxs-lookup"><span data-stu-id="8bb0b-133">format</span></span>|[<span data-ttu-id="8bb0b-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="8bb0b-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="8bb0b-p102">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8bb0b-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bb0b-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bb0b-137">JSON representation</span></span>

<span data-ttu-id="8bb0b-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bb0b-138">Here is a JSON representation of the resource.</span></span>

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
