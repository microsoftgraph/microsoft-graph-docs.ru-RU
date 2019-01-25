---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе и содержит коллекцию plannerTasks. Он также может иметь коллекцию plannerBuckets. Каждый объект плана имеет сведения о объекта, которое может содержать дополнительные сведения о плане. Дополнительные сведения о связях между группами, планы и задачи можно планировщик работы.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529553"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="1ef4b-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1ef4b-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ef4b-108">Ресурс **plannerPlan** представляет план в Office 365.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="1ef4b-109">План может принадлежать [группе](group.md) и содержит коллекцию [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="1ef4b-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="1ef4b-110">Он также может иметь коллекцию [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="1ef4b-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="1ef4b-111">Каждый объект плана имеет [сведения о](plannerplandetails.md) объекта, которое может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="1ef4b-112">Дополнительные сведения о связях между группами, планы и задачи можно [Планировщик работы](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="1ef4b-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="1ef4b-113">Методы</span><span class="sxs-lookup"><span data-stu-id="1ef4b-113">Methods</span></span>

| <span data-ttu-id="1ef4b-114">Метод</span><span class="sxs-lookup"><span data-stu-id="1ef4b-114">Method</span></span>           | <span data-ttu-id="1ef4b-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1ef4b-115">Return Type</span></span>    |<span data-ttu-id="1ef4b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef4b-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ef4b-117">Получение plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1ef4b-117">[Get plannerPlan](../api/plannerplan-get.md)</span></span> | [<span data-ttu-id="1ef4b-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1ef4b-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="1ef4b-119">Считывание свойств и связей объекта plannerPlan.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|<span data-ttu-id="1ef4b-120">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="1ef4b-120">[List buckets](../api/plannerplan-list-buckets.md)</span></span> |<span data-ttu-id="1ef4b-121">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="1ef4b-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="1ef4b-122">Получение коллекции объектов plannerBucket.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="1ef4b-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="1ef4b-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="1ef4b-124">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="1ef4b-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1ef4b-125">Получение коллекции объектов **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="1ef4b-126">Update</span><span class="sxs-lookup"><span data-stu-id="1ef4b-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="1ef4b-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1ef4b-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="1ef4b-128">Обновление объекта plannerPlan.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1ef4b-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ef4b-129">Properties</span></span>
| <span data-ttu-id="1ef4b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ef4b-130">Property</span></span>     | <span data-ttu-id="1ef4b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ef4b-131">Type</span></span>   |<span data-ttu-id="1ef4b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef4b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ef4b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ef4b-133">createdDateTime</span></span>|<span data-ttu-id="1ef4b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ef4b-134">DateTimeOffset</span></span>|<span data-ttu-id="1ef4b-p103">Только для чтения. Дата и время создания плана. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1ef4b-139">id</span><span class="sxs-lookup"><span data-stu-id="1ef4b-139">id</span></span>|<span data-ttu-id="1ef4b-140">String</span><span class="sxs-lookup"><span data-stu-id="1ef4b-140">String</span></span>| <span data-ttu-id="1ef4b-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-141">Read-only.</span></span> <span data-ttu-id="1ef4b-142">Идентификатор плана.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-142">ID of the plan.</span></span> <span data-ttu-id="1ef4b-143">Это 28 знаков без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1ef4b-144">[Формат](tasks-identifiers-disclaimer.md) проверяются на службу.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1ef4b-145">owner</span><span class="sxs-lookup"><span data-stu-id="1ef4b-145">owner</span></span>|<span data-ttu-id="1ef4b-146">String</span><span class="sxs-lookup"><span data-stu-id="1ef4b-146">String</span></span>|<span data-ttu-id="1ef4b-147">Идентификатор [группы](group.md) , который несет ответственность за планирование.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="1ef4b-148">В этом поле можно указать допустимое группы должен существовать.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="1ef4b-149">После его установки, это свойство не удается обновить.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="1ef4b-150">title</span><span class="sxs-lookup"><span data-stu-id="1ef4b-150">title</span></span>|<span data-ttu-id="1ef4b-151">String</span><span class="sxs-lookup"><span data-stu-id="1ef4b-151">String</span></span>|<span data-ttu-id="1ef4b-p106">Обязательный. Название плана.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="1ef4b-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="1ef4b-154">createdBy</span></span>|[<span data-ttu-id="1ef4b-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="1ef4b-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="1ef4b-p107">Только для чтения. Пользователь, создавший этот план.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-p107">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="1ef4b-158">контекстов</span><span class="sxs-lookup"><span data-stu-id="1ef4b-158">contexts</span></span>|<span data-ttu-id="1ef4b-159">[plannerPlanContextCollection](plannerplancontextcollection.md);</span><span class="sxs-lookup"><span data-stu-id="1ef4b-159">[plannerPlanContextCollection](plannerplancontextcollection.md)</span></span>| <span data-ttu-id="1ef4b-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-160">Read-only.</span></span> <span data-ttu-id="1ef4b-161">Дополнительные пользовательских интерфейсов, в которых используется этот план, представленные в виде [plannerPlanContext](plannerplancontext.md) записей.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ef4b-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ef4b-162">Relationships</span></span>
| <span data-ttu-id="1ef4b-163">Связь</span><span class="sxs-lookup"><span data-stu-id="1ef4b-163">Relationship</span></span> | <span data-ttu-id="1ef4b-164">Тип</span><span class="sxs-lookup"><span data-stu-id="1ef4b-164">Type</span></span>   |<span data-ttu-id="1ef4b-165">Описание</span><span class="sxs-lookup"><span data-stu-id="1ef4b-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ef4b-166">buckets</span><span class="sxs-lookup"><span data-stu-id="1ef4b-166">buckets</span></span>|<span data-ttu-id="1ef4b-167">Коллекция объектов [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="1ef4b-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="1ef4b-p109">Только для чтения. Допускает значение null. Коллекция контейнеров в плане.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="1ef4b-171">details</span><span class="sxs-lookup"><span data-stu-id="1ef4b-171">details</span></span>|<span data-ttu-id="1ef4b-172">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="1ef4b-172">[plannerPlanDetails](plannerplandetails.md)</span></span>| <span data-ttu-id="1ef4b-p110">Только для чтения. Допускает значение null. Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-p110">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="1ef4b-176">tasks</span><span class="sxs-lookup"><span data-stu-id="1ef4b-176">tasks</span></span>|<span data-ttu-id="1ef4b-177">Коллекция объектов [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="1ef4b-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1ef4b-p111">Только для чтения. Допускает значение null. Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-p111">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ef4b-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ef4b-181">JSON representation</span></span>

<span data-ttu-id="1ef4b-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ef4b-182">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
