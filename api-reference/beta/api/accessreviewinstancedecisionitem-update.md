---
title: Обновление АкцессревиевинстанцедеЦисионитем
description: Обновление существующего объекта АкцессревиевинстанцедеЦисионитем, для которого вызывающий пользователь является проверяющим.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f14ed26169c659354af16963e03e449f246421c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214387"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="ae283-103">Обновление АкцессревиевинстанцедеЦисионитем</span><span class="sxs-lookup"><span data-stu-id="ae283-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="ae283-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae283-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae283-105">Обновление решений Access, известных как [акцессревиевинстанцедеЦисионитемс](../resources/accessreviewinstancedecisionitem.md), для которых пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="ae283-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="ae283-106">Любые изменения, внесенные в **акцессревиевинстанцедеЦисионитем** , могут выполняться только вызываемыми пользователями, указанными в качестве проверяющего для родительского [акцессревиевинстанце](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="ae283-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ae283-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae283-107">Permissions</span></span>
<span data-ttu-id="ae283-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="ae283-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ae283-109">Делегированные разрешения для личных учетных записей Майкрософт не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="ae283-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="ae283-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae283-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae283-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae283-111">Permission type</span></span>                        | <span data-ttu-id="ae283-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae283-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae283-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae283-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae283-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae283-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="ae283-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae283-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae283-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae283-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae283-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae283-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="ae283-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae283-118">Request headers</span></span>
| <span data-ttu-id="ae283-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ae283-119">Name</span></span>         | <span data-ttu-id="ae283-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae283-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="ae283-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae283-121">Authorization</span></span>|<span data-ttu-id="ae283-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae283-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ae283-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ae283-124">Content-type</span></span> | <span data-ttu-id="ae283-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae283-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae283-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae283-127">Request body</span></span>
<span data-ttu-id="ae283-128">В следующей таблице приведены свойства, принятые для обновления `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="ae283-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="ae283-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae283-129">Property</span></span>     | <span data-ttu-id="ae283-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ae283-130">Type</span></span>       | <span data-ttu-id="ae283-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ae283-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ae283-132">решении</span><span class="sxs-lookup"><span data-stu-id="ae283-132">decision</span></span>  | <span data-ttu-id="ae283-133">String</span><span class="sxs-lookup"><span data-stu-id="ae283-133">String</span></span> | <span data-ttu-id="ae283-134">Решение о доступе к проверяемой сущности.</span><span class="sxs-lookup"><span data-stu-id="ae283-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="ae283-135">Возможные значения: `Approve` `Deny` `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="ae283-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="ae283-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae283-136">Required.</span></span>  |
|  <span data-ttu-id="ae283-137">текста</span><span class="sxs-lookup"><span data-stu-id="ae283-137">justification</span></span> | <span data-ttu-id="ae283-138">String</span><span class="sxs-lookup"><span data-stu-id="ae283-138">String</span></span> | <span data-ttu-id="ae283-139">Контекст проверки, предоставленной администраторам.</span><span class="sxs-lookup"><span data-stu-id="ae283-139">Context of the review provided to admins.</span></span> <span data-ttu-id="ae283-140">Является обязательным, если Жустификатионрекуиредонаппровал имеет значение true для Акцессревиевсчедуледефинитион.</span><span class="sxs-lookup"><span data-stu-id="ae283-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="ae283-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae283-141">Response</span></span>
<span data-ttu-id="ae283-142">В случае успешного выполнения этот метод возвращает `204, NoContent` код отклика и без текста отклика.</span><span class="sxs-lookup"><span data-stu-id="ae283-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="ae283-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae283-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="ae283-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae283-144">Examples</span></span>

<span data-ttu-id="ae283-145">Это пример утверждающего доступа для пользователя, представленного в `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="ae283-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae283-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae283-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
}
```
# <a name="c"></a>[<span data-ttu-id="ae283-147">C#</span><span class="sxs-lookup"><span data-stu-id="ae283-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae283-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae283-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae283-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae283-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae283-150">Java</span><span class="sxs-lookup"><span data-stu-id="ae283-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="ae283-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae283-151">Response</span></span>
><span data-ttu-id="ae283-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae283-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
