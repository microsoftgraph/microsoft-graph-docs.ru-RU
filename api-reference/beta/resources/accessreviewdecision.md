---
title: Тип ресурса accessReviewDecision
description: AccessReviewDecision представляет решение о проверке доступа Azure AD для доступа определенной сущности.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 52d4e2a262d3a90010cc0e254e11f2d723a5e550
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292695"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="fd87e-103">Тип ресурса accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="fd87e-103">accessReviewDecision resource type</span></span>

<span data-ttu-id="fd87e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd87e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="fd87e-105">В функции [проверки](accessreviews-root.md) доступа Azure AD эта функция представляет решение о проверке доступа Azure AD для доступа `accessReviewDecision` определенной сущности.</span><span class="sxs-lookup"><span data-stu-id="fd87e-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="fd87e-106">В рамках проверки доступа или экземпляра рецензии на повторяющийся доступ имеется один экземпляр для `accessReviewDecision` каждого проверяемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd87e-106">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="fd87e-107">Например, если группа состоит из двух гостей и одного не гостя в качестве участников, а для нее выполняется проверка доступа гостей, то будут два объекта принятия решений для проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="fd87e-107">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="fd87e-108">Если рецензент изменяет свое решение или другой рецензент переопределяет его, то `accessReviewDecision` обновляется.</span><span class="sxs-lookup"><span data-stu-id="fd87e-108">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="fd87e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="fd87e-109">Methods</span></span>

<span data-ttu-id="fd87e-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="fd87e-110">None.</span></span>  <span data-ttu-id="fd87e-111">Объекты этого типа автоматически создаются функцией при инициализации проверки доступа и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="fd87e-111">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="fd87e-112">Их можно получить из проверки доступа с помощью [решений](../api/accessreview-listdecisions.md) и [связей mydecisions.](../api/accessreview-listmydecisions.md)</span><span class="sxs-lookup"><span data-stu-id="fd87e-112">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="fd87e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd87e-113">Properties</span></span>

<span data-ttu-id="fd87e-114">В этой таблице иллюстрируют базовые свойства объектов этого типа.</span><span class="sxs-lookup"><span data-stu-id="fd87e-114">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="fd87e-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd87e-115">Property</span></span>                        | <span data-ttu-id="fd87e-116">Тип</span><span class="sxs-lookup"><span data-stu-id="fd87e-116">Type</span></span>                         | <span data-ttu-id="fd87e-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fd87e-117">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="fd87e-118">ИД решения в рамках проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="fd87e-118">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="fd87e-119">Созданный функцией ид проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="fd87e-119">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="fd87e-120">userIdentity</span><span class="sxs-lookup"><span data-stu-id="fd87e-120">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="fd87e-121">Удостоверение проверяющего.</span><span class="sxs-lookup"><span data-stu-id="fd87e-121">The identity of the reviewer.</span></span> <span data-ttu-id="fd87e-122">Если рекомендация использовалась в качестве отзыва, userPrincipalName пуст.</span><span class="sxs-lookup"><span data-stu-id="fd87e-122">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="fd87e-123">Дата и время последней проверки для этого права доступа.</span><span class="sxs-lookup"><span data-stu-id="fd87e-123">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="fd87e-124">Результат проверки, один из `NotReviewed` `Deny` , или `DontKnow` `Approve` .</span><span class="sxs-lookup"><span data-stu-id="fd87e-124">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="fd87e-125">Бизнес-обоснование проверяемой, если она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="fd87e-125">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="fd87e-126">userIdentity</span><span class="sxs-lookup"><span data-stu-id="fd87e-126">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="fd87e-127">После завершения проверки, если результаты были применены вручную, удостоверение пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="fd87e-127">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="fd87e-128">Если отзыв был применен автоматически, userPrincipalName пуст.</span><span class="sxs-lookup"><span data-stu-id="fd87e-128">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="fd87e-129">Дата и время принятия решения о проверке.</span><span class="sxs-lookup"><span data-stu-id="fd87e-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="fd87e-130">Результат применения решения, один из `NotApplied` `Success` , , или `Failed` `NotFound` `NotSupported` .</span><span class="sxs-lookup"><span data-stu-id="fd87e-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="fd87e-131">Рекомендация, сгенерированная функцией, показанная рецензенту, одна из или `Approve` `Deny` `NotAvailable` .</span><span class="sxs-lookup"><span data-stu-id="fd87e-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="fd87e-132">Кроме того, могут присутствовать дополнительные свойства в зависимости от типа объекта, обладания доступом, который был решен.</span><span class="sxs-lookup"><span data-stu-id="fd87e-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="fd87e-133">Например, если решением для проверки доступа является членство определенного пользователя в группе или доступ к приложению, пользователь, который потенциально собирается получить доступ, будет удален с помощью этих свойств:</span><span class="sxs-lookup"><span data-stu-id="fd87e-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="fd87e-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd87e-134">Property</span></span>                        | <span data-ttu-id="fd87e-135">Тип</span><span class="sxs-lookup"><span data-stu-id="fd87e-135">Type</span></span>                         | <span data-ttu-id="fd87e-136">Описание</span><span class="sxs-lookup"><span data-stu-id="fd87e-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="fd87e-137">ИД пользователя, доступ к которым был рассмотрен.</span><span class="sxs-lookup"><span data-stu-id="fd87e-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="fd87e-138">Отображаемого имени пользователя, доступ к которым был рассмотрен.</span><span class="sxs-lookup"><span data-stu-id="fd87e-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="fd87e-139">Имя пользователя, доступ к которым был рассмотрен.</span><span class="sxs-lookup"><span data-stu-id="fd87e-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="fd87e-140">Связи</span><span class="sxs-lookup"><span data-stu-id="fd87e-140">Relationships</span></span>

<span data-ttu-id="fd87e-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fd87e-141">None.</span></span>  <span data-ttu-id="fd87e-142">Объекты этого типа можно получить из проверки доступа с помощью решений и связей [mydecisions](../api/accessreview-listmydecisions.md) объекта [accessReview.](accessreview.md) [](../api/accessreview-listdecisions.md)</span><span class="sxs-lookup"><span data-stu-id="fd87e-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="fd87e-143">См. также</span><span class="sxs-lookup"><span data-stu-id="fd87e-143">See also</span></span>

| <span data-ttu-id="fd87e-144">Метод</span><span class="sxs-lookup"><span data-stu-id="fd87e-144">Method</span></span>           | <span data-ttu-id="fd87e-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fd87e-145">Return Type</span></span>    |<span data-ttu-id="fd87e-146">Описание</span><span class="sxs-lookup"><span data-stu-id="fd87e-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd87e-147">Список решений accessReview</span><span class="sxs-lookup"><span data-stu-id="fd87e-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="fd87e-148">[Коллекция accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="fd87e-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="fd87e-149">Получите решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="fd87e-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="fd87e-150">Список решений accessReview</span><span class="sxs-lookup"><span data-stu-id="fd87e-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="fd87e-151">[Коллекция accessReviewDecision](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="fd87e-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="fd87e-152">Как рецензент получите мои решения по accessReview.</span><span class="sxs-lookup"><span data-stu-id="fd87e-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd87e-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd87e-153">JSON representation</span></span>

<span data-ttu-id="fd87e-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd87e-154">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


