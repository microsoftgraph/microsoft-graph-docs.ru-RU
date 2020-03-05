---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e06afabfa01e7c63f103208bb0f290bcb58e4c56
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447110"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="51cfa-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="51cfa-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="51cfa-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="51cfa-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="51cfa-106">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="51cfa-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="51cfa-107">Каждый объект [Plan](plannerplan.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="51cfa-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="51cfa-108">Методы</span><span class="sxs-lookup"><span data-stu-id="51cfa-108">Methods</span></span>

| <span data-ttu-id="51cfa-109">Метод</span><span class="sxs-lookup"><span data-stu-id="51cfa-109">Method</span></span>           | <span data-ttu-id="51cfa-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="51cfa-110">Return Type</span></span>    |<span data-ttu-id="51cfa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="51cfa-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51cfa-112">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="51cfa-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | <span data-ttu-id="51cfa-113">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="51cfa-113">[plannerPlanDetails](plannerplandetails.md)</span></span> |<span data-ttu-id="51cfa-114">Чтение свойств и связей объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="51cfa-114">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|<span data-ttu-id="51cfa-115">[обновление](../api/plannerplandetails-update.md).</span><span class="sxs-lookup"><span data-stu-id="51cfa-115">[Update](../api/plannerplandetails-update.md)</span></span> | <span data-ttu-id="51cfa-116">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="51cfa-116">[plannerPlanDetails](plannerplandetails.md)</span></span>    |<span data-ttu-id="51cfa-117">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="51cfa-117">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="51cfa-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="51cfa-118">Properties</span></span>
| <span data-ttu-id="51cfa-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="51cfa-119">Property</span></span>     | <span data-ttu-id="51cfa-120">Тип</span><span class="sxs-lookup"><span data-stu-id="51cfa-120">Type</span></span>   |<span data-ttu-id="51cfa-121">Описание</span><span class="sxs-lookup"><span data-stu-id="51cfa-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51cfa-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="51cfa-122">categoryDescriptions</span></span>|[<span data-ttu-id="51cfa-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="51cfa-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="51cfa-124">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="51cfa-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="51cfa-125">id</span><span class="sxs-lookup"><span data-stu-id="51cfa-125">id</span></span>|<span data-ttu-id="51cfa-126">String</span><span class="sxs-lookup"><span data-stu-id="51cfa-126">String</span></span>| <span data-ttu-id="51cfa-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51cfa-127">Read-only.</span></span> <span data-ttu-id="51cfa-128">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="51cfa-128">ID of the plan details.</span></span> <span data-ttu-id="51cfa-129">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="51cfa-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="51cfa-130">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="51cfa-130">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="51cfa-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="51cfa-131">sharedWith</span></span>|[<span data-ttu-id="51cfa-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="51cfa-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="51cfa-p104">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, используйте API Групп для предоставления доступа к плану [группы](group.md). Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="51cfa-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="51cfa-136">Связи</span><span class="sxs-lookup"><span data-stu-id="51cfa-136">Relationships</span></span>
<span data-ttu-id="51cfa-137">Нет</span><span class="sxs-lookup"><span data-stu-id="51cfa-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="51cfa-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51cfa-138">JSON representation</span></span>
<span data-ttu-id="51cfa-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51cfa-139">Here is a JSON representation of the resource.</span></span>

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
