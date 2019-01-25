---
title: Тип ресурса accessReviewDecision
description: В Azure AD access дается обзор компонента, `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.  В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.  К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.  Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517402"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="1d9e5-106">Тип ресурса accessReviewDecision</span><span class="sxs-lookup"><span data-stu-id="1d9e5-106">accessReviewDecision resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d9e5-107">В компоненте [дается обзор доступа](accessreviews-root.md) Azure AD `accessReviewDecision` представляет Azure AD access review принятия решения об доступа к конкретной сущности.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="1d9e5-108">В рамках проверки доступа, или экземпляр повторяющейся проверки доступа, существует один `accessReviewDecision` на проверенные пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-108">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="1d9e5-109">К примеру Если группы имеет два Гости и один не гостевая-как члены и обзор доступа с гостевым выполняется для этой группы будет двух объектов решений проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-109">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="1d9e5-110">Если проверяющий изменяет их принятия решений или другой редактор переопределяет их, а затем `accessReviewDecision` обновляется.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-110">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="1d9e5-111">Методы</span><span class="sxs-lookup"><span data-stu-id="1d9e5-111">Methods</span></span>

<span data-ttu-id="1d9e5-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-112">None.</span></span>  <span data-ttu-id="1d9e5-113">Объекты данного типа автоматически создаются с помощью функции при доступе просмотрите инициализирует и не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-113">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="1d9e5-114">Они могут быть получены из проверки доступа с помощью [решения](../api/accessreview-listdecisions.md) и [mydecisions](../api/accessreview-listmydecisions.md) связи.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-114">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="1d9e5-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d9e5-115">Properties</span></span>

<span data-ttu-id="1d9e5-116">В данной таблице представлены основные свойства объектов этого типа.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-116">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="1d9e5-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d9e5-117">Property</span></span>                        | <span data-ttu-id="1d9e5-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1d9e5-118">Type</span></span>                         | <span data-ttu-id="1d9e5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1d9e5-119">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="1d9e5-120">Идентификатор решения в рамках проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-120">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="1d9e5-121">Идентификатор созданного компонента проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-121">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="1d9e5-122">удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="1d9e5-122">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="1d9e5-123">Удостоверение проверяющий.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-123">The identity of the reviewer.</span></span>                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="1d9e5-124">Дата и время последней проверки базы данных для доступа к справа было задано.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-124">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="1d9e5-125">Результат проверки.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-125">The result of the review.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="1d9e5-126">Деловое обоснование рецензента, если указано.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-126">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="1d9e5-127">удостоверению пользователя</span><span class="sxs-lookup"><span data-stu-id="1d9e5-127">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="1d9e5-128">После завершения проверки, если результаты были применены вручную, пользователь идентификатор пользователя, который применяется решение.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-128">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span>                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="1d9e5-129">Дата и время, когда была применена Обзор решения.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="1d9e5-130">Результат применения принятия решений, один из `NotApplied`, `Success`, `Failed`, `NotFound` или `NotSupported`.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="1d9e5-131">Рекомендация созданный компонент-показано проверяющему, один из `Approve`, `Deny` или `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="1d9e5-132">Кроме того в зависимости от типа объекта имеет доступ, которое было принято решение после объекта может присутствовать дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="1d9e5-133">Например если решение проверки доступа членство в группах конкретному пользователю или доступ к приложениям, пользователи, которые потенциально будут иметь доступ удалены идентифицируется через эти свойства:</span><span class="sxs-lookup"><span data-stu-id="1d9e5-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="1d9e5-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d9e5-134">Property</span></span>                        | <span data-ttu-id="1d9e5-135">Тип</span><span class="sxs-lookup"><span data-stu-id="1d9e5-135">Type</span></span>                         | <span data-ttu-id="1d9e5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="1d9e5-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="1d9e5-137">Идентификатор пользователя, которого доступа прошел проверку.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="1d9e5-138">Отображаемое имя пользователя, которого доступа прошел проверку.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="1d9e5-139">Имя пользователя участника пользователя, которого доступа прошел проверку.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="1d9e5-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="1d9e5-140">Relationships</span></span>

<span data-ttu-id="1d9e5-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-141">None.</span></span>  <span data-ttu-id="1d9e5-142">Объекты данного типа можно извлечь из проверки доступа с помощью [решения](../api/accessreview-listdecisions.md) и [mydecisions](../api/accessreview-listmydecisions.md) связи объекта [accessReview](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="1d9e5-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="1d9e5-143">См. также</span><span class="sxs-lookup"><span data-stu-id="1d9e5-143">See also</span></span>

| <span data-ttu-id="1d9e5-144">Метод</span><span class="sxs-lookup"><span data-stu-id="1d9e5-144">Method</span></span>           | <span data-ttu-id="1d9e5-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d9e5-145">Return Type</span></span>    |<span data-ttu-id="1d9e5-146">Описание</span><span class="sxs-lookup"><span data-stu-id="1d9e5-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d9e5-147">Список accessReview решения</span><span class="sxs-lookup"><span data-stu-id="1d9e5-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="1d9e5-148">[accessReviewDecision](accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1d9e5-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="1d9e5-149">Получите решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="1d9e5-150">Мои accessReview решения</span><span class="sxs-lookup"><span data-stu-id="1d9e5-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="1d9e5-151">[accessReviewDecision](accessreviewdecision.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1d9e5-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="1d9e5-152">В качестве читателя получите Мои решения accessReview.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d9e5-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d9e5-153">JSON representation</span></span>

<span data-ttu-id="1d9e5-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d9e5-154">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
