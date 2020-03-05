---
title: Тип ресурса АкцессревиевдеЦисион
description: В функции рецензирования Access в `accessReviewDecision` Azure AD — представляет решение для проверки доступа к определенному объекту в Azure AD.  При просмотре доступа или экземпляре повторяющейся проверки доступа существует один `accessReviewDecision` проверенный пользователь.  Например, если в группе есть два гостей и один не гость, а для этой группы выполняется проверка доступа для гостей, то будут доступны два объекта решения для проверки доступа.  Если проверяющий изменяет свое решение или другой проверяющий переопределяет их, `accessReviewDecision` то обновляется.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e92eb6b17b76ac3f8e44404dfbc776463170e0fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508480"
---
# <a name="accessreviewdecision-resource-type"></a><span data-ttu-id="5970d-106">Тип ресурса АкцессревиевдеЦисион</span><span class="sxs-lookup"><span data-stu-id="5970d-106">accessReviewDecision resource type</span></span>

<span data-ttu-id="5970d-107">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5970d-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5970d-108">В функции [рецензирования Access](accessreviews-root.md) в `accessReviewDecision` Azure AD — представляет решение для проверки доступа к определенному объекту в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5970d-108">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReviewDecision` represents an Azure AD access review decision of a particular entity's access.</span></span>  <span data-ttu-id="5970d-109">При просмотре доступа или экземпляре повторяющейся проверки доступа существует один `accessReviewDecision` проверенный пользователь.</span><span class="sxs-lookup"><span data-stu-id="5970d-109">Within an access review, or an instance of a recurring access review, there is one `accessReviewDecision` per reviewed user.</span></span>  <span data-ttu-id="5970d-110">Например, если в группе есть два гостей и один не гость, а для этой группы выполняется проверка доступа для гостей, то будут доступны два объекта решения для проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5970d-110">For example, if a group has two guests and one non-guest as members, and an access review of guests is performed for that group, then there will be two access review decision objects.</span></span>  <span data-ttu-id="5970d-111">Если проверяющий изменяет свое решение или другой проверяющий переопределяет их, `accessReviewDecision` то обновляется.</span><span class="sxs-lookup"><span data-stu-id="5970d-111">If a reviewer changes their decision, or another reviewer overrides them, then the `accessReviewDecision` is updated.</span></span>


## <a name="methods"></a><span data-ttu-id="5970d-112">Методы</span><span class="sxs-lookup"><span data-stu-id="5970d-112">Methods</span></span>

<span data-ttu-id="5970d-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="5970d-113">None.</span></span>  <span data-ttu-id="5970d-114">Объекты этого типа автоматически создаются компонентом при инициализации проверки доступа и не могут быть удалены.</span><span class="sxs-lookup"><span data-stu-id="5970d-114">Objects of this type are automatically created by the feature when an access review initializes, and cannot be deleted.</span></span>  <span data-ttu-id="5970d-115">Они могут извлекаться из проверки доступа с помощью связей " [решения](../api/accessreview-listdecisions.md) " и " [мидеЦисионс](../api/accessreview-listmydecisions.md) ".</span><span class="sxs-lookup"><span data-stu-id="5970d-115">They can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships.</span></span>

## <a name="properties"></a><span data-ttu-id="5970d-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5970d-116">Properties</span></span>

<span data-ttu-id="5970d-117">В этой таблице показаны основные свойства объектов этого типа.</span><span class="sxs-lookup"><span data-stu-id="5970d-117">This table illustrates the base properties of objects of this type.</span></span> 

| <span data-ttu-id="5970d-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5970d-118">Property</span></span>                        | <span data-ttu-id="5970d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5970d-119">Type</span></span>                         | <span data-ttu-id="5970d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5970d-120">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | <span data-ttu-id="5970d-121">Идентификатор решения в рамках проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5970d-121">The id of the decision within the access review.</span></span>                                                                                     |
| `accessReviewId`                |`String`                      | <span data-ttu-id="5970d-122">Созданный компонентом идентификатор проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="5970d-122">The feature-generated id of the access review.</span></span>                                                                                       |
| `reviewedBy`                    |[<span data-ttu-id="5970d-123">userIdentity</span><span class="sxs-lookup"><span data-stu-id="5970d-123">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="5970d-124">Удостоверение проверяющего.</span><span class="sxs-lookup"><span data-stu-id="5970d-124">The identity of the reviewer.</span></span> <span data-ttu-id="5970d-125">Если в качестве проверки использовалась рекомендация, параметр userPrincipalName пуст.</span><span class="sxs-lookup"><span data-stu-id="5970d-125">If the recommendation was used as the review, the userPrincipalName is empty.</span></span>                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | <span data-ttu-id="5970d-126">Дата и время, когда было предоставлено Последнее рецензирование для этого права доступа.</span><span class="sxs-lookup"><span data-stu-id="5970d-126">The date and time the most recent review for this access right was supplied.</span></span>                                                                         |
| `reviewResult`                  |`String`                      | <span data-ttu-id="5970d-127">Результат проверки, один `NotReviewed`из, `Deny` `DontKnow` или. `Approve`</span><span class="sxs-lookup"><span data-stu-id="5970d-127">The result of the review, one of `NotReviewed`, `Deny`, `DontKnow` or `Approve`.</span></span>                                                                                    |
| `justification`                 |`String`                      | <span data-ttu-id="5970d-128">Деловое обоснование проверяющего, если оно указано.</span><span class="sxs-lookup"><span data-stu-id="5970d-128">The reviewer's business justification, if supplied.</span></span>                                                                         |
| `appliedBy`                     |[<span data-ttu-id="5970d-129">userIdentity</span><span class="sxs-lookup"><span data-stu-id="5970d-129">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="5970d-130">По завершении проверки, если результаты были вручную применены, удостоверение пользователя, который применил решение.</span><span class="sxs-lookup"><span data-stu-id="5970d-130">When the review completes, if the results were manually applied, the user identity of the user who applied the decision.</span></span> <span data-ttu-id="5970d-131">Если Рецензирование было применено автоматически, значение userPrincipalName пусто.</span><span class="sxs-lookup"><span data-stu-id="5970d-131">If the review was auto-applied, the userPrincipalName is empty.</span></span>                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | <span data-ttu-id="5970d-132">Дата и время применения решения проверки.</span><span class="sxs-lookup"><span data-stu-id="5970d-132">The date and time when the review decision was applied.</span></span>                                                          |
| `applyResult`                   |`String`                      | <span data-ttu-id="5970d-133">Результат `NotApplied`применения решения, один из, `Success` `Failed`, `NotFound` или. `NotSupported`</span><span class="sxs-lookup"><span data-stu-id="5970d-133">The outcome of applying the decision, one of `NotApplied`, `Success`, `Failed`, `NotFound` or `NotSupported`.</span></span>                      |
| `accessRecommendation`          |`String`                      | <span data-ttu-id="5970d-134">Созданная с помощью функции рекомендация, показанная рецензенту, один из `Approve` `Deny` или `NotAvailable`.</span><span class="sxs-lookup"><span data-stu-id="5970d-134">The feature- generated recommendation shown to the reviewer, one of `Approve`, `Deny` or `NotAvailable`.</span></span> |


<span data-ttu-id="5970d-135">Кроме того, могут присутствовать дополнительные свойства в зависимости от типа объекта, которому назначен доступ.</span><span class="sxs-lookup"><span data-stu-id="5970d-135">In addition, additional properties may be present depending on the object type of the object possessing the access that was decided upon.</span></span>  <span data-ttu-id="5970d-136">Например, если решение "Проверка доступа" является участником группы определенного пользователя или доступом к приложениям, то пользователь, который может получить доступ к нему, будет удален с помощью следующих свойств:</span><span class="sxs-lookup"><span data-stu-id="5970d-136">For example, if the access review decision is a particular user's group membership or application access, the user who is potentially going to have their access be removed is identified through these properties:</span></span>

| <span data-ttu-id="5970d-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="5970d-137">Property</span></span>                        | <span data-ttu-id="5970d-138">Тип</span><span class="sxs-lookup"><span data-stu-id="5970d-138">Type</span></span>                         | <span data-ttu-id="5970d-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5970d-139">Description</span></span>                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | <span data-ttu-id="5970d-140">Идентификатор пользователя, доступ к которому был проверен.</span><span class="sxs-lookup"><span data-stu-id="5970d-140">The id of user whose access was reviewed.</span></span>                                                                                    |
| `userDisplayName`                            |`String`                      | <span data-ttu-id="5970d-141">Отображаемое имя пользователя, доступ к которому был проверен.</span><span class="sxs-lookup"><span data-stu-id="5970d-141">The display name of the user whose access was reviewed.</span></span>                                                                                     |
| `userPrincipalName`                            |`String`                      | <span data-ttu-id="5970d-142">Имя участника пользователя, для которого был проверен доступ.</span><span class="sxs-lookup"><span data-stu-id="5970d-142">The user principal name of the user whose access was reviewed.</span></span>                                                                                     |



## <a name="relationships"></a><span data-ttu-id="5970d-143">Связи</span><span class="sxs-lookup"><span data-stu-id="5970d-143">Relationships</span></span>

<span data-ttu-id="5970d-144">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5970d-144">None.</span></span>  <span data-ttu-id="5970d-145">Объекты этого типа можно получить из проверки доступа с помощью отношений [решений](../api/accessreview-listdecisions.md) и [МидеЦисионс](../api/accessreview-listmydecisions.md) в объекте [акцессревиев](accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="5970d-145">Objects of this type can be retrieved from an access review using the [decisions](../api/accessreview-listdecisions.md) and [mydecisions](../api/accessreview-listmydecisions.md) relationships of the [accessReview](accessreview.md) object.</span></span>

## <a name="see-also"></a><span data-ttu-id="5970d-146">См. также</span><span class="sxs-lookup"><span data-stu-id="5970d-146">See also</span></span>

| <span data-ttu-id="5970d-147">Метод</span><span class="sxs-lookup"><span data-stu-id="5970d-147">Method</span></span>           | <span data-ttu-id="5970d-148">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5970d-148">Return Type</span></span>    |<span data-ttu-id="5970d-149">Описание</span><span class="sxs-lookup"><span data-stu-id="5970d-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5970d-150">Список решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="5970d-150">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="5970d-151">Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="5970d-151">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="5970d-152">Получение решений для Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="5970d-152">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="5970d-153">Список моих решений Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="5970d-153">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="5970d-154">Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)</span><span class="sxs-lookup"><span data-stu-id="5970d-154">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="5970d-155">В качестве проверяющего получите мое решение Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="5970d-155">As a reviewer, get my decisions of an accessReview.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5970d-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5970d-156">JSON representation</span></span>

<span data-ttu-id="5970d-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5970d-157">Here is a JSON representation of the resource.</span></span>

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
