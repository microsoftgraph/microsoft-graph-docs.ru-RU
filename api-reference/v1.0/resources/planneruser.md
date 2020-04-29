---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 49b8989bd8526cbe8074a386ae31e76fd195642d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447096"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="c617a-104">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="c617a-104">plannerUser resource type</span></span>

<span data-ttu-id="c617a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c617a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c617a-106">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="c617a-106">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="c617a-107">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="c617a-107">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="c617a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c617a-108">Methods</span></span>

| <span data-ttu-id="c617a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c617a-109">Method</span></span>           | <span data-ttu-id="c617a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c617a-110">Return Type</span></span>    |<span data-ttu-id="c617a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c617a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c617a-112">Список планов</span><span class="sxs-lookup"><span data-stu-id="c617a-112">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="c617a-113">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="c617a-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c617a-114">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="c617a-114">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="c617a-115">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="c617a-115">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="c617a-116">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c617a-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c617a-117">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="c617a-117">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="c617a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c617a-118">Properties</span></span>
| <span data-ttu-id="c617a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c617a-119">Property</span></span>     | <span data-ttu-id="c617a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c617a-120">Type</span></span>   |<span data-ttu-id="c617a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c617a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c617a-122">id</span><span class="sxs-lookup"><span data-stu-id="c617a-122">id</span></span>|<span data-ttu-id="c617a-123">String</span><span class="sxs-lookup"><span data-stu-id="c617a-123">String</span></span>| <span data-ttu-id="c617a-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c617a-124">Read-only.</span></span> <span data-ttu-id="c617a-125">Идентификатор объекта Планенрусер</span><span class="sxs-lookup"><span data-stu-id="c617a-125">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="c617a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="c617a-126">Relationships</span></span>
| <span data-ttu-id="c617a-127">Связь</span><span class="sxs-lookup"><span data-stu-id="c617a-127">Relationship</span></span> | <span data-ttu-id="c617a-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c617a-128">Type</span></span>   |<span data-ttu-id="c617a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c617a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c617a-130">планирует</span><span class="sxs-lookup"><span data-stu-id="c617a-130">plans</span></span>|<span data-ttu-id="c617a-131">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="c617a-131">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c617a-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c617a-132">Read-only.</span></span> <span data-ttu-id="c617a-133">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c617a-133">Nullable.</span></span> <span data-ttu-id="c617a-134">Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="c617a-134">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="c617a-135">tasks</span><span class="sxs-lookup"><span data-stu-id="c617a-135">tasks</span></span>|<span data-ttu-id="c617a-136">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c617a-136">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c617a-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c617a-137">Read-only.</span></span> <span data-ttu-id="c617a-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c617a-138">Nullable.</span></span> <span data-ttu-id="c617a-139">Возвращает [планов](plannerplan.md) , предоставленный пользователю.</span><span class="sxs-lookup"><span data-stu-id="c617a-139">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c617a-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c617a-140">JSON representation</span></span>
<span data-ttu-id="c617a-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c617a-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
