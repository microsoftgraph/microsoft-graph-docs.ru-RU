---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. Каждый объект Plan содержит объект Details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5661477ff59036e633eb82c23e9c50d7c2c8b4a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462333"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="1f54e-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="1f54e-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="1f54e-105">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="1f54e-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="1f54e-106">Каждый объект [Plan](plannerplan.md) содержит объект Details.</span><span class="sxs-lookup"><span data-stu-id="1f54e-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="1f54e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1f54e-107">Methods</span></span>

| <span data-ttu-id="1f54e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1f54e-108">Method</span></span>           | <span data-ttu-id="1f54e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1f54e-109">Return Type</span></span>    |<span data-ttu-id="1f54e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f54e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f54e-111">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="1f54e-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | <span data-ttu-id="1f54e-112">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="1f54e-112">[plannerPlanDetails](plannerplandetails.md)</span></span> |<span data-ttu-id="1f54e-113">Чтение свойств и связей объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="1f54e-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="1f54e-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="1f54e-114">Update</span></span>](../api/plannerplandetails-update.md) | <span data-ttu-id="1f54e-115">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="1f54e-115">[plannerPlanDetails](plannerplandetails.md)</span></span>    |<span data-ttu-id="1f54e-116">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="1f54e-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f54e-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f54e-117">Properties</span></span>
| <span data-ttu-id="1f54e-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f54e-118">Property</span></span>     | <span data-ttu-id="1f54e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1f54e-119">Type</span></span>   |<span data-ttu-id="1f54e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1f54e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f54e-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="1f54e-121">categoryDescriptions</span></span>|[<span data-ttu-id="1f54e-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="1f54e-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="1f54e-123">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="1f54e-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="1f54e-124">id</span><span class="sxs-lookup"><span data-stu-id="1f54e-124">id</span></span>|<span data-ttu-id="1f54e-125">String</span><span class="sxs-lookup"><span data-stu-id="1f54e-125">String</span></span>| <span data-ttu-id="1f54e-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1f54e-126">Read-only.</span></span> <span data-ttu-id="1f54e-127">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="1f54e-127">ID of the plan details.</span></span> <span data-ttu-id="1f54e-128">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="1f54e-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1f54e-129">[Проверка формата](planner-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="1f54e-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1f54e-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="1f54e-130">sharedWith</span></span>|[<span data-ttu-id="1f54e-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="1f54e-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="1f54e-p104">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, используйте API Групп для предоставления доступа к плану [группы](group.md). Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="1f54e-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1f54e-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="1f54e-135">Relationships</span></span>
<span data-ttu-id="1f54e-136">Нет</span><span class="sxs-lookup"><span data-stu-id="1f54e-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1f54e-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f54e-137">JSON representation</span></span>
<span data-ttu-id="1f54e-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f54e-138">Here is a JSON representation of the resource.</span></span>

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
