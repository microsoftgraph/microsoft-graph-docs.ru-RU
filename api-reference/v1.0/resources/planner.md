---
title: Тип ресурсов планировщика
description: Ресурс **планировщика** — это точка входа для объектной модели Planner. Он возвращает ресурс **планировщика singleton.**  Он не содержит никаких полезных свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8fc5f91dd8da85b259dd792a0926311d57098ee9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470678"
---
# <a name="planner-resource-type"></a><span data-ttu-id="35571-105">Тип ресурсов планировщика</span><span class="sxs-lookup"><span data-stu-id="35571-105">planner resource type</span></span>

<span data-ttu-id="35571-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35571-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35571-107">Ресурс **планировщика** — это точка входа для объектной модели Planner.</span><span class="sxs-lookup"><span data-stu-id="35571-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="35571-108">Он возвращает ресурс **планировщика singleton.**</span><span class="sxs-lookup"><span data-stu-id="35571-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="35571-109">Он не содержит никаких полезных свойств.</span><span class="sxs-lookup"><span data-stu-id="35571-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="35571-110">Методы</span><span class="sxs-lookup"><span data-stu-id="35571-110">Methods</span></span>

| <span data-ttu-id="35571-111">Метод</span><span class="sxs-lookup"><span data-stu-id="35571-111">Method</span></span>           | <span data-ttu-id="35571-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35571-112">Return Type</span></span>    |<span data-ttu-id="35571-113">Описание</span><span class="sxs-lookup"><span data-stu-id="35571-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35571-114">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="35571-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |<span data-ttu-id="35571-115">[plannerBucket](plannerbucket.md);</span><span class="sxs-lookup"><span data-stu-id="35571-115">[plannerBucket](plannerbucket.md)</span></span>| <span data-ttu-id="35571-116">Создайте новый **планировщикBucket,** разместив в коллекции ведер.</span><span class="sxs-lookup"><span data-stu-id="35571-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="35571-117">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="35571-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="35571-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="35571-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="35571-119">Создайте новый **планировщикPlan,** разместив в коллекции планов.</span><span class="sxs-lookup"><span data-stu-id="35571-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="35571-120">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="35571-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |<span data-ttu-id="35571-121">[plannerTask](plannertask.md);</span><span class="sxs-lookup"><span data-stu-id="35571-121">[plannerTask](plannertask.md)</span></span>| <span data-ttu-id="35571-122">Создайте новый **планировщикTask,** разместив в коллекции задач.</span><span class="sxs-lookup"><span data-stu-id="35571-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35571-123">Связи</span><span class="sxs-lookup"><span data-stu-id="35571-123">Relationships</span></span>
| <span data-ttu-id="35571-124">Связь</span><span class="sxs-lookup"><span data-stu-id="35571-124">Relationship</span></span> | <span data-ttu-id="35571-125">Тип</span><span class="sxs-lookup"><span data-stu-id="35571-125">Type</span></span>   |<span data-ttu-id="35571-126">Описание</span><span class="sxs-lookup"><span data-stu-id="35571-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35571-127">buckets</span><span class="sxs-lookup"><span data-stu-id="35571-127">buckets</span></span>|<span data-ttu-id="35571-128">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="35571-128">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="35571-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35571-129">Read-only.</span></span> <span data-ttu-id="35571-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="35571-130">Nullable.</span></span> <span data-ttu-id="35571-131">Возвращает коллекцию указанных ведер</span><span class="sxs-lookup"><span data-stu-id="35571-131">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="35571-132">планы</span><span class="sxs-lookup"><span data-stu-id="35571-132">plans</span></span>|<span data-ttu-id="35571-133">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="35571-133">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="35571-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35571-134">Read-only.</span></span> <span data-ttu-id="35571-135">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="35571-135">Nullable.</span></span> <span data-ttu-id="35571-136">Возвращает коллекцию указанных планов</span><span class="sxs-lookup"><span data-stu-id="35571-136">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="35571-137">tasks</span><span class="sxs-lookup"><span data-stu-id="35571-137">tasks</span></span>|<span data-ttu-id="35571-138">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="35571-138">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="35571-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35571-139">Read-only.</span></span> <span data-ttu-id="35571-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="35571-140">Nullable.</span></span> <span data-ttu-id="35571-141">Возвращает коллекцию указанных задач</span><span class="sxs-lookup"><span data-stu-id="35571-141">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35571-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35571-142">JSON representation</span></span>
<span data-ttu-id="35571-143">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35571-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="35571-144">Пример</span><span class="sxs-lookup"><span data-stu-id="35571-144">Example</span></span>

<span data-ttu-id="35571-145">Ресурс **планировщика** доступен в корне графа.</span><span class="sxs-lookup"><span data-stu-id="35571-145">The **planner** resource is available at the root of the graph.</span></span>

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
```http
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

