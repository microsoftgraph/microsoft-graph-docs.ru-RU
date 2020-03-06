---
title: Тип ресурса планировщика
description: Ресурс **планировщика** — точка входа для объектной модели планировщика. Он возвращает одноэлементный ресурс **планировщика** .  Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a7387b95e933378cb089834a1af29e0c7ca45266
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534037"
---
# <a name="planner-resource-type"></a><span data-ttu-id="9cabe-105">Тип ресурса планировщика</span><span class="sxs-lookup"><span data-stu-id="9cabe-105">planner resource type</span></span>

<span data-ttu-id="9cabe-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cabe-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cabe-107">Ресурс **планировщика** — точка входа для объектной модели планировщика.</span><span class="sxs-lookup"><span data-stu-id="9cabe-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="9cabe-108">Он возвращает одноэлементный ресурс **планировщика** .</span><span class="sxs-lookup"><span data-stu-id="9cabe-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="9cabe-109">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="9cabe-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="9cabe-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9cabe-110">Methods</span></span>

| <span data-ttu-id="9cabe-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9cabe-111">Method</span></span>           | <span data-ttu-id="9cabe-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9cabe-112">Return Type</span></span>    |<span data-ttu-id="9cabe-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9cabe-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9cabe-114">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="9cabe-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="9cabe-115">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="9cabe-115">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="9cabe-116">Создание нового **plannerBucket** путем публикации в коллекции "сегменты".</span><span class="sxs-lookup"><span data-stu-id="9cabe-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="9cabe-117">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9cabe-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="9cabe-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9cabe-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="9cabe-119">Создание нового **plannerPlan** путем публикации в коллекции plans.</span><span class="sxs-lookup"><span data-stu-id="9cabe-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="9cabe-120">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="9cabe-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="9cabe-121">plannerTask</span><span class="sxs-lookup"><span data-stu-id="9cabe-121">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="9cabe-122">Создание нового **plannerTask** путем публикации в коллекции Tasks.</span><span class="sxs-lookup"><span data-stu-id="9cabe-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cabe-123">Связи</span><span class="sxs-lookup"><span data-stu-id="9cabe-123">Relationships</span></span>
| <span data-ttu-id="9cabe-124">Связь</span><span class="sxs-lookup"><span data-stu-id="9cabe-124">Relationship</span></span> | <span data-ttu-id="9cabe-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9cabe-125">Type</span></span>   |<span data-ttu-id="9cabe-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9cabe-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cabe-127">buckets</span><span class="sxs-lookup"><span data-stu-id="9cabe-127">buckets</span></span>|<span data-ttu-id="9cabe-128">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="9cabe-128">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="9cabe-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cabe-129">Read-only.</span></span> <span data-ttu-id="9cabe-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9cabe-130">Nullable.</span></span> <span data-ttu-id="9cabe-131">Возвращает коллекцию указанных сегментов</span><span class="sxs-lookup"><span data-stu-id="9cabe-131">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="9cabe-132">планирует</span><span class="sxs-lookup"><span data-stu-id="9cabe-132">plans</span></span>|<span data-ttu-id="9cabe-133">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="9cabe-133">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="9cabe-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cabe-134">Read-only.</span></span> <span data-ttu-id="9cabe-135">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9cabe-135">Nullable.</span></span> <span data-ttu-id="9cabe-136">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="9cabe-136">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="9cabe-137">tasks</span><span class="sxs-lookup"><span data-stu-id="9cabe-137">tasks</span></span>|<span data-ttu-id="9cabe-138">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9cabe-138">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9cabe-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9cabe-139">Read-only.</span></span> <span data-ttu-id="9cabe-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9cabe-140">Nullable.</span></span> <span data-ttu-id="9cabe-141">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="9cabe-141">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cabe-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cabe-142">JSON representation</span></span>
<span data-ttu-id="9cabe-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cabe-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="9cabe-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9cabe-144">Example</span></span>

<span data-ttu-id="9cabe-145">Ресурс **планировщика** доступен в корневом каталоге диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9cabe-145">The **planner** resource is available at the root of the graph.</span></span>

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
