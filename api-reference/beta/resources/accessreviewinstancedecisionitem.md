---
title: accessReviewInstanceDecisionItem type
description: Представляет решение о доступе пользователя к accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 968af49a9033ea749522132204d63b4f55ba25c7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469243"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="c87f2-103">accessReviewInstanceDecisionItem type</span><span class="sxs-lookup"><span data-stu-id="c87f2-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="c87f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c87f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

>[!NOTE]
><span data-ttu-id="c87f2-105">Свойство `target` будет обесценилось в v1.0 и заменено `principal` свойствами и `resource` .</span><span class="sxs-lookup"><span data-stu-id="c87f2-105">The property `target` will be deprecated in v1.0 and replaced by properties `principal` and `resource`.</span></span>

<span data-ttu-id="c87f2-106">Представляет решение о проверке доступа к Azure [AD](accessreviewsv2-root.md) в экземпляре проверки.</span><span class="sxs-lookup"><span data-stu-id="c87f2-106">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="c87f2-107">Это решение представляет определение доступа пользователя или директора службы для данного экземпляра [обзора доступа.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="c87f2-107">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c87f2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c87f2-108">Methods</span></span>

| <span data-ttu-id="c87f2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c87f2-109">Method</span></span> | <span data-ttu-id="c87f2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c87f2-110">Return Type</span></span> | <span data-ttu-id="c87f2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c87f2-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="c87f2-112">List accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="c87f2-112">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="c87f2-113">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="c87f2-113">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="c87f2-114">Списки всех accessReviewInstanceDecisionItem для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="c87f2-114">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="c87f2-115">Список accessReviewInstanceDecisionItems до утверждения</span><span class="sxs-lookup"><span data-stu-id="c87f2-115">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="c87f2-116">[accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="c87f2-116">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="c87f2-117">Получите все accessReviewInstanceDecisionItems, назначенные вызываемой пользователю, для определенного accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="c87f2-117">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="c87f2-118">Обновление accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="c87f2-118">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="c87f2-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="c87f2-119">None.</span></span> | <span data-ttu-id="c87f2-120">Для любого accessReviewInstanceDecisionItems, на который вызывается пользователь, на который назначен рецензент, вызывающий пользователь может записать решение, заплатив объект решения.</span><span class="sxs-lookup"><span data-stu-id="c87f2-120">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c87f2-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c87f2-121">Properties</span></span>
| <span data-ttu-id="c87f2-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c87f2-122">Property</span></span> | <span data-ttu-id="c87f2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c87f2-123">Type</span></span> |  <span data-ttu-id="c87f2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c87f2-124">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="c87f2-125">id</span><span class="sxs-lookup"><span data-stu-id="c87f2-125">id</span></span> | <span data-ttu-id="c87f2-126">String</span><span class="sxs-lookup"><span data-stu-id="c87f2-126">String</span></span> | <span data-ttu-id="c87f2-127">Идентификатор решения.</span><span class="sxs-lookup"><span data-stu-id="c87f2-127">The identifier of the decision.</span></span> |
| <span data-ttu-id="c87f2-128">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="c87f2-128">accessReviewId</span></span> | <span data-ttu-id="c87f2-129">String</span><span class="sxs-lookup"><span data-stu-id="c87f2-129">String</span></span> | <span data-ttu-id="c87f2-130">Идентификатор родителя accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="c87f2-130">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="c87f2-131">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="c87f2-131">reviewedBy</span></span> | [<span data-ttu-id="c87f2-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="c87f2-132">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="c87f2-133">Идентификатор рецензента.</span><span class="sxs-lookup"><span data-stu-id="c87f2-133">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="c87f2-134">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="c87f2-134">reviewedDateTime</span></span> | <span data-ttu-id="c87f2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c87f2-135">DateTimeOffset</span></span> | <span data-ttu-id="c87f2-136">Время, затмив время проверки.</span><span class="sxs-lookup"><span data-stu-id="c87f2-136">The timestamp when the review occurred.</span></span> |
| <span data-ttu-id="c87f2-137">решение</span><span class="sxs-lookup"><span data-stu-id="c87f2-137">decision</span></span> | <span data-ttu-id="c87f2-138">String</span><span class="sxs-lookup"><span data-stu-id="c87f2-138">String</span></span> | <span data-ttu-id="c87f2-139">Результат проверки.</span><span class="sxs-lookup"><span data-stu-id="c87f2-139">Result of the review.</span></span> <span data-ttu-id="c87f2-140">Возможные значения: `Approve` `Deny` , , или `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="c87f2-140">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="c87f2-141">обоснование</span><span class="sxs-lookup"><span data-stu-id="c87f2-141">justification</span></span> | <span data-ttu-id="c87f2-142">String</span><span class="sxs-lookup"><span data-stu-id="c87f2-142">String</span></span> | <span data-ttu-id="c87f2-143">Обоснование решения по пересмотру.</span><span class="sxs-lookup"><span data-stu-id="c87f2-143">The review decision justification.</span></span> |
| <span data-ttu-id="c87f2-144">appliedBy</span><span class="sxs-lookup"><span data-stu-id="c87f2-144">appliedBy</span></span> | [<span data-ttu-id="c87f2-145">userIdentity</span><span class="sxs-lookup"><span data-stu-id="c87f2-145">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="c87f2-146">Идентификатор пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="c87f2-146">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="c87f2-147">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="c87f2-147">appliedDateTime</span></span> | <span data-ttu-id="c87f2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c87f2-148">DateTimeOffset</span></span> | <span data-ttu-id="c87f2-149">Время, за которое было применено решение об утверждении.</span><span class="sxs-lookup"><span data-stu-id="c87f2-149">The timestamp when the approval decision was applied.</span></span> <span data-ttu-id="c87f2-150">Тип DatetimeOffset представляет сведения о дате и времени в формате ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="c87f2-150">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c87f2-151">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c87f2-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="c87f2-152">applyResult</span><span class="sxs-lookup"><span data-stu-id="c87f2-152">applyResult</span></span> | <span data-ttu-id="c87f2-153">String</span><span class="sxs-lookup"><span data-stu-id="c87f2-153">String</span></span> | <span data-ttu-id="c87f2-154">Результат применения решения.</span><span class="sxs-lookup"><span data-stu-id="c87f2-154">The result of applying the decision.</span></span> <span data-ttu-id="c87f2-155">Возможные значения: `NotApplied` , , , , или `Success` `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="c87f2-155">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="c87f2-156">рекомендация</span><span class="sxs-lookup"><span data-stu-id="c87f2-156">recommendation</span></span> | <span data-ttu-id="c87f2-157">String</span><span class="sxs-lookup"><span data-stu-id="c87f2-157">String</span></span> | <span data-ttu-id="c87f2-158">Сгенерированная системой рекомендация для принятия решения об утверждении.</span><span class="sxs-lookup"><span data-stu-id="c87f2-158">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="c87f2-159">Возможные значения: `Approve` `Deny` , или `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="c87f2-159">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="c87f2-160">target</span><span class="sxs-lookup"><span data-stu-id="c87f2-160">target</span></span> | [<span data-ttu-id="c87f2-161">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="c87f2-161">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="c87f2-162">Цель этого конкретного решения.</span><span class="sxs-lookup"><span data-stu-id="c87f2-162">The target of this specific decision.</span></span> <span data-ttu-id="c87f2-163">Целевые показатели принятия решений могут быть разных типов , каждый из которых имеет свои собственные свойства.</span><span class="sxs-lookup"><span data-stu-id="c87f2-163">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="c87f2-164">См. [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="c87f2-164">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |
|<span data-ttu-id="c87f2-165">основной</span><span class="sxs-lookup"><span data-stu-id="c87f2-165">principal</span></span>|[<span data-ttu-id="c87f2-166">identity</span><span class="sxs-lookup"><span data-stu-id="c87f2-166">identity</span></span>](../resources/identity.md)|<span data-ttu-id="c87f2-167">Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="c87f2-167">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="c87f2-168">Это свойство представляет сведения о принципе.</span><span class="sxs-lookup"><span data-stu-id="c87f2-168">This property represents details of the principal.</span></span> <span data-ttu-id="c87f2-169">Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным элементом является "Bob", а ресурсом является "Sales".</span><span class="sxs-lookup"><span data-stu-id="c87f2-169">For example, if a decision item represents access of User "Bob" to Group "Sales" - The principal is "Bob" and the resource is "Sales".</span></span> <span data-ttu-id="c87f2-170">Основные принципы могут быть двух типов : userIdentity и servicePrincipalIdentity.</span><span class="sxs-lookup"><span data-stu-id="c87f2-170">Principals can be of two types - userIdentity and servicePrincipalIdentity.</span></span>|
|<span data-ttu-id="c87f2-171">resource</span><span class="sxs-lookup"><span data-stu-id="c87f2-171">resource</span></span>|[<span data-ttu-id="c87f2-172">accessReviewInstanceDecisionItemResource</span><span class="sxs-lookup"><span data-stu-id="c87f2-172">accessReviewInstanceDecisionItemResource</span></span>](../resources/accessreviewinstancedecisionitemresource.md)|<span data-ttu-id="c87f2-173">Каждый элемент решения в обзоре доступа представляет доступ директора к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="c87f2-173">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="c87f2-174">Это свойство представляет сведения о ресурсе.</span><span class="sxs-lookup"><span data-stu-id="c87f2-174">This property represents details of the resource.</span></span> <span data-ttu-id="c87f2-175">Например, если элемент решения представляет доступ пользователя "Bob" к группе "Sales", то основным является Боб, а ресурсом является "Sales".</span><span class="sxs-lookup"><span data-stu-id="c87f2-175">For example, if a decision item represents access of User "Bob" to Group "Sales" - The principal is Bob and the resource is "Sales".</span></span> <span data-ttu-id="c87f2-176">Ресурсы могут быть нескольких типов.</span><span class="sxs-lookup"><span data-stu-id="c87f2-176">Resources can be of multiple types.</span></span> <span data-ttu-id="c87f2-177">См. [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)</span><span class="sxs-lookup"><span data-stu-id="c87f2-177">See [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c87f2-178">Связи</span><span class="sxs-lookup"><span data-stu-id="c87f2-178">Relationships</span></span>

| <span data-ttu-id="c87f2-179">Связь</span><span class="sxs-lookup"><span data-stu-id="c87f2-179">Relationship</span></span> | <span data-ttu-id="c87f2-180">Тип</span><span class="sxs-lookup"><span data-stu-id="c87f2-180">Type</span></span>   |<span data-ttu-id="c87f2-181">Описание</span><span class="sxs-lookup"><span data-stu-id="c87f2-181">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c87f2-182">экземпляр</span><span class="sxs-lookup"><span data-stu-id="c87f2-182">instance</span></span> |[<span data-ttu-id="c87f2-183">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="c87f2-183">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="c87f2-184">Существует точно один accessReviewInstance, связанный с каждым решением.</span><span class="sxs-lookup"><span data-stu-id="c87f2-184">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="c87f2-185">Экземпляр является родителем элемента решения, представляющего повторение проверки доступа, на которое принимается решение.</span><span class="sxs-lookup"><span data-stu-id="c87f2-185">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c87f2-186">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c87f2-186">JSON representation</span></span>

<span data-ttu-id="c87f2-187">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c87f2-187">Here is a JSON representation of the resource.</span></span>

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
  "id": "String (identifier)",
  "accessReviewId": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "reviewedDateTime": "String (timestamp)",
  "decision": "String",
  "justification": "String",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "String (timestamp)",
  "applyResult": "String",
  "recommendation": "String",
  "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  },
  "principal": {
    "@odata.type": "microsoft.graph.identity"
  },
  "resource": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
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
