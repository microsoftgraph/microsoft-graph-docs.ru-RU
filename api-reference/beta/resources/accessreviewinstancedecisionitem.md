---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 228fbe473fe65fe84c9dfa7c62f3689681d47e39
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443190"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="24009-103">accessReviewInstanceDecisionItem type</span><span class="sxs-lookup"><span data-stu-id="24009-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="24009-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24009-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="24009-105">Представляет решение о проверке доступа к Azure [AD](accessreviewsv2-root.md) в экземпляре проверки.</span><span class="sxs-lookup"><span data-stu-id="24009-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="24009-106">Это решение представляет определение доступа пользователя или директора службы для данного экземпляра [обзора доступа.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="24009-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="24009-107">Методы</span><span class="sxs-lookup"><span data-stu-id="24009-107">Methods</span></span>

| <span data-ttu-id="24009-108">Метод</span><span class="sxs-lookup"><span data-stu-id="24009-108">Method</span></span> | <span data-ttu-id="24009-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24009-109">Return Type</span></span> | <span data-ttu-id="24009-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24009-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="24009-111">List accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="24009-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="24009-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="24009-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="24009-113">Списки всех accessReviewInstanceDecisionItem для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="24009-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="24009-114">Список accessReviewInstanceDecisionItems до утверждения</span><span class="sxs-lookup"><span data-stu-id="24009-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="24009-115">[accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="24009-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="24009-116">Получите все accessReviewInstanceDecisionItems, назначенные вызываемой пользователю, для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="24009-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="24009-117">Обновление accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="24009-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="24009-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="24009-118">None.</span></span> | <span data-ttu-id="24009-119">Для любого accessReviewInstanceDecisionItems, на который вызывается пользователь, на который назначен рецензент, вызывающий пользователь может записать решение, заплатив объект решения.</span><span class="sxs-lookup"><span data-stu-id="24009-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="24009-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="24009-120">Properties</span></span>
| <span data-ttu-id="24009-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="24009-121">Property</span></span> | <span data-ttu-id="24009-122">Тип</span><span class="sxs-lookup"><span data-stu-id="24009-122">Type</span></span> |  <span data-ttu-id="24009-123">Описание</span><span class="sxs-lookup"><span data-stu-id="24009-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="24009-124">id</span><span class="sxs-lookup"><span data-stu-id="24009-124">id</span></span> | <span data-ttu-id="24009-125">String</span><span class="sxs-lookup"><span data-stu-id="24009-125">String</span></span> | <span data-ttu-id="24009-126">Идентификатор решения.</span><span class="sxs-lookup"><span data-stu-id="24009-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="24009-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="24009-127">accessReviewId</span></span> | <span data-ttu-id="24009-128">String</span><span class="sxs-lookup"><span data-stu-id="24009-128">String</span></span> | <span data-ttu-id="24009-129">Идентификатор родителя accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="24009-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="24009-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="24009-130">reviewedBy</span></span> | [<span data-ttu-id="24009-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="24009-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="24009-132">Идентификатор рецензента.</span><span class="sxs-lookup"><span data-stu-id="24009-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="24009-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="24009-133">reviewedDateTime</span></span> | <span data-ttu-id="24009-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24009-134">DateTimeOffset</span></span> | <span data-ttu-id="24009-135">DateTime при просмотре.</span><span class="sxs-lookup"><span data-stu-id="24009-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="24009-136">решение</span><span class="sxs-lookup"><span data-stu-id="24009-136">decision</span></span> | <span data-ttu-id="24009-137">String</span><span class="sxs-lookup"><span data-stu-id="24009-137">String</span></span> | <span data-ttu-id="24009-138">Результат проверки.</span><span class="sxs-lookup"><span data-stu-id="24009-138">Result of the review.</span></span> <span data-ttu-id="24009-139">Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="24009-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="24009-140">обоснование</span><span class="sxs-lookup"><span data-stu-id="24009-140">justification</span></span> | <span data-ttu-id="24009-141">String</span><span class="sxs-lookup"><span data-stu-id="24009-141">String</span></span> | <span data-ttu-id="24009-142">Обоснование решения по пересмотру.</span><span class="sxs-lookup"><span data-stu-id="24009-142">The review decision justification.</span></span> |
| <span data-ttu-id="24009-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="24009-143">appliedBy</span></span> | [<span data-ttu-id="24009-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="24009-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="24009-145">Идентификатор пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="24009-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="24009-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="24009-146">appliedDateTime</span></span> | <span data-ttu-id="24009-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24009-147">DateTimeOffset</span></span> | <span data-ttu-id="24009-148">DateTime, когда было применено решение об утверждении.</span><span class="sxs-lookup"><span data-stu-id="24009-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="24009-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="24009-149">applyResult</span></span> | <span data-ttu-id="24009-150">String</span><span class="sxs-lookup"><span data-stu-id="24009-150">String</span></span> | <span data-ttu-id="24009-151">Результат применения решения.</span><span class="sxs-lookup"><span data-stu-id="24009-151">The result of applying the decision.</span></span> <span data-ttu-id="24009-152">Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="24009-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="24009-153">рекомендация</span><span class="sxs-lookup"><span data-stu-id="24009-153">recommendation</span></span> | <span data-ttu-id="24009-154">String</span><span class="sxs-lookup"><span data-stu-id="24009-154">String</span></span> | <span data-ttu-id="24009-155">Сгенерированная системой рекомендация для принятия решения об утверждении.</span><span class="sxs-lookup"><span data-stu-id="24009-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="24009-156">Возможные значения: `Approve` `Deny` , или `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="24009-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="24009-157">target</span><span class="sxs-lookup"><span data-stu-id="24009-157">target</span></span> | [<span data-ttu-id="24009-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="24009-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="24009-159">Цель этого конкретного решения.</span><span class="sxs-lookup"><span data-stu-id="24009-159">The target of this specific decision.</span></span> <span data-ttu-id="24009-160">Целевые показатели принятия решений могут быть разных типов , каждый из которых имеет свои собственные свойства.</span><span class="sxs-lookup"><span data-stu-id="24009-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="24009-161">См. [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="24009-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="24009-162">Связи</span><span class="sxs-lookup"><span data-stu-id="24009-162">Relationships</span></span>

| <span data-ttu-id="24009-163">Связь</span><span class="sxs-lookup"><span data-stu-id="24009-163">Relationship</span></span> | <span data-ttu-id="24009-164">Тип</span><span class="sxs-lookup"><span data-stu-id="24009-164">Type</span></span>   |<span data-ttu-id="24009-165">Описание</span><span class="sxs-lookup"><span data-stu-id="24009-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24009-166">экземпляр</span><span class="sxs-lookup"><span data-stu-id="24009-166">instance</span></span> |[<span data-ttu-id="24009-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="24009-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="24009-168">Существует точно один accessReviewInstance, связанный с каждым решением.</span><span class="sxs-lookup"><span data-stu-id="24009-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="24009-169">Экземпляр является родителем элемента решения, представляющего повторение проверки доступа, на которое принимается решение.</span><span class="sxs-lookup"><span data-stu-id="24009-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="24009-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24009-170">JSON representation</span></span>

<span data-ttu-id="24009-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24009-171">Here is a JSON representation of the resource.</span></span>

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
