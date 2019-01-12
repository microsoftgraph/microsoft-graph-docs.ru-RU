---
title: Тип ресурса planner
description: Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955137"
---
# <a name="planner-resource-type"></a><span data-ttu-id="62501-105">Тип ресурса planner</span><span class="sxs-lookup"><span data-stu-id="62501-105">planner resource type</span></span>

<span data-ttu-id="62501-p102">Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="62501-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="62501-109">Методы</span><span class="sxs-lookup"><span data-stu-id="62501-109">Methods</span></span>

| <span data-ttu-id="62501-110">Метод</span><span class="sxs-lookup"><span data-stu-id="62501-110">Method</span></span>           | <span data-ttu-id="62501-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="62501-111">Return Type</span></span>    |<span data-ttu-id="62501-112">Описание</span><span class="sxs-lookup"><span data-stu-id="62501-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="62501-113">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="62501-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="62501-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="62501-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="62501-115">Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.</span><span class="sxs-lookup"><span data-stu-id="62501-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="62501-116">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="62501-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="62501-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="62501-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="62501-118">Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.</span><span class="sxs-lookup"><span data-stu-id="62501-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="62501-119">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="62501-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="62501-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="62501-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="62501-121">Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.</span><span class="sxs-lookup"><span data-stu-id="62501-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62501-122">Связи</span><span class="sxs-lookup"><span data-stu-id="62501-122">Relationships</span></span>
| <span data-ttu-id="62501-123">Связь</span><span class="sxs-lookup"><span data-stu-id="62501-123">Relationship</span></span> | <span data-ttu-id="62501-124">Тип</span><span class="sxs-lookup"><span data-stu-id="62501-124">Type</span></span>   |<span data-ttu-id="62501-125">Описание</span><span class="sxs-lookup"><span data-stu-id="62501-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62501-126">buckets</span><span class="sxs-lookup"><span data-stu-id="62501-126">buckets</span></span>|<span data-ttu-id="62501-127">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="62501-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="62501-p103">Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.</span><span class="sxs-lookup"><span data-stu-id="62501-p103">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="62501-131">plans</span><span class="sxs-lookup"><span data-stu-id="62501-131">plans</span></span>|<span data-ttu-id="62501-132">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="62501-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="62501-p104">Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.</span><span class="sxs-lookup"><span data-stu-id="62501-p104">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="62501-136">tasks</span><span class="sxs-lookup"><span data-stu-id="62501-136">tasks</span></span>|<span data-ttu-id="62501-137">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="62501-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="62501-p105">Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.</span><span class="sxs-lookup"><span data-stu-id="62501-p105">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62501-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="62501-141">JSON representation</span></span>
<span data-ttu-id="62501-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62501-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="62501-143">Пример</span><span class="sxs-lookup"><span data-stu-id="62501-143">Example</span></span>

<span data-ttu-id="62501-144">**Планировщик работы** ресурсов доступна в корне диаграммы.</span><span class="sxs-lookup"><span data-stu-id="62501-144">The **planner** resource is available at the root of the graph.</span></span>

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
