---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4ec087de509d66f48c8921252cb1b058e6581741
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521680"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="01ca1-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="01ca1-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="01ca1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01ca1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01ca1-106">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="01ca1-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="01ca1-107">Каждый объект [Plan](plannerplan.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="01ca1-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="01ca1-108">Методы</span><span class="sxs-lookup"><span data-stu-id="01ca1-108">Methods</span></span>

| <span data-ttu-id="01ca1-109">Метод</span><span class="sxs-lookup"><span data-stu-id="01ca1-109">Method</span></span>           | <span data-ttu-id="01ca1-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01ca1-110">Return Type</span></span>    |<span data-ttu-id="01ca1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01ca1-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01ca1-112">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="01ca1-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | <span data-ttu-id="01ca1-113">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="01ca1-113">[plannerPlanDetails](plannerplandetails.md)</span></span> |<span data-ttu-id="01ca1-114">Чтение свойств и связей объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="01ca1-114">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|<span data-ttu-id="01ca1-115">[обновление](../api/plannerplandetails-update.md).</span><span class="sxs-lookup"><span data-stu-id="01ca1-115">[Update](../api/plannerplandetails-update.md)</span></span> | <span data-ttu-id="01ca1-116">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="01ca1-116">[plannerPlanDetails](plannerplandetails.md)</span></span>    |<span data-ttu-id="01ca1-117">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="01ca1-117">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="01ca1-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="01ca1-118">Properties</span></span>
| <span data-ttu-id="01ca1-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="01ca1-119">Property</span></span>     | <span data-ttu-id="01ca1-120">Тип</span><span class="sxs-lookup"><span data-stu-id="01ca1-120">Type</span></span>   |<span data-ttu-id="01ca1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="01ca1-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01ca1-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="01ca1-122">categoryDescriptions</span></span>|[<span data-ttu-id="01ca1-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="01ca1-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="01ca1-124">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="01ca1-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="01ca1-125">id</span><span class="sxs-lookup"><span data-stu-id="01ca1-125">id</span></span>|<span data-ttu-id="01ca1-126">String</span><span class="sxs-lookup"><span data-stu-id="01ca1-126">String</span></span>| <span data-ttu-id="01ca1-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01ca1-127">Read-only.</span></span> <span data-ttu-id="01ca1-128">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="01ca1-128">The ID of the plan details.</span></span> <span data-ttu-id="01ca1-129">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="01ca1-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="01ca1-130">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="01ca1-130">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="01ca1-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="01ca1-131">sharedWith</span></span>|[<span data-ttu-id="01ca1-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="01ca1-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="01ca1-133">Набор идентификаторов пользователей, к которым предоставлен общий доступ к этому плану.</span><span class="sxs-lookup"><span data-stu-id="01ca1-133">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="01ca1-134">Если вы используете группы Office 365, используйте API групп для управления членством в группах, чтобы поделиться планом [группы](group.md) .</span><span class="sxs-lookup"><span data-stu-id="01ca1-134">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="01ca1-135">Вы также можете добавить существующих членов группы в эту коллекцию, хотя это не требуется для доступа к плану, принадлежащему группе.</span><span class="sxs-lookup"><span data-stu-id="01ca1-135">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="01ca1-136">контекстдетаилс</span><span class="sxs-lookup"><span data-stu-id="01ca1-136">contextDetails</span></span>|<span data-ttu-id="01ca1-137">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md);</span><span class="sxs-lookup"><span data-stu-id="01ca1-137">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)</span></span>|<span data-ttu-id="01ca1-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01ca1-138">Read-only.</span></span> <span data-ttu-id="01ca1-139">Коллекция дополнительных сведений, связанных с записями [планнерпланконтекст](plannerplancontext.md) , которые определены для контейнера [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="01ca1-139">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="01ca1-140">Связи</span><span class="sxs-lookup"><span data-stu-id="01ca1-140">Relationships</span></span>
<span data-ttu-id="01ca1-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="01ca1-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="01ca1-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="01ca1-142">JSON representation</span></span>
<span data-ttu-id="01ca1-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01ca1-143">The following is a JSON representation of the resource.</span></span>

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
