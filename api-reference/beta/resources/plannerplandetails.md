---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом plan связан объект details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529882"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="29ac3-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="29ac3-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29ac3-p102">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="29ac3-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="29ac3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="29ac3-107">Methods</span></span>

| <span data-ttu-id="29ac3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="29ac3-108">Method</span></span>           | <span data-ttu-id="29ac3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29ac3-109">Return Type</span></span>    |<span data-ttu-id="29ac3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="29ac3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29ac3-111">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="29ac3-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | <span data-ttu-id="29ac3-112">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="29ac3-112">[plannerPlanDetails](plannerplandetails.md)</span></span> |<span data-ttu-id="29ac3-113">Чтение свойства и связи объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="29ac3-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="29ac3-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="29ac3-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="29ac3-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="29ac3-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="29ac3-116">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="29ac3-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="29ac3-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="29ac3-117">Properties</span></span>
| <span data-ttu-id="29ac3-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="29ac3-118">Property</span></span>     | <span data-ttu-id="29ac3-119">Тип</span><span class="sxs-lookup"><span data-stu-id="29ac3-119">Type</span></span>   |<span data-ttu-id="29ac3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="29ac3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29ac3-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="29ac3-121">categoryDescriptions</span></span>|[<span data-ttu-id="29ac3-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="29ac3-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="29ac3-123">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="29ac3-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="29ac3-124">id</span><span class="sxs-lookup"><span data-stu-id="29ac3-124">id</span></span>|<span data-ttu-id="29ac3-125">String</span><span class="sxs-lookup"><span data-stu-id="29ac3-125">String</span></span>| <span data-ttu-id="29ac3-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ac3-126">Read-only.</span></span> <span data-ttu-id="29ac3-127">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="29ac3-127">The ID of the plan details.</span></span> <span data-ttu-id="29ac3-128">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="29ac3-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="29ac3-129">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="29ac3-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="29ac3-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="29ac3-130">sharedWith</span></span>|[<span data-ttu-id="29ac3-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="29ac3-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="29ac3-132">Набор, этот план используется совместно с идентификаторами пользователей.</span><span class="sxs-lookup"><span data-stu-id="29ac3-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="29ac3-133">Если вы используете Office 365 групп, используйте группы API для управления членством в группе для совместного использования плана [группы](group.md) .</span><span class="sxs-lookup"><span data-stu-id="29ac3-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="29ac3-134">Можно также добавить существующих членов группы этой коллекции, несмотря на то, что в порядке их для доступа к плана, принадлежащих группе не требуется.</span><span class="sxs-lookup"><span data-stu-id="29ac3-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="29ac3-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="29ac3-135">contextDetails</span></span>|<span data-ttu-id="29ac3-136">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md);</span><span class="sxs-lookup"><span data-stu-id="29ac3-136">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)</span></span>|<span data-ttu-id="29ac3-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29ac3-137">Read-only.</span></span> <span data-ttu-id="29ac3-138">Коллекция Дополнительные сведения, связанные с записями [plannerPlanContext](plannerplancontext.md) , определенных для контейнера [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="29ac3-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="29ac3-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="29ac3-139">Relationships</span></span>
<span data-ttu-id="29ac3-140">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="29ac3-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="29ac3-141">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="29ac3-141">JSON representation</span></span>
<span data-ttu-id="29ac3-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29ac3-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplandetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
