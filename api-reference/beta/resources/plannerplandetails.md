---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 486d96f7ed9abc2347b15fcc5bd2e09a4c9a8932
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064075"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="77df6-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="77df6-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="77df6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77df6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77df6-106">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="77df6-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="77df6-107">Каждый объект [Plan](plannerplan.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="77df6-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="77df6-108">Методы</span><span class="sxs-lookup"><span data-stu-id="77df6-108">Methods</span></span>

| <span data-ttu-id="77df6-109">Метод</span><span class="sxs-lookup"><span data-stu-id="77df6-109">Method</span></span>           | <span data-ttu-id="77df6-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77df6-110">Return Type</span></span>    |<span data-ttu-id="77df6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="77df6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77df6-112">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="77df6-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | <span data-ttu-id="77df6-113">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="77df6-113">[plannerPlanDetails](plannerplandetails.md)</span></span> |<span data-ttu-id="77df6-114">Чтение свойств и связей объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="77df6-114">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="77df6-115">Обновление</span><span class="sxs-lookup"><span data-stu-id="77df6-115">Update</span></span>](../api/plannerplandetails-update.md) | <span data-ttu-id="77df6-116">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="77df6-116">[plannerPlanDetails](plannerplandetails.md)</span></span>    |<span data-ttu-id="77df6-117">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="77df6-117">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77df6-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="77df6-118">Properties</span></span>
| <span data-ttu-id="77df6-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="77df6-119">Property</span></span>     | <span data-ttu-id="77df6-120">Тип</span><span class="sxs-lookup"><span data-stu-id="77df6-120">Type</span></span>   |<span data-ttu-id="77df6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="77df6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77df6-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="77df6-122">categoryDescriptions</span></span>|[<span data-ttu-id="77df6-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="77df6-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="77df6-124">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="77df6-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="77df6-125">id</span><span class="sxs-lookup"><span data-stu-id="77df6-125">id</span></span>|<span data-ttu-id="77df6-126">String</span><span class="sxs-lookup"><span data-stu-id="77df6-126">String</span></span>| <span data-ttu-id="77df6-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77df6-127">Read-only.</span></span> <span data-ttu-id="77df6-128">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="77df6-128">The ID of the plan details.</span></span> <span data-ttu-id="77df6-129">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="77df6-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="77df6-130">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="77df6-130">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="77df6-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="77df6-131">sharedWith</span></span>|[<span data-ttu-id="77df6-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="77df6-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="77df6-133">Набор идентификаторов пользователей, к которым предоставлен общий доступ к этому плану.</span><span class="sxs-lookup"><span data-stu-id="77df6-133">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="77df6-134">Если вы используете группы Microsoft 365, используйте API групп для управления членством в группах, чтобы поделиться планом [группы](group.md) .</span><span class="sxs-lookup"><span data-stu-id="77df6-134">If you are using Microsoft 365 groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="77df6-135">Вы также можете добавить существующих членов группы в эту коллекцию, хотя это не требуется для доступа к плану, принадлежащему группе.</span><span class="sxs-lookup"><span data-stu-id="77df6-135">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="77df6-136">контекстдетаилс</span><span class="sxs-lookup"><span data-stu-id="77df6-136">contextDetails</span></span>|<span data-ttu-id="77df6-137">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md);</span><span class="sxs-lookup"><span data-stu-id="77df6-137">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)</span></span>|<span data-ttu-id="77df6-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77df6-138">Read-only.</span></span> <span data-ttu-id="77df6-139">Коллекция дополнительных сведений, связанных с записями [планнерпланконтекст](plannerplancontext.md) , которые определены для контейнера [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="77df6-139">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="77df6-140">Связи</span><span class="sxs-lookup"><span data-stu-id="77df6-140">Relationships</span></span>
<span data-ttu-id="77df6-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="77df6-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="77df6-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="77df6-142">JSON representation</span></span>
<span data-ttu-id="77df6-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77df6-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


