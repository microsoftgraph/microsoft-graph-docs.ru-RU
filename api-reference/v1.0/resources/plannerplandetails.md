---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом plan связан объект details.
ms.openlocfilehash: eac0082c72e46101d8d02367f8c13aef5e921d17
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024976"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="d4a50-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d4a50-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="d4a50-p102">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="d4a50-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d4a50-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d4a50-107">Methods</span></span>

| <span data-ttu-id="d4a50-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d4a50-108">Method</span></span>           | <span data-ttu-id="d4a50-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4a50-109">Return Type</span></span>    |<span data-ttu-id="d4a50-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d4a50-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4a50-111">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d4a50-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="d4a50-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d4a50-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="d4a50-113">Чтение свойств и отношений объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="d4a50-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="d4a50-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="d4a50-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="d4a50-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d4a50-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="d4a50-116">Обновление объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="d4a50-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4a50-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4a50-117">Properties</span></span>
| <span data-ttu-id="d4a50-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4a50-118">Property</span></span>     | <span data-ttu-id="d4a50-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d4a50-119">Type</span></span>   |<span data-ttu-id="d4a50-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4a50-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4a50-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="d4a50-121">categoryDescriptions</span></span>|[<span data-ttu-id="d4a50-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="d4a50-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="d4a50-123">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="d4a50-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="d4a50-124">id</span><span class="sxs-lookup"><span data-stu-id="d4a50-124">id</span></span>|<span data-ttu-id="d4a50-125">String</span><span class="sxs-lookup"><span data-stu-id="d4a50-125">String</span></span>| <span data-ttu-id="d4a50-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4a50-126">Read-only.</span></span> <span data-ttu-id="d4a50-127">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="d4a50-127">ID of the plan details.</span></span> <span data-ttu-id="d4a50-128">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="d4a50-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d4a50-129">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="d4a50-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d4a50-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="d4a50-130">sharedWith</span></span>|[<span data-ttu-id="d4a50-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="d4a50-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="d4a50-p104">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="d4a50-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d4a50-135">Связи</span><span class="sxs-lookup"><span data-stu-id="d4a50-135">Relationships</span></span>
<span data-ttu-id="d4a50-136">Нет</span><span class="sxs-lookup"><span data-stu-id="d4a50-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d4a50-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4a50-137">JSON representation</span></span>
<span data-ttu-id="d4a50-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4a50-138">Here is a JSON representation of the resource.</span></span>

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