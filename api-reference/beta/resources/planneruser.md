---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 70ca7596cfb809a16b76f684a85c97b0c3e43a50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521638"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="08026-103">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="08026-103">plannerUser resource type</span></span>

<span data-ttu-id="08026-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08026-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08026-105">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="08026-105">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="08026-106">Методы</span><span class="sxs-lookup"><span data-stu-id="08026-106">Methods</span></span>

| <span data-ttu-id="08026-107">Метод</span><span class="sxs-lookup"><span data-stu-id="08026-107">Method</span></span>           | <span data-ttu-id="08026-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="08026-108">Return Type</span></span>    |<span data-ttu-id="08026-109">Описание</span><span class="sxs-lookup"><span data-stu-id="08026-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="08026-110">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="08026-110">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="08026-111">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="08026-111">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="08026-112">Получение [перечисление plannertasks](plannertask.md) , назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="08026-112">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="08026-113">Список объектов favoritePlans</span><span class="sxs-lookup"><span data-stu-id="08026-113">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="08026-114">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="08026-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="08026-115">Получите [планов](plannerplan.md) , помеченный пользователем как избранный.</span><span class="sxs-lookup"><span data-stu-id="08026-115">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="08026-116">Список объектов recentPlans</span><span class="sxs-lookup"><span data-stu-id="08026-116">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="08026-117">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="08026-117">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="08026-118">Получение [планов](plannerplan.md) , недавно просмотренных пользователем.</span><span class="sxs-lookup"><span data-stu-id="08026-118">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|<span data-ttu-id="08026-119">[обновление](../api/planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="08026-119">[Update](../api/planneruser-update.md)</span></span> | [<span data-ttu-id="08026-120">plannerUser</span><span class="sxs-lookup"><span data-stu-id="08026-120">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="08026-121">Обновление объекта **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="08026-121">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="08026-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="08026-122">Properties</span></span>
| <span data-ttu-id="08026-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="08026-123">Property</span></span>     | <span data-ttu-id="08026-124">Тип</span><span class="sxs-lookup"><span data-stu-id="08026-124">Type</span></span>   |<span data-ttu-id="08026-125">Описание</span><span class="sxs-lookup"><span data-stu-id="08026-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08026-126">id</span><span class="sxs-lookup"><span data-stu-id="08026-126">id</span></span>|<span data-ttu-id="08026-127">String</span><span class="sxs-lookup"><span data-stu-id="08026-127">String</span></span>| <span data-ttu-id="08026-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08026-128">Read-only.</span></span> <span data-ttu-id="08026-129">Идентификатор объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="08026-129">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="08026-130">фаворитепланреференцес</span><span class="sxs-lookup"><span data-stu-id="08026-130">favoritePlanReferences</span></span>|<span data-ttu-id="08026-131">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="08026-131">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)</span></span>| <span data-ttu-id="08026-132">Коллекция, содержащая ссылки на планы, помеченные пользователем как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="08026-132">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="08026-133">рецентпланреференцес</span><span class="sxs-lookup"><span data-stu-id="08026-133">recentPlanReferences</span></span>|<span data-ttu-id="08026-134">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="08026-134">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)</span></span>| <span data-ttu-id="08026-135">Коллекция, содержащая ссылки на планы, которые пользователь недавно просматривал в приложениях, поддерживающих последние планы.</span><span class="sxs-lookup"><span data-stu-id="08026-135">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08026-136">Связи</span><span class="sxs-lookup"><span data-stu-id="08026-136">Relationships</span></span>
| <span data-ttu-id="08026-137">Связь</span><span class="sxs-lookup"><span data-stu-id="08026-137">Relationship</span></span> | <span data-ttu-id="08026-138">Тип</span><span class="sxs-lookup"><span data-stu-id="08026-138">Type</span></span>   |<span data-ttu-id="08026-139">Описание</span><span class="sxs-lookup"><span data-stu-id="08026-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08026-140">tasks</span><span class="sxs-lookup"><span data-stu-id="08026-140">tasks</span></span>|<span data-ttu-id="08026-141">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="08026-141">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="08026-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08026-142">Read-only.</span></span> <span data-ttu-id="08026-143">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="08026-143">Nullable.</span></span> <span data-ttu-id="08026-144">Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="08026-144">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="08026-145">фаворитепланс</span><span class="sxs-lookup"><span data-stu-id="08026-145">favoritePlans</span></span>|<span data-ttu-id="08026-146">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="08026-146">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="08026-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08026-147">Read-only.</span></span> <span data-ttu-id="08026-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="08026-148">Nullable.</span></span> <span data-ttu-id="08026-149">Возвращает [планов](plannerplan.md) , отмеченный пользователем как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="08026-149">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="08026-150">рецентпланс</span><span class="sxs-lookup"><span data-stu-id="08026-150">recentPlans</span></span>|<span data-ttu-id="08026-151">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="08026-151">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="08026-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08026-152">Read-only.</span></span> <span data-ttu-id="08026-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="08026-153">Nullable.</span></span> <span data-ttu-id="08026-154">Возвращает [планов](plannerplan.md) , которые недавно просматривал пользователь в приложениях, которые поддерживают последние планы.</span><span class="sxs-lookup"><span data-stu-id="08026-154">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08026-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08026-155">JSON representation</span></span>
<span data-ttu-id="08026-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08026-156">The following is a JSON representation of the resource.</span></span>

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
