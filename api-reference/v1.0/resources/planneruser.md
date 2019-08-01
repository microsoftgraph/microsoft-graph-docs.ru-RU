---
title: Тип ресурса plannerUser
description: Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. Он не содержит пригодных для использования свойств.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d995888b55282ac9db8aef9cc047f069a3cf20fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035142"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="1533b-104">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="1533b-104">plannerUser resource type</span></span>

<span data-ttu-id="1533b-105">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="1533b-105">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="1533b-106">Он не содержит пригодных для использования свойств.</span><span class="sxs-lookup"><span data-stu-id="1533b-106">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="1533b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1533b-107">Methods</span></span>

| <span data-ttu-id="1533b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1533b-108">Method</span></span>           | <span data-ttu-id="1533b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1533b-109">Return Type</span></span>    |<span data-ttu-id="1533b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1533b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1533b-111">Список планов</span><span class="sxs-lookup"><span data-stu-id="1533b-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="1533b-112">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="1533b-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1533b-113">Получение коллекции объектов **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="1533b-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="1533b-114">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="1533b-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="1533b-115">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="1533b-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1533b-116">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="1533b-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1533b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="1533b-117">Properties</span></span>
| <span data-ttu-id="1533b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="1533b-118">Property</span></span>     | <span data-ttu-id="1533b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1533b-119">Type</span></span>   |<span data-ttu-id="1533b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1533b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1533b-121">id</span><span class="sxs-lookup"><span data-stu-id="1533b-121">id</span></span>|<span data-ttu-id="1533b-122">String</span><span class="sxs-lookup"><span data-stu-id="1533b-122">String</span></span>| <span data-ttu-id="1533b-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1533b-123">Read-only.</span></span> <span data-ttu-id="1533b-124">Идентификатор объекта Планенрусер</span><span class="sxs-lookup"><span data-stu-id="1533b-124">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="1533b-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="1533b-125">Relationships</span></span>
| <span data-ttu-id="1533b-126">Отношение</span><span class="sxs-lookup"><span data-stu-id="1533b-126">Relationship</span></span> | <span data-ttu-id="1533b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1533b-127">Type</span></span>   |<span data-ttu-id="1533b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1533b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1533b-129">планирует</span><span class="sxs-lookup"><span data-stu-id="1533b-129">plans</span></span>|<span data-ttu-id="1533b-130">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="1533b-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1533b-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1533b-131">Read-only.</span></span> <span data-ttu-id="1533b-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1533b-132">Nullable.</span></span> <span data-ttu-id="1533b-133">Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="1533b-133">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="1533b-134">tasks</span><span class="sxs-lookup"><span data-stu-id="1533b-134">tasks</span></span>|<span data-ttu-id="1533b-135">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="1533b-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1533b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1533b-136">Read-only.</span></span> <span data-ttu-id="1533b-137">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1533b-137">Nullable.</span></span> <span data-ttu-id="1533b-138">Возвращает [планов](plannerplan.md) , предоставленный пользователю.</span><span class="sxs-lookup"><span data-stu-id="1533b-138">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1533b-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1533b-139">JSON representation</span></span>
<span data-ttu-id="1533b-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1533b-140">Here is a JSON representation of the resource.</span></span>

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
