---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8333596ee93a42db8eded49815059e8633bf3db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037635"
---
# <a name="planner-resource-type"></a><span data-ttu-id="d5796-105">Тип ресурса планировщика</span><span class="sxs-lookup"><span data-stu-id="d5796-105">planner resource type</span></span>

<span data-ttu-id="d5796-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5796-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5796-107">Ресурс **планировщика** — точка входа для объектной модели планировщика.</span><span class="sxs-lookup"><span data-stu-id="d5796-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="d5796-108">Он возвращает одноэлементный ресурс **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="d5796-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="d5796-109">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="d5796-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d5796-110">Методы</span><span class="sxs-lookup"><span data-stu-id="d5796-110">Methods</span></span>

| <span data-ttu-id="d5796-111">Метод</span><span class="sxs-lookup"><span data-stu-id="d5796-111">Method</span></span>           | <span data-ttu-id="d5796-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d5796-112">Return Type</span></span>    |<span data-ttu-id="d5796-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d5796-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d5796-114">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d5796-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="d5796-115">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="d5796-115">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="d5796-116">Создание нового **plannerBucket** путем публикации в коллекции "сегменты".</span><span class="sxs-lookup"><span data-stu-id="d5796-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="d5796-117">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d5796-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="d5796-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d5796-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="d5796-119">Создание нового **plannerPlan** путем публикации в коллекции plans.</span><span class="sxs-lookup"><span data-stu-id="d5796-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="d5796-120">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="d5796-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |<span data-ttu-id="d5796-121">[plannerTask](plannertask.md);</span><span class="sxs-lookup"><span data-stu-id="d5796-121">[plannerTask](plannertask.md)</span></span>| <span data-ttu-id="d5796-122">Создание нового **plannerTask** путем публикации в коллекции Tasks.</span><span class="sxs-lookup"><span data-stu-id="d5796-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5796-123">Связи</span><span class="sxs-lookup"><span data-stu-id="d5796-123">Relationships</span></span>
| <span data-ttu-id="d5796-124">Связь</span><span class="sxs-lookup"><span data-stu-id="d5796-124">Relationship</span></span> | <span data-ttu-id="d5796-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d5796-125">Type</span></span>   |<span data-ttu-id="d5796-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d5796-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5796-127">buckets</span><span class="sxs-lookup"><span data-stu-id="d5796-127">buckets</span></span>|<span data-ttu-id="d5796-128">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d5796-128">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d5796-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5796-129">Read-only.</span></span> <span data-ttu-id="d5796-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d5796-130">Nullable.</span></span> <span data-ttu-id="d5796-131">Возвращает коллекцию указанных сегментов</span><span class="sxs-lookup"><span data-stu-id="d5796-131">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="d5796-132">планирует</span><span class="sxs-lookup"><span data-stu-id="d5796-132">plans</span></span>|<span data-ttu-id="d5796-133">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d5796-133">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d5796-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5796-134">Read-only.</span></span> <span data-ttu-id="d5796-135">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d5796-135">Nullable.</span></span> <span data-ttu-id="d5796-136">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="d5796-136">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="d5796-137">tasks</span><span class="sxs-lookup"><span data-stu-id="d5796-137">tasks</span></span>|<span data-ttu-id="d5796-138">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d5796-138">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d5796-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d5796-139">Read-only.</span></span> <span data-ttu-id="d5796-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d5796-140">Nullable.</span></span> <span data-ttu-id="d5796-141">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="d5796-141">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5796-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5796-142">JSON representation</span></span>
<span data-ttu-id="d5796-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5796-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="d5796-144">Пример</span><span class="sxs-lookup"><span data-stu-id="d5796-144">Example</span></span>

<span data-ttu-id="d5796-145">Ресурс **планировщика** доступен в корневом каталоге диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d5796-145">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

