---
title: Тип ресурса planner
description: Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523402"
---
# <a name="planner-resource-type"></a><span data-ttu-id="2d82d-105">Тип ресурса planner</span><span class="sxs-lookup"><span data-stu-id="2d82d-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d82d-p102">Ресурс **planner** — это точка входа для объектной модели Планировщика. Он возвращает одноэлементный ресурс **planner**.  Он не содержит свойства, которые можно использовать.</span><span class="sxs-lookup"><span data-stu-id="2d82d-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="2d82d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="2d82d-109">Methods</span></span>

| <span data-ttu-id="2d82d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="2d82d-110">Method</span></span>           | <span data-ttu-id="2d82d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2d82d-111">Return Type</span></span>    |<span data-ttu-id="2d82d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2d82d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d82d-113">Создание объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="2d82d-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="2d82d-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="2d82d-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="2d82d-115">Создайте объект **plannerBucket**, отправив запрос POST в коллекцию buckets.</span><span class="sxs-lookup"><span data-stu-id="2d82d-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="2d82d-116">Создание объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2d82d-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="2d82d-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2d82d-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="2d82d-118">Создайте объект **plannerPlan**, отправив запрос POST в коллекцию plans.</span><span class="sxs-lookup"><span data-stu-id="2d82d-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="2d82d-119">Создание объекта plannerTask</span><span class="sxs-lookup"><span data-stu-id="2d82d-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="2d82d-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="2d82d-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="2d82d-121">Создайте объект **plannerTask**, отправив запрос POST в коллекцию tasks.</span><span class="sxs-lookup"><span data-stu-id="2d82d-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d82d-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d82d-122">Properties</span></span>
| <span data-ttu-id="2d82d-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d82d-123">Property</span></span>     | <span data-ttu-id="2d82d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="2d82d-124">Type</span></span>   |<span data-ttu-id="2d82d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2d82d-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d82d-126">id</span><span class="sxs-lookup"><span data-stu-id="2d82d-126">id</span></span>|<span data-ttu-id="2d82d-127">String</span><span class="sxs-lookup"><span data-stu-id="2d82d-127">String</span></span>| <span data-ttu-id="2d82d-p103">Только для чтения. Идентификатор ресурса **planner**.</span><span class="sxs-lookup"><span data-stu-id="2d82d-p103">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d82d-130">Связи</span><span class="sxs-lookup"><span data-stu-id="2d82d-130">Relationships</span></span>
| <span data-ttu-id="2d82d-131">Связь</span><span class="sxs-lookup"><span data-stu-id="2d82d-131">Relationship</span></span> | <span data-ttu-id="2d82d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2d82d-132">Type</span></span>   |<span data-ttu-id="2d82d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2d82d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d82d-134">buckets</span><span class="sxs-lookup"><span data-stu-id="2d82d-134">buckets</span></span>|<span data-ttu-id="2d82d-135">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="2d82d-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="2d82d-p104">Только для чтения. Допускает значение null. Возвращает коллекцию указанных сегментов.</span><span class="sxs-lookup"><span data-stu-id="2d82d-p104">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="2d82d-139">plans</span><span class="sxs-lookup"><span data-stu-id="2d82d-139">plans</span></span>|<span data-ttu-id="2d82d-140">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="2d82d-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="2d82d-p105">Только для чтения. Допускает значение null. Возвращает коллекцию указанных планов.</span><span class="sxs-lookup"><span data-stu-id="2d82d-p105">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="2d82d-144">tasks</span><span class="sxs-lookup"><span data-stu-id="2d82d-144">tasks</span></span>|<span data-ttu-id="2d82d-145">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="2d82d-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2d82d-p106">Только для чтения. Допускает значение null. Возвращает коллекцию указанных задач.</span><span class="sxs-lookup"><span data-stu-id="2d82d-p106">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2d82d-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2d82d-149">JSON representation</span></span>
<span data-ttu-id="2d82d-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d82d-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planner.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
