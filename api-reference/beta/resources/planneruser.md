---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd279e541df4b45e47d1c389d2e8a1e212b01a41
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344344"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="3b81c-103">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="3b81c-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b81c-104">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="3b81c-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="3b81c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3b81c-105">Methods</span></span>

| <span data-ttu-id="3b81c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3b81c-106">Method</span></span>           | <span data-ttu-id="3b81c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b81c-107">Return Type</span></span>    |<span data-ttu-id="3b81c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3b81c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b81c-109">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="3b81c-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="3b81c-110">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="3b81c-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3b81c-111">Получение [перечисление plannertasks](plannertask.md) , назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="3b81c-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="3b81c-112">Список Фаворитепланс</span><span class="sxs-lookup"><span data-stu-id="3b81c-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="3b81c-113">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3b81c-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3b81c-114">Получите [планов](plannerplan.md) , помеченный пользователем как избранный.</span><span class="sxs-lookup"><span data-stu-id="3b81c-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="3b81c-115">Список Рецентпланс</span><span class="sxs-lookup"><span data-stu-id="3b81c-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="3b81c-116">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3b81c-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3b81c-117">Получение [планов](plannerplan.md) , недавно просмотренных пользователем.</span><span class="sxs-lookup"><span data-stu-id="3b81c-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="3b81c-118">Обновление</span><span class="sxs-lookup"><span data-stu-id="3b81c-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="3b81c-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="3b81c-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="3b81c-120">Обновление объекта **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="3b81c-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="3b81c-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b81c-121">Properties</span></span>
| <span data-ttu-id="3b81c-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b81c-122">Property</span></span>     | <span data-ttu-id="3b81c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3b81c-123">Type</span></span>   |<span data-ttu-id="3b81c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3b81c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b81c-125">id</span><span class="sxs-lookup"><span data-stu-id="3b81c-125">id</span></span>|<span data-ttu-id="3b81c-126">String</span><span class="sxs-lookup"><span data-stu-id="3b81c-126">String</span></span>| <span data-ttu-id="3b81c-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b81c-127">Read-only.</span></span> <span data-ttu-id="3b81c-128">Идентификатор объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="3b81c-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="3b81c-129">Фаворитепланреференцес</span><span class="sxs-lookup"><span data-stu-id="3b81c-129">favoritePlanReferences</span></span>|<span data-ttu-id="3b81c-130">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="3b81c-130">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)</span></span>| <span data-ttu-id="3b81c-131">Коллекция, содержащая ссылки на планы, помеченные пользователем как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="3b81c-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="3b81c-132">Рецентпланреференцес</span><span class="sxs-lookup"><span data-stu-id="3b81c-132">recentPlanReferences</span></span>|<span data-ttu-id="3b81c-133">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="3b81c-133">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)</span></span>| <span data-ttu-id="3b81c-134">Коллекция, содержащая ссылки на планы, которые пользователь недавно просматривал в приложениях, поддерживающих последние планы.</span><span class="sxs-lookup"><span data-stu-id="3b81c-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b81c-135">Связи</span><span class="sxs-lookup"><span data-stu-id="3b81c-135">Relationships</span></span>
| <span data-ttu-id="3b81c-136">Отношение</span><span class="sxs-lookup"><span data-stu-id="3b81c-136">Relationship</span></span> | <span data-ttu-id="3b81c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="3b81c-137">Type</span></span>   |<span data-ttu-id="3b81c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="3b81c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b81c-139">tasks</span><span class="sxs-lookup"><span data-stu-id="3b81c-139">tasks</span></span>|<span data-ttu-id="3b81c-140">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="3b81c-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3b81c-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b81c-141">Read-only.</span></span> <span data-ttu-id="3b81c-142">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="3b81c-142">Nullable.</span></span> <span data-ttu-id="3b81c-143">Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="3b81c-143">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="3b81c-144">Фаворитепланс</span><span class="sxs-lookup"><span data-stu-id="3b81c-144">favoritePlans</span></span>|<span data-ttu-id="3b81c-145">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3b81c-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3b81c-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b81c-146">Read-only.</span></span> <span data-ttu-id="3b81c-147">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="3b81c-147">Nullable.</span></span> <span data-ttu-id="3b81c-148">Возвращает [планов](plannerplan.md) , отмеченный пользователем как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="3b81c-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="3b81c-149">Рецентпланс</span><span class="sxs-lookup"><span data-stu-id="3b81c-149">recentPlans</span></span>|<span data-ttu-id="3b81c-150">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="3b81c-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3b81c-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b81c-151">Read-only.</span></span> <span data-ttu-id="3b81c-152">Допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="3b81c-152">Nullable.</span></span> <span data-ttu-id="3b81c-153">Возвращает [планов](plannerplan.md) , которые недавно просматривал пользователь в приложениях, которые поддерживают последние планы.</span><span class="sxs-lookup"><span data-stu-id="3b81c-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b81c-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b81c-154">JSON representation</span></span>
<span data-ttu-id="3b81c-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b81c-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
