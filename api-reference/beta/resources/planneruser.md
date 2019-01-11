---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам, планировщик работы для пользователя. '
localization_priority: Normal
ms.openlocfilehash: 709b259c88d8fe0f02defaa57e77727a7b967cfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820806"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="d627d-103">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="d627d-103">plannerUser resource type</span></span>

> <span data-ttu-id="d627d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d627d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d627d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d627d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d627d-106">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщик работы для [пользователей](user.md).</span><span class="sxs-lookup"><span data-stu-id="d627d-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="d627d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d627d-107">Methods</span></span>

| <span data-ttu-id="d627d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d627d-108">Method</span></span>           | <span data-ttu-id="d627d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d627d-109">Return Type</span></span>    |<span data-ttu-id="d627d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d627d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d627d-111">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="d627d-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="d627d-112">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d627d-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d627d-113">Получите [plannerTasks](plannertask.md) , назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="d627d-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="d627d-114">Список favoritePlans</span><span class="sxs-lookup"><span data-stu-id="d627d-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="d627d-115">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d627d-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d627d-116">Получите [plannerPlans](plannerplan.md) , помеченные как избранные пользователем.</span><span class="sxs-lookup"><span data-stu-id="d627d-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="d627d-117">Список recentPlans</span><span class="sxs-lookup"><span data-stu-id="d627d-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="d627d-118">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d627d-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d627d-119">Получите [plannerPlans](plannerplan.md) недавно отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d627d-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|<span data-ttu-id="d627d-120">[обновление](../api/planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="d627d-120">[Update](../api/planneruser-update.md)</span></span> | [<span data-ttu-id="d627d-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="d627d-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="d627d-122">Обновление объекта **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="d627d-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="d627d-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="d627d-123">Properties</span></span>
| <span data-ttu-id="d627d-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="d627d-124">Property</span></span>     | <span data-ttu-id="d627d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d627d-125">Type</span></span>   |<span data-ttu-id="d627d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d627d-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d627d-127">id</span><span class="sxs-lookup"><span data-stu-id="d627d-127">id</span></span>|<span data-ttu-id="d627d-128">Строка</span><span class="sxs-lookup"><span data-stu-id="d627d-128">String</span></span>| <span data-ttu-id="d627d-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d627d-129">Read-only.</span></span> <span data-ttu-id="d627d-130">Идентификатор plannerUser</span><span class="sxs-lookup"><span data-stu-id="d627d-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="d627d-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="d627d-131">favoritePlanReferences</span></span>|<span data-ttu-id="d627d-132">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="d627d-132">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)</span></span>| <span data-ttu-id="d627d-133">Коллекция, содержащая ссылки на планы, которые пользователь помеченные как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="d627d-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="d627d-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="d627d-134">recentPlanReferences</span></span>|<span data-ttu-id="d627d-135">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="d627d-135">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)</span></span>| <span data-ttu-id="d627d-136">Коллекция, содержащая ссылки на планы, которые были просмотрены недавно пользователя в приложениях, которые поддерживают последние планов.</span><span class="sxs-lookup"><span data-stu-id="d627d-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d627d-137">Связи</span><span class="sxs-lookup"><span data-stu-id="d627d-137">Relationships</span></span>
| <span data-ttu-id="d627d-138">Связь</span><span class="sxs-lookup"><span data-stu-id="d627d-138">Relationship</span></span> | <span data-ttu-id="d627d-139">Тип</span><span class="sxs-lookup"><span data-stu-id="d627d-139">Type</span></span>   |<span data-ttu-id="d627d-140">Описание</span><span class="sxs-lookup"><span data-stu-id="d627d-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d627d-141">tasks</span><span class="sxs-lookup"><span data-stu-id="d627d-141">tasks</span></span>|<span data-ttu-id="d627d-142">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d627d-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d627d-p103">Только для чтения. Допускает значение null. Возвращает объекты [plannerTask](plannertask.md), назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="d627d-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="d627d-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="d627d-146">favoritePlans</span></span>|<span data-ttu-id="d627d-147">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d627d-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d627d-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d627d-148">Read-only.</span></span> <span data-ttu-id="d627d-149">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d627d-149">Nullable.</span></span> <span data-ttu-id="d627d-150">Возвращает [plannerPlans](plannerplan.md) , пользователь помеченные как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="d627d-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="d627d-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="d627d-151">recentPlans</span></span>|<span data-ttu-id="d627d-152">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d627d-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d627d-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d627d-153">Read-only.</span></span> <span data-ttu-id="d627d-154">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d627d-154">Nullable.</span></span> <span data-ttu-id="d627d-155">Возвращает [plannerPlans](plannerplan.md) , который был недавно доступен для просмотра пользователем в приложениях, которые поддерживают последние планов.</span><span class="sxs-lookup"><span data-stu-id="d627d-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d627d-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d627d-156">JSON representation</span></span>
<span data-ttu-id="d627d-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d627d-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
