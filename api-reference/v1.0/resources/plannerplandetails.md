---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом plan связан объект details.
localization_priority: Normal
ms.openlocfilehash: 59064093b485b6c82bd5b2e0b59ca1868e8517e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867741"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="dd883-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="dd883-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="dd883-p102">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="dd883-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="dd883-107">Методы</span><span class="sxs-lookup"><span data-stu-id="dd883-107">Methods</span></span>

| <span data-ttu-id="dd883-108">Метод</span><span class="sxs-lookup"><span data-stu-id="dd883-108">Method</span></span>           | <span data-ttu-id="dd883-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd883-109">Return Type</span></span>    |<span data-ttu-id="dd883-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dd883-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd883-111">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="dd883-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="dd883-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="dd883-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="dd883-113">Чтение свойств и отношений объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="dd883-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="dd883-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="dd883-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="dd883-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="dd883-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="dd883-116">Обновление объекта **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="dd883-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd883-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd883-117">Properties</span></span>
| <span data-ttu-id="dd883-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd883-118">Property</span></span>     | <span data-ttu-id="dd883-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dd883-119">Type</span></span>   |<span data-ttu-id="dd883-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dd883-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd883-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="dd883-121">categoryDescriptions</span></span>|[<span data-ttu-id="dd883-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="dd883-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="dd883-123">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="dd883-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="dd883-124">id</span><span class="sxs-lookup"><span data-stu-id="dd883-124">id</span></span>|<span data-ttu-id="dd883-125">Строка</span><span class="sxs-lookup"><span data-stu-id="dd883-125">String</span></span>| <span data-ttu-id="dd883-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd883-126">Read-only.</span></span> <span data-ttu-id="dd883-127">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="dd883-127">ID of the plan details.</span></span> <span data-ttu-id="dd883-128">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="dd883-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="dd883-129">[Формат](planner-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="dd883-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="dd883-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="dd883-130">sharedWith</span></span>|[<span data-ttu-id="dd883-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="dd883-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="dd883-p104">Список идентификаторов пользователей, у которых есть доступ к этому плану. Если вы используете Группы Office 365, то для предоставления доступа к плану [группы](group.md) используйте API Групп. Вы также можете добавить в эту коллекцию существующих членов группы, но они смогут получить доступ к плану, принадлежащему группе, и без этого.</span><span class="sxs-lookup"><span data-stu-id="dd883-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dd883-135">Связи</span><span class="sxs-lookup"><span data-stu-id="dd883-135">Relationships</span></span>
<span data-ttu-id="dd883-136">Нет</span><span class="sxs-lookup"><span data-stu-id="dd883-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd883-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd883-137">JSON representation</span></span>
<span data-ttu-id="dd883-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd883-138">Here is a JSON representation of the resource.</span></span>

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
