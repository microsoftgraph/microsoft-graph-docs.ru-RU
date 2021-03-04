---
title: тип ресурсов accessReviewInstance
description: Представляет собой повторение `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a0003ab8a79372a4dfefea1a62120ea8e40fa2c1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443197"
---
# <a name="accessreviewinstance-resource-type"></a><span data-ttu-id="cf5b7-103">тип ресурсов accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="cf5b7-103">accessReviewInstance resource type</span></span>

<span data-ttu-id="cf5b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf5b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="cf5b7-105">Представляет повторение проверки доступа Azure [AD.](accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="cf5b7-105">Represents an Azure AD [access review](accessreviewsv2-root.md) recurrence.</span></span> <span data-ttu-id="cf5b7-106">Если родительский [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) является повторяемой проверкой доступа, экземпляры представляют каждое повторение.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-106">If the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="cf5b7-107">Обзор, который не повторяется, будет иметь точно один экземпляр.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-107">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="cf5b7-108">Экземпляры также представляют каждую уникальную группу, проверяемую в определении расписания.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-108">Instances also represent each unique group being reviewed in the schedule definition.</span></span> <span data-ttu-id="cf5b7-109">Если определение расписания проверяет несколько групп, каждая группа будет иметь уникальный экземпляр для каждого повторения.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-109">If a schedule definition reviews multiple groups, each group will have a unique instance for each recurrence.</span></span>

<span data-ttu-id="cf5b7-110">Каждый **accessReviewInstance содержит** список решений, которые могут приниматься рецензентами. [](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="cf5b7-110">Every **accessReviewInstance** contains a list of [decisions](accessreviewinstancedecisionitem.md) that reviewers can take action on.</span></span> <span data-ttu-id="cf5b7-111">Существует одно решение для каждого проверяемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-111">There is one decision per identity being reviewed.</span></span>

## <a name="methods"></a><span data-ttu-id="cf5b7-112">Методы</span><span class="sxs-lookup"><span data-stu-id="cf5b7-112">Methods</span></span>

| <span data-ttu-id="cf5b7-113">Метод</span><span class="sxs-lookup"><span data-stu-id="cf5b7-113">Method</span></span> | <span data-ttu-id="cf5b7-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cf5b7-114">Return Type</span></span> | <span data-ttu-id="cf5b7-115">Описание</span><span class="sxs-lookup"><span data-stu-id="cf5b7-115">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf5b7-116">Список accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="cf5b7-116">List accessReviewInstances</span></span>](../api/accessreviewinstance-list.md) | <span data-ttu-id="cf5b7-117">[accessReviewInstance](accessreviewinstance.md) collection</span><span class="sxs-lookup"><span data-stu-id="cf5b7-117">[accessReviewInstance](accessreviewinstance.md) collection</span></span> | <span data-ttu-id="cf5b7-118">Получите список объектов [accessReviewInstance](../resources/accessreviewinstance.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-118">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span> |
|[<span data-ttu-id="cf5b7-119">Получить accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="cf5b7-119">Get accessReviewInstance</span></span>](../api/accessreviewinstance-get.md) | [<span data-ttu-id="cf5b7-120">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="cf5b7-120">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="cf5b7-121">Возвращает accessReviewInstance для accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-121">Returns accessReviewInstance for an accessReviewScheduleDefinition.</span></span> <span data-ttu-id="cf5b7-122">Не включает связанный accessReviewInstanceDecisionItem в объекте.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-122">Does not include associated accessReviewInstanceDecisionItem\`s in the object.</span></span> |
|[<span data-ttu-id="cf5b7-123">Список ожидающихAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="cf5b7-123">List pendingAccessReviewInstances</span></span>](../api/accessreviewinstance-pendingaccessreviewinstances.md) | <span data-ttu-id="cf5b7-124">[accessReviewInstance collection.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="cf5b7-124">[accessReviewInstance](accessreviewinstance.md) collection.</span></span> | <span data-ttu-id="cf5b7-125">Получите все ожидающих accessReviewInstance ресурсы, назначенные вызываемой пользователю.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-125">Get all pending accessReviewInstance resources assigned to the calling user.</span></span> |
|[<span data-ttu-id="cf5b7-126">Отправка напоминания accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="cf5b7-126">Send accessReviewInstance reminder</span></span>](../api/accessreviewinstance-sendreminder.md) | <span data-ttu-id="cf5b7-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-127">None.</span></span> | <span data-ttu-id="cf5b7-128">Отправьте напоминание рецензентам accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-128">Send a reminder to the reviewers of an accessReviewInstance.</span></span> |
|[<span data-ttu-id="cf5b7-129">Остановка accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="cf5b7-129">Stop accessReviewInstance</span></span>](../api/accessreviewinstance-stop.md) | <span data-ttu-id="cf5b7-130">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-130">None.</span></span> | <span data-ttu-id="cf5b7-131">Вручную остановите accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-131">Manually stop an accessReviewInstance.</span></span> |
|[<span data-ttu-id="cf5b7-132">Принятие рекомендаций</span><span class="sxs-lookup"><span data-stu-id="cf5b7-132">Accept recommendations</span></span>](../api/accessreviewinstance-acceptrecommendations.md) | <span data-ttu-id="cf5b7-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-133">None.</span></span> | <span data-ttu-id="cf5b7-134">Позволяет вызываемой пользователю принять рекомендацию по принятию решений для каждого notReviewed accessReviewInstanceDecisionItem, на которых он является рецензентом для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-134">Allows the calling user to accept the decision recommendation for each NotReviewed accessReviewInstanceDecisionItem that they are the reviewer on for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="cf5b7-135">Применение решений</span><span class="sxs-lookup"><span data-stu-id="cf5b7-135">Apply decisions</span></span>](../api/accessreviewinstance-applydecisions.md) | <span data-ttu-id="cf5b7-136">Нет.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-136">None.</span></span> | <span data-ttu-id="cf5b7-137">Вручную применить решение для accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-137">Manually apply decision on an accessReviewInstance.</span></span> |



## <a name="properties"></a><span data-ttu-id="cf5b7-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf5b7-138">Properties</span></span>
| <span data-ttu-id="cf5b7-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf5b7-139">Property</span></span> | <span data-ttu-id="cf5b7-140">Тип</span><span class="sxs-lookup"><span data-stu-id="cf5b7-140">Type</span></span> | <span data-ttu-id="cf5b7-141">Описание</span><span class="sxs-lookup"><span data-stu-id="cf5b7-141">Description</span></span> |
| :-------------------------| :---------------------------------- | :---------- |
| <span data-ttu-id="cf5b7-142">id</span><span class="sxs-lookup"><span data-stu-id="cf5b7-142">id</span></span> | <span data-ttu-id="cf5b7-143">String</span><span class="sxs-lookup"><span data-stu-id="cf5b7-143">String</span></span> | <span data-ttu-id="cf5b7-144">Уникальный идентификатор экземпляра.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-144">Unique identifier of the instance.</span></span> |
| <span data-ttu-id="cf5b7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cf5b7-145">displayName</span></span> | <span data-ttu-id="cf5b7-146">String</span><span class="sxs-lookup"><span data-stu-id="cf5b7-146">String</span></span> | <span data-ttu-id="cf5b7-147">Имя родительского доступаReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-147">Name of the parent accessReviewScheduleDefinition.</span></span> |
| <span data-ttu-id="cf5b7-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5b7-148">startDateTime</span></span> | <span data-ttu-id="cf5b7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5b7-149">DateTimeOffset</span></span> | <span data-ttu-id="cf5b7-150">DateTime при запуске экземпляра проверки.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-150">DateTime when review instance is scheduled to start.</span></span> <span data-ttu-id="cf5b7-151">Может быть в будущем.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-151">May be in the future.</span></span> |
| <span data-ttu-id="cf5b7-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="cf5b7-152">endDateTime</span></span> | <span data-ttu-id="cf5b7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf5b7-153">DateTimeOffset</span></span> | <span data-ttu-id="cf5b7-154">DateTime, когда экземпляр проверки должен завершиться.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-154">DateTime when review instance is scheduled to end.</span></span> |
| <span data-ttu-id="cf5b7-155">status</span><span class="sxs-lookup"><span data-stu-id="cf5b7-155">status</span></span> | <span data-ttu-id="cf5b7-156">string</span><span class="sxs-lookup"><span data-stu-id="cf5b7-156">string</span></span> | <span data-ttu-id="cf5b7-157">Указывает состояние accessReview.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-157">Specifies the status of an accessReview.</span></span> <span data-ttu-id="cf5b7-158">Типичные состояния `Initializing` включают , , , , , , и `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .</span><span class="sxs-lookup"><span data-stu-id="cf5b7-158">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span>  <span data-ttu-id="cf5b7-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-159">Read-only.</span></span>|
| <span data-ttu-id="cf5b7-160">scope</span><span class="sxs-lookup"><span data-stu-id="cf5b7-160">scope</span></span> | [<span data-ttu-id="cf5b7-161">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="cf5b7-161">accessReviewScope</span></span>](accessreviewscope.md) | <span data-ttu-id="cf5b7-162">Создан на **основе области** и **экземпляраEnumerationScope** на уровне accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-162">Created based on **scope** and **instanceEnumerationScope** at the accessReviewScheduleDefinition level.</span></span> <span data-ttu-id="cf5b7-163">Определяет область пользователей, рассмотренных в группе.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-163">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="cf5b7-164">В случае одногруппного обзора область, определяемая на уровне, `accessReviewScheduleDefinition` применяется ко всем экземплярам.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-164">In the case of a single-group review, the scope defined at the `accessReviewScheduleDefinition` level applies to all instances.</span></span> <span data-ttu-id="cf5b7-165">В случае проверки всех групп область действия для каждой группы может быть различной.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-165">In the case of all groups review, scope may be different for each group.</span></span> <span data-ttu-id="cf5b7-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-166">Read-only.</span></span>  | 
| <span data-ttu-id="cf5b7-167">решения</span><span class="sxs-lookup"><span data-stu-id="cf5b7-167">decisions</span></span> | <span data-ttu-id="cf5b7-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="cf5b7-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="cf5b7-169">Каждый пользователь, рассмотренный в accessReviewInstance, имеет элемент решения, представляющий, был ли его доступ одобрен, отклонен или еще не рассмотрен.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-169">Each user reviewed in an accessReviewInstance has a decision item representing if their access was approved, denied, or not yet reviewed.</span></span> |
| <span data-ttu-id="cf5b7-170">определение</span><span class="sxs-lookup"><span data-stu-id="cf5b7-170">definition</span></span> |[<span data-ttu-id="cf5b7-171">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="cf5b7-171">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="cf5b7-172">Существует точно один accessReviewScheduleDefinition, связанный с каждым экземпляром.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-172">There is exactly one accessReviewScheduleDefinition associated with each instance.</span></span> <span data-ttu-id="cf5b7-173">Это родительское расписание экземпляра, в котором создаются экземпляры для каждого повторения определения обзора и каждой группы, выбранной для проверки по определению.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-173">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cf5b7-174">Связи</span><span class="sxs-lookup"><span data-stu-id="cf5b7-174">Relationships</span></span>

| <span data-ttu-id="cf5b7-175">Связь</span><span class="sxs-lookup"><span data-stu-id="cf5b7-175">Relationship</span></span> | <span data-ttu-id="cf5b7-176">Тип</span><span class="sxs-lookup"><span data-stu-id="cf5b7-176">Type</span></span>   |<span data-ttu-id="cf5b7-177">Описание</span><span class="sxs-lookup"><span data-stu-id="cf5b7-177">Description</span></span>|
|:---------------|:--------|:----------|
| `definition`               |[<span data-ttu-id="cf5b7-178">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="cf5b7-178">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md)          | <span data-ttu-id="cf5b7-179">Существует точно один `accessReviewScheduleDefinition` связанный с каждым экземпляром.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-179">There is exactly one `accessReviewScheduleDefinition` associated with each instance.</span></span> <span data-ttu-id="cf5b7-180">Это родительское расписание экземпляра, в котором создаются экземпляры для каждого повторения определения обзора и каждой группы, выбранной для проверки по определению.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-180">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |
| `decisions`               |<span data-ttu-id="cf5b7-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="cf5b7-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span>        | <span data-ttu-id="cf5b7-182">Каждый пользователь, рассмотренный в элементе, имеет элемент решения, представляющий, были ли они утверждены, отклонены `accessReviewInstance` или еще не рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-182">Each user reviewed in an `accessReviewInstance` has a decision item representing if they were approved, denied, or not yet reviewed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf5b7-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf5b7-183">JSON representation</span></span>

<span data-ttu-id="cf5b7-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf5b7-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
