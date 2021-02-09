---
title: Тип ресурса accessReviewInstanceDecisionItem
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10166dc9da512bf74a0b4e5ad97f4797cdf6c317
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159201"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="6982b-103">Тип ресурса accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="6982b-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="6982b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6982b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6982b-105">Представляет решение о проверке [доступа](accessreviewsv2-root.md) Azure AD для экземпляра проверки.</span><span class="sxs-lookup"><span data-stu-id="6982b-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="6982b-106">Это решение представляет определение доступа пользователя или директора-службы для данного экземпляра [проверки доступа.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="6982b-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6982b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6982b-107">Methods</span></span>

| <span data-ttu-id="6982b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6982b-108">Method</span></span> | <span data-ttu-id="6982b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6982b-109">Return Type</span></span> | <span data-ttu-id="6982b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6982b-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="6982b-111">Список accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="6982b-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="6982b-112">[Коллекция accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="6982b-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="6982b-113">Перечисляет все accessReviewInstanceDecisionItem для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="6982b-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="6982b-114">Список accessReviewInstanceDecisionItems, ожидающих утверждения</span><span class="sxs-lookup"><span data-stu-id="6982b-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="6982b-115">[коллекция accessReviewInstanceDecisionItem;](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="6982b-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="6982b-116">Получите все accessReviewInstanceDecisionItems, присвоенные вызыванию пользователю, для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="6982b-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="6982b-117">Обновление accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="6982b-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="6982b-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="6982b-118">None.</span></span> | <span data-ttu-id="6982b-119">Для любых объектов accessReviewInstanceDecisionItems, в которые назначен вызывающий пользователь, вызывающий пользователь может записать решение, обновив объект решения.</span><span class="sxs-lookup"><span data-stu-id="6982b-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6982b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="6982b-120">Properties</span></span>
| <span data-ttu-id="6982b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="6982b-121">Property</span></span> | <span data-ttu-id="6982b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6982b-122">Type</span></span> |  <span data-ttu-id="6982b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6982b-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="6982b-124">id</span><span class="sxs-lookup"><span data-stu-id="6982b-124">id</span></span> | <span data-ttu-id="6982b-125">String</span><span class="sxs-lookup"><span data-stu-id="6982b-125">String</span></span> | <span data-ttu-id="6982b-126">Идентификатор решения.</span><span class="sxs-lookup"><span data-stu-id="6982b-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="6982b-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="6982b-127">accessReviewId</span></span> | <span data-ttu-id="6982b-128">String</span><span class="sxs-lookup"><span data-stu-id="6982b-128">String</span></span> | <span data-ttu-id="6982b-129">Идентификатор родительского accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="6982b-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="6982b-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="6982b-130">reviewedBy</span></span> | [<span data-ttu-id="6982b-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6982b-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="6982b-132">Идентификатор проверяемого.</span><span class="sxs-lookup"><span data-stu-id="6982b-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="6982b-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="6982b-133">reviewedDateTime</span></span> | <span data-ttu-id="6982b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6982b-134">DateTimeOffset</span></span> | <span data-ttu-id="6982b-135">Дата и время проверки.</span><span class="sxs-lookup"><span data-stu-id="6982b-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="6982b-136">decision</span><span class="sxs-lookup"><span data-stu-id="6982b-136">decision</span></span> | <span data-ttu-id="6982b-137">String</span><span class="sxs-lookup"><span data-stu-id="6982b-137">String</span></span> | <span data-ttu-id="6982b-138">Результат проверки.</span><span class="sxs-lookup"><span data-stu-id="6982b-138">Result of the review.</span></span> <span data-ttu-id="6982b-139">Возможные значения: `Approve` , , , или `Deny` `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="6982b-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="6982b-140">обоснование</span><span class="sxs-lookup"><span data-stu-id="6982b-140">justification</span></span> | <span data-ttu-id="6982b-141">String</span><span class="sxs-lookup"><span data-stu-id="6982b-141">String</span></span> | <span data-ttu-id="6982b-142">Обоснование принятия решения о проверке.</span><span class="sxs-lookup"><span data-stu-id="6982b-142">The review decision justification.</span></span> |
| <span data-ttu-id="6982b-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="6982b-143">appliedBy</span></span> | [<span data-ttu-id="6982b-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6982b-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="6982b-145">Идентификатор пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="6982b-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="6982b-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="6982b-146">appliedDateTime</span></span> | <span data-ttu-id="6982b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6982b-147">DateTimeOffset</span></span> | <span data-ttu-id="6982b-148">Дата и время, когда было применено решение об утверждении.</span><span class="sxs-lookup"><span data-stu-id="6982b-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="6982b-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="6982b-149">applyResult</span></span> | <span data-ttu-id="6982b-150">String</span><span class="sxs-lookup"><span data-stu-id="6982b-150">String</span></span> | <span data-ttu-id="6982b-151">Результат применения решения.</span><span class="sxs-lookup"><span data-stu-id="6982b-151">The result of applying the decision.</span></span> <span data-ttu-id="6982b-152">Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="6982b-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="6982b-153">recommendation</span><span class="sxs-lookup"><span data-stu-id="6982b-153">recommendation</span></span> | <span data-ttu-id="6982b-154">String</span><span class="sxs-lookup"><span data-stu-id="6982b-154">String</span></span> | <span data-ttu-id="6982b-155">Системная рекомендация для решения об утверждении.</span><span class="sxs-lookup"><span data-stu-id="6982b-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="6982b-156">Возможные значения: `Approve` , `Deny` , или `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="6982b-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="6982b-157">target</span><span class="sxs-lookup"><span data-stu-id="6982b-157">target</span></span> | [<span data-ttu-id="6982b-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="6982b-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="6982b-159">Цель конкретного решения.</span><span class="sxs-lookup"><span data-stu-id="6982b-159">The target of this specific decision.</span></span> <span data-ttu-id="6982b-160">Целевые объекты принятия решений могут быть разных типов , каждый из которых имеет собственные свойства.</span><span class="sxs-lookup"><span data-stu-id="6982b-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="6982b-161">См. [accessReviewInstanceDecisionItemTarget.](accessreviewinstancedecisionitemtarget.md)</span><span class="sxs-lookup"><span data-stu-id="6982b-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="6982b-162">Связи</span><span class="sxs-lookup"><span data-stu-id="6982b-162">Relationships</span></span>

| <span data-ttu-id="6982b-163">Связь</span><span class="sxs-lookup"><span data-stu-id="6982b-163">Relationship</span></span> | <span data-ttu-id="6982b-164">Тип</span><span class="sxs-lookup"><span data-stu-id="6982b-164">Type</span></span>   |<span data-ttu-id="6982b-165">Описание</span><span class="sxs-lookup"><span data-stu-id="6982b-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6982b-166">экземпляр</span><span class="sxs-lookup"><span data-stu-id="6982b-166">instance</span></span> |[<span data-ttu-id="6982b-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="6982b-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="6982b-168">С каждым решением связан только один accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="6982b-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="6982b-169">Экземпляр является родительским элементом элемента решения, представляющим повторение проверки доступа, на которое было принято решение.</span><span class="sxs-lookup"><span data-stu-id="6982b-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6982b-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6982b-170">JSON representation</span></span>

<span data-ttu-id="6982b-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6982b-171">Here is a JSON representation of the resource.</span></span>

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
