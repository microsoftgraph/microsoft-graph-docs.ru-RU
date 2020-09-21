---
title: Тип ресурса plannerUser
description: 'Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 309f464afe33f09366f7905af7698660dd161094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063991"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="983e0-103">Тип ресурса plannerUser</span><span class="sxs-lookup"><span data-stu-id="983e0-103">plannerUser resource type</span></span>

<span data-ttu-id="983e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="983e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="983e0-105">Ресурс **plannerUser** предоставляет доступ к ресурсам планировщика для [пользователя](user.md).</span><span class="sxs-lookup"><span data-stu-id="983e0-105">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="983e0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="983e0-106">Methods</span></span>

| <span data-ttu-id="983e0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="983e0-107">Method</span></span>           | <span data-ttu-id="983e0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="983e0-108">Return Type</span></span>    |<span data-ttu-id="983e0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="983e0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="983e0-110">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="983e0-110">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="983e0-111">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="983e0-111">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="983e0-112">Получение [перечисление plannertasks](plannertask.md) , назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="983e0-112">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="983e0-113">Список объектов favoritePlans</span><span class="sxs-lookup"><span data-stu-id="983e0-113">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="983e0-114">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="983e0-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="983e0-115">Получите [планов](plannerplan.md) , помеченный пользователем как избранный.</span><span class="sxs-lookup"><span data-stu-id="983e0-115">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="983e0-116">Список объектов recentPlans</span><span class="sxs-lookup"><span data-stu-id="983e0-116">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="983e0-117">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="983e0-117">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="983e0-118">Получение [планов](plannerplan.md) , недавно просмотренных пользователем.</span><span class="sxs-lookup"><span data-stu-id="983e0-118">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="983e0-119">Обновление</span><span class="sxs-lookup"><span data-stu-id="983e0-119">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="983e0-120">plannerUser</span><span class="sxs-lookup"><span data-stu-id="983e0-120">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="983e0-121">Обновление объекта **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="983e0-121">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="983e0-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="983e0-122">Properties</span></span>
| <span data-ttu-id="983e0-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="983e0-123">Property</span></span>     | <span data-ttu-id="983e0-124">Тип</span><span class="sxs-lookup"><span data-stu-id="983e0-124">Type</span></span>   |<span data-ttu-id="983e0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="983e0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="983e0-126">id</span><span class="sxs-lookup"><span data-stu-id="983e0-126">id</span></span>|<span data-ttu-id="983e0-127">String</span><span class="sxs-lookup"><span data-stu-id="983e0-127">String</span></span>| <span data-ttu-id="983e0-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="983e0-128">Read-only.</span></span> <span data-ttu-id="983e0-129">Идентификатор объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="983e0-129">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="983e0-130">фаворитепланреференцес</span><span class="sxs-lookup"><span data-stu-id="983e0-130">favoritePlanReferences</span></span>|<span data-ttu-id="983e0-131">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md);</span><span class="sxs-lookup"><span data-stu-id="983e0-131">[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)</span></span>| <span data-ttu-id="983e0-132">Коллекция, содержащая ссылки на планы, помеченные пользователем как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="983e0-132">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="983e0-133">рецентпланреференцес</span><span class="sxs-lookup"><span data-stu-id="983e0-133">recentPlanReferences</span></span>|<span data-ttu-id="983e0-134">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md).</span><span class="sxs-lookup"><span data-stu-id="983e0-134">[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)</span></span>| <span data-ttu-id="983e0-135">Коллекция, содержащая ссылки на планы, которые пользователь недавно просматривал в приложениях, поддерживающих последние планы.</span><span class="sxs-lookup"><span data-stu-id="983e0-135">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="983e0-136">Связи</span><span class="sxs-lookup"><span data-stu-id="983e0-136">Relationships</span></span>
| <span data-ttu-id="983e0-137">Связь</span><span class="sxs-lookup"><span data-stu-id="983e0-137">Relationship</span></span> | <span data-ttu-id="983e0-138">Тип</span><span class="sxs-lookup"><span data-stu-id="983e0-138">Type</span></span>   |<span data-ttu-id="983e0-139">Описание</span><span class="sxs-lookup"><span data-stu-id="983e0-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="983e0-140">tasks</span><span class="sxs-lookup"><span data-stu-id="983e0-140">tasks</span></span>|<span data-ttu-id="983e0-141">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="983e0-141">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="983e0-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="983e0-142">Read-only.</span></span> <span data-ttu-id="983e0-143">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="983e0-143">Nullable.</span></span> <span data-ttu-id="983e0-144">Возвращает [перечисление plannertasks](plannertask.md) , назначенный пользователю.</span><span class="sxs-lookup"><span data-stu-id="983e0-144">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="983e0-145">фаворитепланс</span><span class="sxs-lookup"><span data-stu-id="983e0-145">favoritePlans</span></span>|<span data-ttu-id="983e0-146">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="983e0-146">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="983e0-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="983e0-147">Read-only.</span></span> <span data-ttu-id="983e0-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="983e0-148">Nullable.</span></span> <span data-ttu-id="983e0-149">Возвращает [планов](plannerplan.md) , отмеченный пользователем как "Избранное".</span><span class="sxs-lookup"><span data-stu-id="983e0-149">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="983e0-150">рецентпланс</span><span class="sxs-lookup"><span data-stu-id="983e0-150">recentPlans</span></span>|<span data-ttu-id="983e0-151">Коллекция объектов [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="983e0-151">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="983e0-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="983e0-152">Read-only.</span></span> <span data-ttu-id="983e0-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="983e0-153">Nullable.</span></span> <span data-ttu-id="983e0-154">Возвращает [планов](plannerplan.md) , которые недавно просматривал пользователь в приложениях, которые поддерживают последние планы.</span><span class="sxs-lookup"><span data-stu-id="983e0-154">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="983e0-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="983e0-155">JSON representation</span></span>
<span data-ttu-id="983e0-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="983e0-156">The following is a JSON representation of the resource.</span></span>

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


