---
title: Тип ресурса plannerPlan
description: Ресурс **plannerPlan** представляет план в Office 365. План может принадлежать группе и содержать коллекцию перечисление plannertasks. Он также может иметь коллекцию Планнербуккетс. Каждый объект Plan содержит объект Details, который может содержать дополнительные сведения о плане. Более подробную информацию о связях между группами, планами и задачами можно узнать в разделе Планировщик.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578871"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="12db9-107">Тип ресурса plannerPlan</span><span class="sxs-lookup"><span data-stu-id="12db9-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12db9-108">Ресурс **plannerPlan** представляет план в Office 365.</span><span class="sxs-lookup"><span data-stu-id="12db9-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="12db9-109">План может принадлежать [группе](group.md) и содержать коллекцию [перечисление plannertasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="12db9-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="12db9-110">Он также может иметь коллекцию [планнербуккетс](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="12db9-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="12db9-111">Каждый объект Plan содержит объект [Details](plannerplandetails.md) , который может содержать дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="12db9-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="12db9-112">Более подробную информацию о связях между группами, планами и задачами можно узнать в разделе [планировщик](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="12db9-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="12db9-113">Методы</span><span class="sxs-lookup"><span data-stu-id="12db9-113">Methods</span></span>

| <span data-ttu-id="12db9-114">Метод</span><span class="sxs-lookup"><span data-stu-id="12db9-114">Method</span></span>           | <span data-ttu-id="12db9-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12db9-115">Return Type</span></span>    |<span data-ttu-id="12db9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="12db9-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12db9-117">Получение объекта plannerPlan</span><span class="sxs-lookup"><span data-stu-id="12db9-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="12db9-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="12db9-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="12db9-119">Чтение свойств и связей объекта **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="12db9-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="12db9-120">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="12db9-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="12db9-121">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="12db9-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="12db9-122">Получение коллекции объектов **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="12db9-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="12db9-123">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="12db9-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="12db9-124">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="12db9-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="12db9-125">Получение коллекции объектов **plannerTask** .</span><span class="sxs-lookup"><span data-stu-id="12db9-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="12db9-126">Обновление</span><span class="sxs-lookup"><span data-stu-id="12db9-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="12db9-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="12db9-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="12db9-128">Обновление объекта **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="12db9-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="12db9-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="12db9-129">Properties</span></span>
| <span data-ttu-id="12db9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="12db9-130">Property</span></span>     | <span data-ttu-id="12db9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="12db9-131">Type</span></span>   |<span data-ttu-id="12db9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="12db9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12db9-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12db9-133">createdDateTime</span></span>|<span data-ttu-id="12db9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12db9-134">DateTimeOffset</span></span>|<span data-ttu-id="12db9-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db9-135">Read-only.</span></span> <span data-ttu-id="12db9-136">Дата и время создания плана.</span><span class="sxs-lookup"><span data-stu-id="12db9-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="12db9-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="12db9-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12db9-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="12db9-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="12db9-139">id</span><span class="sxs-lookup"><span data-stu-id="12db9-139">id</span></span>|<span data-ttu-id="12db9-140">String</span><span class="sxs-lookup"><span data-stu-id="12db9-140">String</span></span>| <span data-ttu-id="12db9-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db9-141">Read-only.</span></span> <span data-ttu-id="12db9-142">ИДЕНТИФИКАТОР плана.</span><span class="sxs-lookup"><span data-stu-id="12db9-142">ID of the plan.</span></span> <span data-ttu-id="12db9-143">Содержит 28 знаков, учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="12db9-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="12db9-144">[Проверка формата](tasks-identifiers-disclaimer.md) проводится для службы.</span><span class="sxs-lookup"><span data-stu-id="12db9-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="12db9-145">owner</span><span class="sxs-lookup"><span data-stu-id="12db9-145">owner</span></span>|<span data-ttu-id="12db9-146">String</span><span class="sxs-lookup"><span data-stu-id="12db9-146">String</span></span>|<span data-ttu-id="12db9-147">Идентификатор [группы](group.md) , которой принадлежит план.</span><span class="sxs-lookup"><span data-stu-id="12db9-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="12db9-148">Для задания этого поля должна существовать допустимая группа.</span><span class="sxs-lookup"><span data-stu-id="12db9-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="12db9-149">После задания этого свойства это свойство невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="12db9-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="12db9-150">title</span><span class="sxs-lookup"><span data-stu-id="12db9-150">title</span></span>|<span data-ttu-id="12db9-151">String</span><span class="sxs-lookup"><span data-stu-id="12db9-151">String</span></span>|<span data-ttu-id="12db9-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12db9-152">Required.</span></span> <span data-ttu-id="12db9-153">Название плана.</span><span class="sxs-lookup"><span data-stu-id="12db9-153">Title of the plan.</span></span>|
|<span data-ttu-id="12db9-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="12db9-154">createdBy</span></span>|[<span data-ttu-id="12db9-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="12db9-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="12db9-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db9-156">Read-only.</span></span> <span data-ttu-id="12db9-157">Пользователь, создавший план.</span><span class="sxs-lookup"><span data-stu-id="12db9-157">The user who created the plan.</span></span>|
|<span data-ttu-id="12db9-158">контекстах</span><span class="sxs-lookup"><span data-stu-id="12db9-158">contexts</span></span>|<span data-ttu-id="12db9-159">[plannerPlanContextCollection](plannerplancontextcollection.md);</span><span class="sxs-lookup"><span data-stu-id="12db9-159">[plannerPlanContextCollection](plannerplancontextcollection.md)</span></span>| <span data-ttu-id="12db9-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db9-160">Read-only.</span></span> <span data-ttu-id="12db9-161">Дополнительные пользовательские взаимодействия, в которых используется этот план, представленный в виде записей [планнерпланконтекст](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="12db9-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12db9-162">Связи</span><span class="sxs-lookup"><span data-stu-id="12db9-162">Relationships</span></span>
| <span data-ttu-id="12db9-163">Отношение</span><span class="sxs-lookup"><span data-stu-id="12db9-163">Relationship</span></span> | <span data-ttu-id="12db9-164">Тип</span><span class="sxs-lookup"><span data-stu-id="12db9-164">Type</span></span>   |<span data-ttu-id="12db9-165">Описание</span><span class="sxs-lookup"><span data-stu-id="12db9-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12db9-166">сегментов</span><span class="sxs-lookup"><span data-stu-id="12db9-166">buckets</span></span>|<span data-ttu-id="12db9-167">Коллекция [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="12db9-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="12db9-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db9-168">Read-only.</span></span> <span data-ttu-id="12db9-169">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="12db9-169">Nullable.</span></span> <span data-ttu-id="12db9-170">Коллекция сегментов в плане.</span><span class="sxs-lookup"><span data-stu-id="12db9-170">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="12db9-171">подробности</span><span class="sxs-lookup"><span data-stu-id="12db9-171">details</span></span>|<span data-ttu-id="12db9-172">[plannerPlanDetails](plannerplandetails.md);</span><span class="sxs-lookup"><span data-stu-id="12db9-172">[plannerPlanDetails](plannerplandetails.md)</span></span>| <span data-ttu-id="12db9-173">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db9-173">Read-only.</span></span> <span data-ttu-id="12db9-174">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="12db9-174">Nullable.</span></span> <span data-ttu-id="12db9-175">Дополнительные сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="12db9-175">Additional details about the plan.</span></span>|
|<span data-ttu-id="12db9-176">tasks</span><span class="sxs-lookup"><span data-stu-id="12db9-176">tasks</span></span>|<span data-ttu-id="12db9-177">Коллекция [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="12db9-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="12db9-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="12db9-178">Read-only.</span></span> <span data-ttu-id="12db9-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="12db9-179">Nullable.</span></span> <span data-ttu-id="12db9-180">Коллекция задач в плане.</span><span class="sxs-lookup"><span data-stu-id="12db9-180">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12db9-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12db9-181">JSON representation</span></span>

<span data-ttu-id="12db9-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12db9-182">Here is a JSON representation of the resource.</span></span>

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
