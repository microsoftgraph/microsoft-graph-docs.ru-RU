---
title: Тип ресурса accessReviewDecision
description: В Azure AD access дается обзор компонента, `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.  В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.  К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.  Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b6b10a53726e12c37a598f8df735a3f70174c807
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977558"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="9e3cf-106">Тип ресурса accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="9e3cf-106">accessReviewDecision resource type</span></span>

> <span data-ttu-id="9e3cf-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e3cf-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e3cf-109">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-109">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="9e3cf-110">В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-110">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="9e3cf-111">К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-111">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="9e3cf-112">Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-112">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="9e3cf-113">Methods</span><span class="sxs-lookup"><span data-stu-id="9e3cf-113">Methods</span></span>

<span data-ttu-id="9e3cf-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-114">None.</span></span>  <span data-ttu-id="9e3cf-115">Объекты данного типа автоматически создаются с помощью функции при доступе просмотрите инициализирует и не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-115">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="9e3cf-116">Они могут быть получены из проверки доступа с помощью [решения](../api/accessreview-listdecisions.md) и [mydecisions](../api/accessreview-listmydecisions.md) связи.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-116">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="9e3cf-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e3cf-117">Properties</span></span>

<span data-ttu-id="9e3cf-118">В данной таблице представлены основные свойства объектов этого типа.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-118">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="9e3cf-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e3cf-119">Property</span></span>                        | <span data-ttu-id="9e3cf-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9e3cf-120">Type</span></span>                         | <span data-ttu-id="9e3cf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9e3cf-121">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="9e3cf-122">Идентификатор решения в рамках проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-122">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="9e3cf-123">Идентификатор созданного компонента проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-123">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="9e3cf-124">удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="9e3cf-124">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="9e3cf-125">Удостоверение проверяющий.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-125">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="9e3cf-126">Дата и время последней проверки базы данных для доступа к справа было задано.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="9e3cf-127">Результат проверки.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-127">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="9e3cf-128">Деловое обоснование рецензента, если указано.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="9e3cf-129">удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="9e3cf-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="9e3cf-130">После завершения проверки, если результаты были применены вручную, пользователь идентификатор пользователя, который применяется решение.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="9e3cf-131">Дата и время, когда была применена Обзор решения.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-131">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="9e3cf-132">Результат применения принятия решений, один из `NotApplied`, `Success`, `Failed`, `NotFound` или `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-132">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="9e3cf-133">Рекомендация созданный компонент-показано проверяющему, один из `Approve`, `Deny` или `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-133">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="9e3cf-134">Кроме того в зависимости от типа объекта имеет доступ, которое было принято решение после объекта может присутствовать дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-134">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="9e3cf-135">Например если решение проверки доступа членство в группах конкретному пользователю или доступ к приложениям, пользователи, которые потенциально будут иметь доступ удалены идентифицируется через эти свойства:</span><span class="sxs-lookup"><span data-stu-id="9e3cf-135">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="9e3cf-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e3cf-136">Property</span></span>                        | <span data-ttu-id="9e3cf-137">Тип</span><span class="sxs-lookup"><span data-stu-id="9e3cf-137">Type</span></span>                         | <span data-ttu-id="9e3cf-138">Описание</span><span class="sxs-lookup"><span data-stu-id="9e3cf-138">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="9e3cf-139">Идентификатор пользователя, которого доступа прошел проверку.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-139">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="9e3cf-140">Отображаемое имя пользователя, которого доступа прошел проверку.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-140">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="9e3cf-141">Имя пользователя участника пользователя, которого доступа прошел проверку.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-141">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="9e3cf-142">Связи</span><span class="sxs-lookup"><span data-stu-id="9e3cf-142">Relationships</span></span>

<span data-ttu-id="9e3cf-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-143">None.</span></span>  <span data-ttu-id="9e3cf-144">Объекты данного типа можно извлечь из проверки доступа с помощью [решения](../api/accessreview-listdecisions.md) и [mydecisions](../api/accessreview-listmydecisions.md) связи объекта [accessReview](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="9e3cf-144">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="9e3cf-145">См. также</span><span class="sxs-lookup"><span data-stu-id="9e3cf-145">See also</span></span>

| <span data-ttu-id="9e3cf-146">Метод</span><span class="sxs-lookup"><span data-stu-id="9e3cf-146">Method</span></span>           | <span data-ttu-id="9e3cf-147">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e3cf-147">Return Type</span></span>    |<span data-ttu-id="9e3cf-148">Описание</span><span class="sxs-lookup"><span data-stu-id="9e3cf-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e3cf-149">Список accessReview решения</span><span class="sxs-lookup"><span data-stu-id="9e3cf-149">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="9e3cf-150">[accessReviewDecision](accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9e3cf-150">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="9e3cf-151">Получите решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-151">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="9e3cf-152">Мои accessReview решения</span><span class="sxs-lookup"><span data-stu-id="9e3cf-152">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="9e3cf-153">[accessReviewDecision](accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9e3cf-153">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="9e3cf-154">В качестве читателя получите Мои решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-154">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e3cf-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e3cf-155">JSON representation</span></span>

<span data-ttu-id="9e3cf-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e3cf-156">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
