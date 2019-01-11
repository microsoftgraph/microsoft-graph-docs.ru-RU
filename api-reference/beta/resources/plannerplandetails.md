---
title: Тип ресурса plannerPlanDetails
description: Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом plan связан объект details.
localization_priority: Normal
ms.openlocfilehash: 117a2f69324180a7ef45dcf96c773f510bdbcb9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860160"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="a8ad7-104">Тип ресурса plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8ad7-104">plannerPlanDetails resource type</span></span>

> <span data-ttu-id="a8ad7-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8ad7-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8ad7-p103">Ресурс **plannerPlanDetails** представляет дополнительные сведения о плане. С каждым объектом [plan](plannerplan.md) связан объект details.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-p103">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="a8ad7-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a8ad7-109">Methods</span></span>

| <span data-ttu-id="a8ad7-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a8ad7-110">Method</span></span>           | <span data-ttu-id="a8ad7-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8ad7-111">Return Type</span></span>    |<span data-ttu-id="a8ad7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ad7-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8ad7-113">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8ad7-113">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="a8ad7-114">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8ad7-114">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="a8ad7-115">Чтение свойства и связи объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="a8ad7-115">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="a8ad7-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="a8ad7-116">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="a8ad7-117">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a8ad7-117">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="a8ad7-118">Обновление объекта **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="a8ad7-118">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a8ad7-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8ad7-119">Properties</span></span>
| <span data-ttu-id="a8ad7-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8ad7-120">Property</span></span>     | <span data-ttu-id="a8ad7-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a8ad7-121">Type</span></span>   |<span data-ttu-id="a8ad7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ad7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8ad7-123">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a8ad7-123">categoryDescriptions</span></span>|[<span data-ttu-id="a8ad7-124">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a8ad7-124">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="a8ad7-125">Объект с описаниями шести категорий, которые могут быть связаны с задачами в плане.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-125">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="a8ad7-126">id</span><span class="sxs-lookup"><span data-stu-id="a8ad7-126">id</span></span>|<span data-ttu-id="a8ad7-127">Строка</span><span class="sxs-lookup"><span data-stu-id="a8ad7-127">String</span></span>| <span data-ttu-id="a8ad7-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-128">Read-only.</span></span> <span data-ttu-id="a8ad7-129">Идентификатор сведений о плане.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-129">The ID of the plan details.</span></span> <span data-ttu-id="a8ad7-130">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-130">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a8ad7-131">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-131">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a8ad7-132">sharedWith</span><span class="sxs-lookup"><span data-stu-id="a8ad7-132">sharedWith</span></span>|[<span data-ttu-id="a8ad7-133">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="a8ad7-133">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="a8ad7-134">Набор, этот план используется совместно с идентификаторами пользователей.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-134">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="a8ad7-135">Если вы используете Office 365 групп, используйте группы API для управления членством в группе для совместного использования плана [группы](group.md) .</span><span class="sxs-lookup"><span data-stu-id="a8ad7-135">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="a8ad7-136">Можно также добавить существующих членов группы этой коллекции, несмотря на то, что в порядке их для доступа к плана, принадлежащих группе не требуется.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-136">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="a8ad7-137">contextDetails</span><span class="sxs-lookup"><span data-stu-id="a8ad7-137">contextDetails</span></span>|<span data-ttu-id="a8ad7-138">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md);</span><span class="sxs-lookup"><span data-stu-id="a8ad7-138">[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)</span></span>|<span data-ttu-id="a8ad7-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-139">Read-only.</span></span> <span data-ttu-id="a8ad7-140">Коллекция Дополнительные сведения, связанные с записями [plannerPlanContext](plannerplancontext.md) , определенных для контейнера [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="a8ad7-140">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a8ad7-141">Связи</span><span class="sxs-lookup"><span data-stu-id="a8ad7-141">Relationships</span></span>
<span data-ttu-id="a8ad7-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a8ad7-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a8ad7-143">JSON representation</span></span>
<span data-ttu-id="a8ad7-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8ad7-144">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
