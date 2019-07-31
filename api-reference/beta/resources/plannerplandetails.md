---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 61296138f1477219e85ae7fd372102b8c7fd3a47
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965889"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="c72df-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c72df-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c72df-105">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="c72df-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="c72df-106">Каждый объект [Plan](plannerplan.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="c72df-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="c72df-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c72df-107">Methods</span></span>

| <span data-ttu-id="c72df-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c72df-108">Method</span></span>           | <span data-ttu-id="c72df-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c72df-109">Return Type</span></span>    |<span data-ttu-id="c72df-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c72df-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c72df-111">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c72df-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | <span data-ttu-id="c72df-112">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="c72df-112">[plannerPlanDetails](plannerplandetails.md)</span></span> |<span data-ttu-id="c72df-113">Чтение свойств и связей объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="c72df-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|<span data-ttu-id="c72df-114">[обновление](../api/plannerplandetails-update.md);</span><span class="sxs-lookup"><span data-stu-id="c72df-114">[Update](../api/plannerplandetails-update.md)</span></span> | <span data-ttu-id="c72df-115">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="c72df-115">[plannerPlanDetails](plannerplandetails.md)</span></span>    |<span data-ttu-id="c72df-116">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="c72df-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c72df-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c72df-117">Properties</span></span>
| <span data-ttu-id="c72df-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c72df-118">Property</span></span>     | <span data-ttu-id="c72df-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c72df-119">Type</span></span>   |<span data-ttu-id="c72df-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c72df-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c72df-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="c72df-121">categoryDescriptions</span></span>|[<span data-ttu-id="c72df-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="c72df-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="c72df-123">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="c72df-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="c72df-124">id</span><span class="sxs-lookup"><span data-stu-id="c72df-124">id</span></span>|<span data-ttu-id="c72df-125">String</span><span class="sxs-lookup"><span data-stu-id="c72df-125">String</span></span>| <span data-ttu-id="c72df-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c72df-126">Read-only.</span></span> <span data-ttu-id="c72df-127">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="c72df-127">The ID of the plan details.</span></span> <span data-ttu-id="c72df-128">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="c72df-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c72df-129">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="c72df-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c72df-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="c72df-130">sharedWith</span></span>|[<span data-ttu-id="c72df-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="c72df-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="c72df-132">Набор идентификаторов пользователей, к которым предоставлен общий доступ к этому плану.</span><span class="sxs-lookup"><span data-stu-id="c72df-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="c72df-133">Если вы используете группы Office 365, используйте API групп для управления членством в группах, чтобы поделиться планом [группы](group.md) .</span><span class="sxs-lookup"><span data-stu-id="c72df-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="c72df-134">Вы также можете добавить существующих членов группы в эту коллекцию, хотя это не требуется для доступа к плану, принадлежащему группе.</span><span class="sxs-lookup"><span data-stu-id="c72df-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="c72df-135">Контекстдетаилс</span><span class="sxs-lookup"><span data-stu-id="c72df-135">contextDetails</span></span>|<span data-ttu-id="c72df-136">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md);</span><span class="sxs-lookup"><span data-stu-id="c72df-136">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)</span></span>|<span data-ttu-id="c72df-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c72df-137">Read-only.</span></span> <span data-ttu-id="c72df-138">Коллекция дополнительных сведений, связанных с записями [планнерпланконтекст](plannerplancontext.md) , которые определены для контейнера [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="c72df-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c72df-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="c72df-139">Relationships</span></span>
<span data-ttu-id="c72df-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c72df-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c72df-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c72df-141">JSON representation</span></span>
<span data-ttu-id="c72df-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c72df-142">The following is a JSON representation of the resource.</span></span>

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
