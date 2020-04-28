---
title: Тип ресурса АкцессревиевдеЦисион
description: АкцессревиевдеЦисион представляет решение для проверки поправки Azure AD на доступ к определенному объекту.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f603ae8ae2c80f9f177d7469013ebde9148bb948
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472245"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="6cd40-103">Тип ресурса АкцессревиевдеЦисион</span><span class="sxs-lookup"><span data-stu-id="6cd40-103">accessReviewDecision resource type</span></span>

<span data-ttu-id="6cd40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cd40-105">В функции [рецензирования Access](accessreviews-root.md) в `accessReviewDecision` Azure AD — представляет решение для проверки доступа к определенному объекту в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6cd40-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="6cd40-106">При просмотре доступа или экземпляре повторяющейся проверки доступа существует один `accessReviewDecision` проверенный пользователь.</span><span class="sxs-lookup"><span data-stu-id="6cd40-106">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="6cd40-107">Например, если в группе есть два гостей и один не гость, а для этой группы выполняется проверка доступа для гостей, то будут доступны два объекта решения для проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="6cd40-107">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="6cd40-108">Если проверяющий изменяет свое решение или другой проверяющий переопределяет их, `accessReviewDecision` то обновляется.</span><span class="sxs-lookup"><span data-stu-id="6cd40-108">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="6cd40-109">Methods</span><span class="sxs-lookup"><span data-stu-id="6cd40-109">Methods</span></span>

<span data-ttu-id="6cd40-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="6cd40-110">None.</span></span>  <span data-ttu-id="6cd40-111">Объекты этого типа автоматически создаются компонентом при инициализации проверки доступа и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="6cd40-111">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="6cd40-112">Они могут извлекаться из проверки доступа с помощью связей " [решения](../api/accessreview-listdecisions.md) " и " [мидеЦисионс](../api/accessreview-listmydecisions.md) ".</span><span class="sxs-lookup"><span data-stu-id="6cd40-112">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="6cd40-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="6cd40-113">Properties</span></span>

<span data-ttu-id="6cd40-114">В этой таблице показаны основные свойства объектов этого типа.</span><span class="sxs-lookup"><span data-stu-id="6cd40-114">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="6cd40-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cd40-115">Property</span></span>                        | <span data-ttu-id="6cd40-116">Тип</span><span class="sxs-lookup"><span data-stu-id="6cd40-116">Type</span></span>                         | <span data-ttu-id="6cd40-117">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd40-117">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="6cd40-118">Идентификатор решения в рамках проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="6cd40-118">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="6cd40-119">Созданный компонентом идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="6cd40-119">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="6cd40-120">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6cd40-120">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="6cd40-121">Удостоверение проверяющего.</span><span class="sxs-lookup"><span data-stu-id="6cd40-121">The identity of the reviewer.</span></span> <span data-ttu-id="6cd40-122">Если в качестве проверки использовалась рекомендация, параметр userPrincipalName пуст.</span><span class="sxs-lookup"><span data-stu-id="6cd40-122">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="6cd40-123">Дата и время, когда было предоставлено Последнее рецензирование для этого права доступа.</span><span class="sxs-lookup"><span data-stu-id="6cd40-123">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="6cd40-124">Результат проверки, один `NotReviewed`из, `Deny` `DontKnow` или. `Approve`</span><span class="sxs-lookup"><span data-stu-id="6cd40-124">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="6cd40-125">Деловое обоснование проверяющего, если оно указано.</span><span class="sxs-lookup"><span data-stu-id="6cd40-125">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="6cd40-126">userIdentity</span><span class="sxs-lookup"><span data-stu-id="6cd40-126">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="6cd40-127">По завершении проверки, если результаты были вручную применены, удостоверение пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="6cd40-127">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="6cd40-128">Если Рецензирование было применено автоматически, значение userPrincipalName пусто.</span><span class="sxs-lookup"><span data-stu-id="6cd40-128">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="6cd40-129">Дата и время применения решения проверки.</span><span class="sxs-lookup"><span data-stu-id="6cd40-129">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="6cd40-130">Результат `NotApplied`применения решения, один из, `Success` `Failed`, `NotFound` или. `NotSupported`</span><span class="sxs-lookup"><span data-stu-id="6cd40-130">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="6cd40-131">Созданная с помощью функции рекомендация, показанная рецензенту, один из `Approve` `Deny` или `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="6cd40-131">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="6cd40-132">Кроме того, могут присутствовать дополнительные свойства в зависимости от типа объекта, которому назначен доступ.</span><span class="sxs-lookup"><span data-stu-id="6cd40-132">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="6cd40-133">Например, если решение "Проверка доступа" является участником группы определенного пользователя или доступом к приложениям, то пользователь, который может получить доступ к нему, будет удален с помощью следующих свойств:</span><span class="sxs-lookup"><span data-stu-id="6cd40-133">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="6cd40-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cd40-134">Property</span></span>                        | <span data-ttu-id="6cd40-135">Тип</span><span class="sxs-lookup"><span data-stu-id="6cd40-135">Type</span></span>                         | <span data-ttu-id="6cd40-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd40-136">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="6cd40-137">Идентификатор пользователя, доступ к которому был проверен.</span><span class="sxs-lookup"><span data-stu-id="6cd40-137">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="6cd40-138">Отображаемое имя пользователя, доступ к которому был проверен.</span><span class="sxs-lookup"><span data-stu-id="6cd40-138">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="6cd40-139">Имя участника пользователя, для которого был проверен доступ.</span><span class="sxs-lookup"><span data-stu-id="6cd40-139">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="6cd40-140">Связи</span><span class="sxs-lookup"><span data-stu-id="6cd40-140">Relationships</span></span>

<span data-ttu-id="6cd40-141">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6cd40-141">None.</span></span>  <span data-ttu-id="6cd40-142">Объекты этого типа можно получить из проверки доступа с помощью отношений [решений](../api/accessreview-listdecisions.md) и [МидеЦисионс](../api/accessreview-listmydecisions.md) в объекте [акцессревиев](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="6cd40-142">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="6cd40-143">См. также</span><span class="sxs-lookup"><span data-stu-id="6cd40-143">See also</span></span>

| <span data-ttu-id="6cd40-144">Метод</span><span class="sxs-lookup"><span data-stu-id="6cd40-144">Method</span></span>           | <span data-ttu-id="6cd40-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6cd40-145">Return Type</span></span>    |<span data-ttu-id="6cd40-146">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd40-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6cd40-147">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="6cd40-147">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="6cd40-148">Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="6cd40-148">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="6cd40-149">Получение решений для Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="6cd40-149">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="6cd40-150">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="6cd40-150">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="6cd40-151">Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="6cd40-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="6cd40-152">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="6cd40-152">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cd40-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6cd40-153">JSON representation</span></span>

<span data-ttu-id="6cd40-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cd40-154">Here is a JSON representation of the resource.</span></span>

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
