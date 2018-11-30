---
title: Тип ресурса ChartPoint
description: Представляет точку из ряда в диаграмме.
ms.openlocfilehash: 93c89bca61f27924621df0376bdf50e925e25c86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027739"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="8c3bb-103">Тип ресурса ChartPoint</span><span class="sxs-lookup"><span data-stu-id="8c3bb-103">ChartPoint resource type</span></span>

<span data-ttu-id="8c3bb-104">Представляет точку из ряда в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="8c3bb-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8c3bb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8c3bb-105">Methods</span></span>

| <span data-ttu-id="8c3bb-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8c3bb-106">Method</span></span>           | <span data-ttu-id="8c3bb-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c3bb-107">Return Type</span></span>    |<span data-ttu-id="8c3bb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8c3bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c3bb-109">Получение объекта ChartPoint</span><span class="sxs-lookup"><span data-stu-id="8c3bb-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="8c3bb-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8c3bb-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="8c3bb-111">Чтение свойств и связей объекта chartPoint.</span><span class="sxs-lookup"><span data-stu-id="8c3bb-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="8c3bb-112">List</span><span class="sxs-lookup"><span data-stu-id="8c3bb-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="8c3bb-113">[WorkbookChartPoint](chartpoint.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8c3bb-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="8c3bb-114">Получение коллекции объектов chartPoint.</span><span class="sxs-lookup"><span data-stu-id="8c3bb-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="8c3bb-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="8c3bb-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="8c3bb-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8c3bb-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="8c3bb-117">Получение точки на основании ее положения в ряду.</span><span class="sxs-lookup"><span data-stu-id="8c3bb-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c3bb-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c3bb-118">Properties</span></span>
| <span data-ttu-id="8c3bb-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c3bb-119">Property</span></span>     | <span data-ttu-id="8c3bb-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8c3bb-120">Type</span></span>   |<span data-ttu-id="8c3bb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8c3bb-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c3bb-122">value</span><span class="sxs-lookup"><span data-stu-id="8c3bb-122">value</span></span>|<span data-ttu-id="8c3bb-123">Json</span><span class="sxs-lookup"><span data-stu-id="8c3bb-123">Json</span></span>|<span data-ttu-id="8c3bb-p101">Возвращает значение точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c3bb-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="8c3bb-126">id</span><span class="sxs-lookup"><span data-stu-id="8c3bb-126">id</span></span>|<span data-ttu-id="8c3bb-127">строка</span><span class="sxs-lookup"><span data-stu-id="8c3bb-127">string</span></span>|<span data-ttu-id="8c3bb-128">Уникальный идентификатор</span><span class="sxs-lookup"><span data-stu-id="8c3bb-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c3bb-129">Связи</span><span class="sxs-lookup"><span data-stu-id="8c3bb-129">Relationships</span></span>
| <span data-ttu-id="8c3bb-130">Связь</span><span class="sxs-lookup"><span data-stu-id="8c3bb-130">Relationship</span></span> | <span data-ttu-id="8c3bb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c3bb-131">Type</span></span>   |<span data-ttu-id="8c3bb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c3bb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c3bb-133">format</span><span class="sxs-lookup"><span data-stu-id="8c3bb-133">format</span></span>|[<span data-ttu-id="8c3bb-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="8c3bb-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="8c3bb-p102">Инкапсулирует свойства формата точки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c3bb-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c3bb-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c3bb-137">JSON representation</span></span>

<span data-ttu-id="8c3bb-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c3bb-138">Here is a JSON representation of the resource.</span></span>

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