---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 727da0983ddcaffb158be14a578a5a81eacecab3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037390"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="13e6e-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="13e6e-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="13e6e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13e6e-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="13e6e-106">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="13e6e-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="13e6e-107">Каждый объект [Plan](plannerplan.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="13e6e-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="13e6e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="13e6e-108">Methods</span></span>

| <span data-ttu-id="13e6e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="13e6e-109">Method</span></span>           | <span data-ttu-id="13e6e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13e6e-110">Return Type</span></span>    |<span data-ttu-id="13e6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="13e6e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="13e6e-112">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="13e6e-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | <span data-ttu-id="13e6e-113">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="13e6e-113">[plannerPlanDetails](plannerplandetails.md)</span></span> |<span data-ttu-id="13e6e-114">Чтение свойств и связей объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="13e6e-114">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|<span data-ttu-id="13e6e-115">[обновление](../api/plannerplandetails-update.md).</span><span class="sxs-lookup"><span data-stu-id="13e6e-115">[Update](../api/plannerplandetails-update.md)</span></span> | <span data-ttu-id="13e6e-116">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="13e6e-116">[plannerPlanDetails](plannerplandetails.md)</span></span>    |<span data-ttu-id="13e6e-117">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="13e6e-117">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="13e6e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="13e6e-118">Properties</span></span>
| <span data-ttu-id="13e6e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="13e6e-119">Property</span></span>     | <span data-ttu-id="13e6e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="13e6e-120">Type</span></span>   |<span data-ttu-id="13e6e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="13e6e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13e6e-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="13e6e-122">categoryDescriptions</span></span>|[<span data-ttu-id="13e6e-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="13e6e-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="13e6e-124">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="13e6e-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="13e6e-125">id</span><span class="sxs-lookup"><span data-stu-id="13e6e-125">id</span></span>|<span data-ttu-id="13e6e-126">String</span><span class="sxs-lookup"><span data-stu-id="13e6e-126">String</span></span>| <span data-ttu-id="13e6e-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13e6e-127">Read-only.</span></span> <span data-ttu-id="13e6e-128">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="13e6e-128">ID of the plan details.</span></span> <span data-ttu-id="13e6e-129">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="13e6e-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="13e6e-130">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="13e6e-130">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="13e6e-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="13e6e-131">sharedWith</span></span>|[<span data-ttu-id="13e6e-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="13e6e-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="13e6e-133">Набор идентификаторов пользователей, к которым предоставлен общий доступ к этому плану.</span><span class="sxs-lookup"><span data-stu-id="13e6e-133">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="13e6e-134">Если вы используете группы Microsoft 365, используйте API групп для управления членством в группах, чтобы поделиться планом [группы](group.md) .</span><span class="sxs-lookup"><span data-stu-id="13e6e-134">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="13e6e-135">Вы также можете добавить существующих членов группы в эту коллекцию, несмотря на то, что они не требуются для доступа к плану, принадлежащему группе.</span><span class="sxs-lookup"><span data-stu-id="13e6e-135">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="13e6e-136">Связи</span><span class="sxs-lookup"><span data-stu-id="13e6e-136">Relationships</span></span>
<span data-ttu-id="13e6e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="13e6e-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="13e6e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13e6e-138">JSON representation</span></span>
<span data-ttu-id="13e6e-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13e6e-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

