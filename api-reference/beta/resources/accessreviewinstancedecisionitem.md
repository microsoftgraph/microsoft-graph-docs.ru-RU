---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e5d9b64faafb7dfe4ec4e6f3487643e62885236a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952818"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="6894b-103">accessReviewInstanceDecisionItem type</span><span class="sxs-lookup"><span data-stu-id="6894b-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="6894b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6894b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="6894b-105">Представляет решение о проверке доступа к Azure [AD](accessreviewsv2-root.md) в экземпляре проверки.</span><span class="sxs-lookup"><span data-stu-id="6894b-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="6894b-106">Это решение представляет определение доступа пользователя или директора службы для данного экземпляра [обзора доступа.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="6894b-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6894b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6894b-107">Methods</span></span>

| <span data-ttu-id="6894b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6894b-108">Method</span></span> | <span data-ttu-id="6894b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6894b-109">Return Type</span></span> | <span data-ttu-id="6894b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6894b-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="6894b-111">List accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="6894b-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="6894b-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="6894b-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="6894b-113">Списки всех accessReviewInstanceDecisionItem для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="6894b-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="6894b-114">Список accessReviewInstanceDecisionItems до утверждения</span><span class="sxs-lookup"><span data-stu-id="6894b-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="6894b-115">[accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="6894b-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="6894b-116">Получите все accessReviewInstanceDecisionItems, назначенные вызываемой пользователю, для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="6894b-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="6894b-117">Обновление accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="6894b-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="6894b-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6894b-118">None.</span></span> | <span data-ttu-id="6894b-119">Для любого accessReviewInstanceDecisionItems, на который вызывается пользователь, на который назначен рецензент, вызывающий пользователь может записать решение, заплатив объект решения.</span><span class="sxs-lookup"><span data-stu-id="6894b-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6894b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="6894b-120">Properties</span></span>
| <span data-ttu-id="6894b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="6894b-121">Property</span></span> | <span data-ttu-id="6894b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6894b-122">Type</span></span> |  <span data-ttu-id="6894b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6894b-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="6894b-124">id</span><span class="sxs-lookup"><span data-stu-id="6894b-124">id</span></span> | <span data-ttu-id="6894b-125">Строка</span><span class="sxs-lookup"><span data-stu-id="6894b-125">String</span></span> | <span data-ttu-id="6894b-126">Идентификатор решения.</span><span class="sxs-lookup"><span data-stu-id="6894b-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="6894b-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="6894b-127">accessReviewId</span></span> | <span data-ttu-id="6894b-128">Строка</span><span class="sxs-lookup"><span data-stu-id="6894b-128">String</span></span> | <span data-ttu-id="6894b-129">Идентификатор родителя accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="6894b-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="6894b-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="6894b-130">reviewedBy</span></span> | [<span data-ttu-id="6894b-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6894b-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="6894b-132">Идентификатор рецензента.</span><span class="sxs-lookup"><span data-stu-id="6894b-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="6894b-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="6894b-133">reviewedDateTime</span></span> | <span data-ttu-id="6894b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6894b-134">DateTimeOffset</span></span> | <span data-ttu-id="6894b-135">Время, затмив время проверки.</span><span class="sxs-lookup"><span data-stu-id="6894b-135">The timestamp when the review occurred.</span></span> |
| <span data-ttu-id="6894b-136">решение</span><span class="sxs-lookup"><span data-stu-id="6894b-136">decision</span></span> | <span data-ttu-id="6894b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="6894b-137">String</span></span> | <span data-ttu-id="6894b-138">Результат проверки.</span><span class="sxs-lookup"><span data-stu-id="6894b-138">Result of the review.</span></span> <span data-ttu-id="6894b-139">Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="6894b-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="6894b-140">обоснование</span><span class="sxs-lookup"><span data-stu-id="6894b-140">justification</span></span> | <span data-ttu-id="6894b-141">Строка</span><span class="sxs-lookup"><span data-stu-id="6894b-141">String</span></span> | <span data-ttu-id="6894b-142">Обоснование решения по пересмотру.</span><span class="sxs-lookup"><span data-stu-id="6894b-142">The review decision justification.</span></span> |
| <span data-ttu-id="6894b-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="6894b-143">appliedBy</span></span> | [<span data-ttu-id="6894b-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6894b-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="6894b-145">Идентификатор пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="6894b-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="6894b-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="6894b-146">appliedDateTime</span></span> | <span data-ttu-id="6894b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6894b-147">DateTimeOffset</span></span> | <span data-ttu-id="6894b-148">Время, за которое было применено решение об утверждении.</span><span class="sxs-lookup"><span data-stu-id="6894b-148">The timestamp when the approval decision was applied.</span></span> <span data-ttu-id="6894b-149">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="6894b-149">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6894b-150">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6894b-150">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="6894b-151">applyResult</span><span class="sxs-lookup"><span data-stu-id="6894b-151">applyResult</span></span> | <span data-ttu-id="6894b-152">Строка</span><span class="sxs-lookup"><span data-stu-id="6894b-152">String</span></span> | <span data-ttu-id="6894b-153">Результат применения решения.</span><span class="sxs-lookup"><span data-stu-id="6894b-153">The result of applying the decision.</span></span> <span data-ttu-id="6894b-154">Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="6894b-154">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="6894b-155">рекомендация</span><span class="sxs-lookup"><span data-stu-id="6894b-155">recommendation</span></span> | <span data-ttu-id="6894b-156">Строка</span><span class="sxs-lookup"><span data-stu-id="6894b-156">String</span></span> | <span data-ttu-id="6894b-157">Сгенерированная системой рекомендация для принятия решения об утверждении.</span><span class="sxs-lookup"><span data-stu-id="6894b-157">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="6894b-158">Возможные значения: `Approve` `Deny` , или `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="6894b-158">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="6894b-159">target</span><span class="sxs-lookup"><span data-stu-id="6894b-159">target</span></span> | [<span data-ttu-id="6894b-160">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="6894b-160">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="6894b-161">Цель этого конкретного решения.</span><span class="sxs-lookup"><span data-stu-id="6894b-161">The target of this specific decision.</span></span> <span data-ttu-id="6894b-162">Целевые показатели принятия решений могут быть разных типов , каждый из которых имеет свои собственные свойства.</span><span class="sxs-lookup"><span data-stu-id="6894b-162">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="6894b-163">См. [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="6894b-163">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="6894b-164">Связи</span><span class="sxs-lookup"><span data-stu-id="6894b-164">Relationships</span></span>

| <span data-ttu-id="6894b-165">Связь</span><span class="sxs-lookup"><span data-stu-id="6894b-165">Relationship</span></span> | <span data-ttu-id="6894b-166">Тип</span><span class="sxs-lookup"><span data-stu-id="6894b-166">Type</span></span>   |<span data-ttu-id="6894b-167">Описание</span><span class="sxs-lookup"><span data-stu-id="6894b-167">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6894b-168">экземпляр</span><span class="sxs-lookup"><span data-stu-id="6894b-168">instance</span></span> |[<span data-ttu-id="6894b-169">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="6894b-169">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="6894b-170">Существует точно один accessReviewInstance, связанный с каждым решением.</span><span class="sxs-lookup"><span data-stu-id="6894b-170">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="6894b-171">Экземпляр является родителем элемента решения, представляющего повторение проверки доступа, на которое принимается решение.</span><span class="sxs-lookup"><span data-stu-id="6894b-171">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6894b-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6894b-172">JSON representation</span></span>

<span data-ttu-id="6894b-173">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6894b-173">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "openType": true
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
 "id": "string (identifier)",
 "accessReviewId": "string",
 "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
 },
 "reviewedDateTime": "string (timestamp)",
 "decision": "string",
 "justification": "string",
 "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
 "appliedDateTime": "DateTimeOffset",
 "applyResult": "string",
 "recommendation": "string",
 "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
