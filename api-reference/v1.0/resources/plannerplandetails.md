---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом plan связан объект details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5661477ff59036e633eb82c23e9c50d7c2c8b4a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934676"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="70216-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="70216-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="70216-p102">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="70216-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="70216-107">Методы</span><span class="sxs-lookup"><span data-stu-id="70216-107">Methods</span></span>

| <span data-ttu-id="70216-108">Метод</span><span class="sxs-lookup"><span data-stu-id="70216-108">Method</span></span>           | <span data-ttu-id="70216-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70216-109">Return Type</span></span>    |<span data-ttu-id="70216-110">Описание</span><span class="sxs-lookup"><span data-stu-id="70216-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70216-111">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="70216-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="70216-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="70216-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="70216-113">Чтение свойств и отношений объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="70216-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="70216-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="70216-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="70216-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="70216-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="70216-116">Обновление объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="70216-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="70216-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="70216-117">Properties</span></span>
| <span data-ttu-id="70216-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="70216-118">Property</span></span>     | <span data-ttu-id="70216-119">Тип</span><span class="sxs-lookup"><span data-stu-id="70216-119">Type</span></span>   |<span data-ttu-id="70216-120">Описание</span><span class="sxs-lookup"><span data-stu-id="70216-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70216-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="70216-121">categoryDescriptions</span></span>|[<span data-ttu-id="70216-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="70216-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="70216-123">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="70216-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="70216-124">id</span><span class="sxs-lookup"><span data-stu-id="70216-124">id</span></span>|<span data-ttu-id="70216-125">Строка</span><span class="sxs-lookup"><span data-stu-id="70216-125">String</span></span>| <span data-ttu-id="70216-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70216-126">Read-only.</span></span> <span data-ttu-id="70216-127">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="70216-127">ID of the plan details.</span></span> <span data-ttu-id="70216-128">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="70216-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="70216-129">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="70216-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="70216-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="70216-130">sharedWith</span></span>|[<span data-ttu-id="70216-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="70216-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="70216-p104">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="70216-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="70216-135">Связи</span><span class="sxs-lookup"><span data-stu-id="70216-135">Relationships</span></span>
<span data-ttu-id="70216-136">Нет</span><span class="sxs-lookup"><span data-stu-id="70216-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="70216-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70216-137">JSON representation</span></span>
<span data-ttu-id="70216-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70216-138">Here is a JSON representation of the resource.</span></span>

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
