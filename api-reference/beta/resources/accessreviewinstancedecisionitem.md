---
title: Тип ресурса АкцессревиевинстанцедеЦисионитем
description: Представляет решение для доступа пользователя в Акцессревиевинстанце.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9ad5f8a49d44c82f1a43a1666f08f2b49853395
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001067"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="1daef-103">Тип ресурса АкцессревиевинстанцедеЦисионитем</span><span class="sxs-lookup"><span data-stu-id="1daef-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="1daef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1daef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1daef-105">Представляет решение по [проверке доступа](accessreviewsv2-root.md) Azure AD для экземпляра проверки.</span><span class="sxs-lookup"><span data-stu-id="1daef-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="1daef-106">Это решение представляет определение доступа пользователя или субъекта к данному [экземпляру проверки доступа](accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="1daef-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1daef-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1daef-107">Methods</span></span>

| <span data-ttu-id="1daef-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1daef-108">Method</span></span> | <span data-ttu-id="1daef-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1daef-109">Return Type</span></span> | <span data-ttu-id="1daef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1daef-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="1daef-111">Список АкцессревиевинстанцедеЦисионитемс</span><span class="sxs-lookup"><span data-stu-id="1daef-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="1daef-112">Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="1daef-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="1daef-113">Перечисление всех АкцессревиевинстанцедеЦисионитем для определенного Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="1daef-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="1daef-114">Список ожидающих утверждения АкцессревиевинстанцедеЦисионитемс</span><span class="sxs-lookup"><span data-stu-id="1daef-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="1daef-115">Коллекция [акцессревиевинстанцедеЦисионитем](accessreviewinstancedecisionitem.md) .</span><span class="sxs-lookup"><span data-stu-id="1daef-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="1daef-116">Получение всех АкцессревиевинстанцедеЦисионитемс, назначенных вызывающему пользователю для определенного Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="1daef-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="1daef-117">Обновление АкцессревиевинстанцедеЦисионитем</span><span class="sxs-lookup"><span data-stu-id="1daef-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="1daef-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="1daef-118">None.</span></span> | <span data-ttu-id="1daef-119">Для всех АкцессревиевинстанцедеЦисионитемс, для которых вызывающему пользователю назначен проверяющий, вызывающий пользователь может записать решение, заменив исправление объекта принятия решений.</span><span class="sxs-lookup"><span data-stu-id="1daef-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1daef-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="1daef-120">Properties</span></span>
| <span data-ttu-id="1daef-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="1daef-121">Property</span></span> | <span data-ttu-id="1daef-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1daef-122">Type</span></span> |  <span data-ttu-id="1daef-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1daef-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="1daef-124">id</span><span class="sxs-lookup"><span data-stu-id="1daef-124">id</span></span> | <span data-ttu-id="1daef-125">Строка</span><span class="sxs-lookup"><span data-stu-id="1daef-125">String</span></span> | <span data-ttu-id="1daef-126">Идентификатор решения.</span><span class="sxs-lookup"><span data-stu-id="1daef-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="1daef-127">акцессревиевид</span><span class="sxs-lookup"><span data-stu-id="1daef-127">accessReviewId</span></span> | <span data-ttu-id="1daef-128">Строка</span><span class="sxs-lookup"><span data-stu-id="1daef-128">String</span></span> | <span data-ttu-id="1daef-129">Идентификатор родителя Акцессревиевинстанце.</span><span class="sxs-lookup"><span data-stu-id="1daef-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="1daef-130">ревиеведби</span><span class="sxs-lookup"><span data-stu-id="1daef-130">reviewedBy</span></span> | [<span data-ttu-id="1daef-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1daef-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="1daef-132">Идентификатор проверяющего.</span><span class="sxs-lookup"><span data-stu-id="1daef-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="1daef-133">ревиеведдатетиме</span><span class="sxs-lookup"><span data-stu-id="1daef-133">reviewedDateTime</span></span> | <span data-ttu-id="1daef-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1daef-134">DateTimeOffset</span></span> | <span data-ttu-id="1daef-135">Дата и время, когда произошла проверка.</span><span class="sxs-lookup"><span data-stu-id="1daef-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="1daef-136">решении</span><span class="sxs-lookup"><span data-stu-id="1daef-136">decision</span></span> | <span data-ttu-id="1daef-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1daef-137">String</span></span> | <span data-ttu-id="1daef-138">Результат проверки.</span><span class="sxs-lookup"><span data-stu-id="1daef-138">Result of the review.</span></span> <span data-ttu-id="1daef-139">Возможные значения: `Approve` , `Deny` , `NotReviewed` , или `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="1daef-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="1daef-140">текста</span><span class="sxs-lookup"><span data-stu-id="1daef-140">justification</span></span> | <span data-ttu-id="1daef-141">Строка</span><span class="sxs-lookup"><span data-stu-id="1daef-141">String</span></span> | <span data-ttu-id="1daef-142">Проверка обоснования решения.</span><span class="sxs-lookup"><span data-stu-id="1daef-142">The review decision justification.</span></span> |
| <span data-ttu-id="1daef-143">апплиедби</span><span class="sxs-lookup"><span data-stu-id="1daef-143">appliedBy</span></span> | [<span data-ttu-id="1daef-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1daef-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="1daef-145">Идентификатор пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="1daef-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="1daef-146">апплиеддатетиме</span><span class="sxs-lookup"><span data-stu-id="1daef-146">appliedDateTime</span></span> | <span data-ttu-id="1daef-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1daef-147">DateTimeOffset</span></span> | <span data-ttu-id="1daef-148">Дата и время, когда было применено решение об утверждении.</span><span class="sxs-lookup"><span data-stu-id="1daef-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="1daef-149">апплиресулт</span><span class="sxs-lookup"><span data-stu-id="1daef-149">applyResult</span></span> | <span data-ttu-id="1daef-150">Строка</span><span class="sxs-lookup"><span data-stu-id="1daef-150">String</span></span> | <span data-ttu-id="1daef-151">Результат применения решения.</span><span class="sxs-lookup"><span data-stu-id="1daef-151">The result of applying the decision.</span></span> <span data-ttu-id="1daef-152">Возможные значения: `NotApplied` , `Success` , `Failed` , `NotFound` , или `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="1daef-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="1daef-153">Рекомендуемые</span><span class="sxs-lookup"><span data-stu-id="1daef-153">recommendation</span></span> | <span data-ttu-id="1daef-154">Строка</span><span class="sxs-lookup"><span data-stu-id="1daef-154">String</span></span> | <span data-ttu-id="1daef-155">Созданная системой рекомендация для решения об утверждении.</span><span class="sxs-lookup"><span data-stu-id="1daef-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="1daef-156">Возможные значения: `Approve` , `Deny` , или `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="1daef-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="1daef-157">target</span><span class="sxs-lookup"><span data-stu-id="1daef-157">target</span></span> | [<span data-ttu-id="1daef-158">акцессревиевинстанцедеЦисионитемтаржет</span><span class="sxs-lookup"><span data-stu-id="1daef-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="1daef-159">Цель этого конкретного решения.</span><span class="sxs-lookup"><span data-stu-id="1daef-159">The target of this specific decision.</span></span> <span data-ttu-id="1daef-160">Целевые показатели решений могут принадлежать разным типам — каждый из них имеет собственные конкретные свойства.</span><span class="sxs-lookup"><span data-stu-id="1daef-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="1daef-161">Обратитесь к разделу [акцессревиевинстанцедеЦисионитемтаржет](accessreviewinstancedecisionitemtarget.md).</span><span class="sxs-lookup"><span data-stu-id="1daef-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1daef-162">Связи</span><span class="sxs-lookup"><span data-stu-id="1daef-162">Relationships</span></span>

| <span data-ttu-id="1daef-163">Связь</span><span class="sxs-lookup"><span data-stu-id="1daef-163">Relationship</span></span> | <span data-ttu-id="1daef-164">Тип</span><span class="sxs-lookup"><span data-stu-id="1daef-164">Type</span></span>   |<span data-ttu-id="1daef-165">Описание</span><span class="sxs-lookup"><span data-stu-id="1daef-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1daef-166">вхождения</span><span class="sxs-lookup"><span data-stu-id="1daef-166">instance</span></span> |[<span data-ttu-id="1daef-167">акцессревиевинстанце</span><span class="sxs-lookup"><span data-stu-id="1daef-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="1daef-168">Каждое решение имеет только один Акцессревиевинстанце, связанный с каждым из них.</span><span class="sxs-lookup"><span data-stu-id="1daef-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="1daef-169">Экземпляр является родительским элементом решения, представляющим повторение проверки доступа, над которой принимается решение.</span><span class="sxs-lookup"><span data-stu-id="1daef-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1daef-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1daef-170">JSON representation</span></span>

<span data-ttu-id="1daef-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1daef-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "",
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
