---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам, планировщик работы для пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526881"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="8e83f-103">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="8e83f-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e83f-104">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщик работы для [пользователей](user.md).</span><span class="sxs-lookup"><span data-stu-id="8e83f-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="8e83f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8e83f-105">Methods</span></span>

| <span data-ttu-id="8e83f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8e83f-106">Method</span></span>           | <span data-ttu-id="8e83f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e83f-107">Return Type</span></span>    |<span data-ttu-id="8e83f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8e83f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e83f-109">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="8e83f-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="8e83f-110">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="8e83f-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="8e83f-111">Получите [plannerTasks](plannertask.md) , назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="8e83f-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="8e83f-112">Список favoritePlans</span><span class="sxs-lookup"><span data-stu-id="8e83f-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="8e83f-113">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="8e83f-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8e83f-114">Получите [plannerPlans](plannerplan.md) , помеченные как избранные пользователем.</span><span class="sxs-lookup"><span data-stu-id="8e83f-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="8e83f-115">Список recentPlans</span><span class="sxs-lookup"><span data-stu-id="8e83f-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="8e83f-116">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="8e83f-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8e83f-117">Получите [plannerPlans](plannerplan.md) недавно отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e83f-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="8e83f-118">Update</span><span class="sxs-lookup"><span data-stu-id="8e83f-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="8e83f-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="8e83f-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="8e83f-120">Обновление объекта **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="8e83f-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="8e83f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e83f-121">Properties</span></span>
| <span data-ttu-id="8e83f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e83f-122">Property</span></span>     | <span data-ttu-id="8e83f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8e83f-123">Type</span></span>   |<span data-ttu-id="8e83f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8e83f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e83f-125">id</span><span class="sxs-lookup"><span data-stu-id="8e83f-125">id</span></span>|<span data-ttu-id="8e83f-126">String</span><span class="sxs-lookup"><span data-stu-id="8e83f-126">String</span></span>| <span data-ttu-id="8e83f-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e83f-127">Read-only.</span></span> <span data-ttu-id="8e83f-128">Идентификатор plannerUser</span><span class="sxs-lookup"><span data-stu-id="8e83f-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="8e83f-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="8e83f-129">favoritePlanReferences</span></span>|<span data-ttu-id="8e83f-130">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="8e83f-130">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)</span></span>| <span data-ttu-id="8e83f-131">Коллекция, содержащая ссылки на планы, которые пользователь помеченные как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="8e83f-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="8e83f-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="8e83f-132">recentPlanReferences</span></span>|<span data-ttu-id="8e83f-133">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="8e83f-133">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)</span></span>| <span data-ttu-id="8e83f-134">Коллекция, содержащая ссылки на планы, которые были просмотрены недавно пользователя в приложениях, которые поддерживают последние планов.</span><span class="sxs-lookup"><span data-stu-id="8e83f-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e83f-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="8e83f-135">Relationships</span></span>
| <span data-ttu-id="8e83f-136">Связь</span><span class="sxs-lookup"><span data-stu-id="8e83f-136">Relationship</span></span> | <span data-ttu-id="8e83f-137">Тип</span><span class="sxs-lookup"><span data-stu-id="8e83f-137">Type</span></span>   |<span data-ttu-id="8e83f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8e83f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e83f-139">tasks</span><span class="sxs-lookup"><span data-stu-id="8e83f-139">tasks</span></span>|<span data-ttu-id="8e83f-140">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="8e83f-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="8e83f-p102">Только для чтения. Допускает значение null. Возвращает объекты [plannerTask](plannertask.md), назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="8e83f-p102">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="8e83f-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="8e83f-144">favoritePlans</span></span>|<span data-ttu-id="8e83f-145">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="8e83f-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8e83f-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e83f-146">Read-only.</span></span> <span data-ttu-id="8e83f-147">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8e83f-147">Nullable.</span></span> <span data-ttu-id="8e83f-148">Возвращает [plannerPlans](plannerplan.md) , пользователь помеченные как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="8e83f-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="8e83f-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="8e83f-149">recentPlans</span></span>|<span data-ttu-id="8e83f-150">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="8e83f-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="8e83f-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e83f-151">Read-only.</span></span> <span data-ttu-id="8e83f-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8e83f-152">Nullable.</span></span> <span data-ttu-id="8e83f-153">Возвращает [plannerPlans](plannerplan.md) , который был недавно доступен для просмотра пользователем в приложениях, которые поддерживают последние планов.</span><span class="sxs-lookup"><span data-stu-id="8e83f-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8e83f-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e83f-154">JSON representation</span></span>
<span data-ttu-id="8e83f-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e83f-155">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
