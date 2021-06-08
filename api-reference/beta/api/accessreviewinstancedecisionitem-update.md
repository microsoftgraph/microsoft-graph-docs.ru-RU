---
title: Обновление accessReviewInstanceDecisionItem
description: Обновление существующего объекта accessReviewInstanceDecisionItem, вызываемого пользователем, является рецензентом.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8fb69b4088fe0366f19e076fb069a8d57826ae18
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786638"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="4350c-103">Обновление accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="4350c-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="4350c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4350c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4350c-105">Обновите решения о доступе, известные как [accessReviewInstanceDecisionItems,](../resources/accessreviewinstancedecisionitem.md)для которых пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="4350c-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="4350c-106">Любые обновления, сделанные в **accessReviewInstanceDecisionItem,** могут быть сделаны только путем вызова пользователей, которые указаны в качестве рецензента для родительского [accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="4350c-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4350c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4350c-107">Permissions</span></span>
<span data-ttu-id="4350c-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="4350c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4350c-109">Делегирование разрешений личным учетным записям Майкрософт не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4350c-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="4350c-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4350c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4350c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4350c-111">Permission type</span></span>                        | <span data-ttu-id="4350c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4350c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4350c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4350c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="4350c-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4350c-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4350c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4350c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4350c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4350c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4350c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4350c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="4350c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4350c-118">Request headers</span></span>
| <span data-ttu-id="4350c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4350c-119">Name</span></span>         | <span data-ttu-id="4350c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4350c-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="4350c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4350c-121">Authorization</span></span>|<span data-ttu-id="4350c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4350c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4350c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4350c-124">Content-type</span></span> | <span data-ttu-id="4350c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4350c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4350c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4350c-127">Request body</span></span>
<span data-ttu-id="4350c-128">В следующей таблице показаны свойства, принятые для обновления `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="4350c-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="4350c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4350c-129">Property</span></span>     | <span data-ttu-id="4350c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4350c-130">Type</span></span>       | <span data-ttu-id="4350c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4350c-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4350c-132">решение</span><span class="sxs-lookup"><span data-stu-id="4350c-132">decision</span></span>  | <span data-ttu-id="4350c-133">String</span><span class="sxs-lookup"><span data-stu-id="4350c-133">String</span></span> | <span data-ttu-id="4350c-134">Решение о доступе для проверяемого объекта.</span><span class="sxs-lookup"><span data-stu-id="4350c-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="4350c-135">Возможные значения: `Approve` `Deny` `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="4350c-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="4350c-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4350c-136">Required.</span></span>  |
|  <span data-ttu-id="4350c-137">обоснование</span><span class="sxs-lookup"><span data-stu-id="4350c-137">justification</span></span> | <span data-ttu-id="4350c-138">String</span><span class="sxs-lookup"><span data-stu-id="4350c-138">String</span></span> | <span data-ttu-id="4350c-139">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="4350c-139">Context of the review provided to admins.</span></span> <span data-ttu-id="4350c-140">Обязательно, если оправданиеRequiredOnApproval является true на accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="4350c-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="4350c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4350c-141">Response</span></span>
<span data-ttu-id="4350c-142">В случае успешной работы этот метод возвращает код `204, NoContent` ответа и не возвращает текст ответа.</span><span class="sxs-lookup"><span data-stu-id="4350c-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="4350c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4350c-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="4350c-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="4350c-144">Examples</span></span>

<span data-ttu-id="4350c-145">Это пример утверждения доступа для пользователя, представленного пользователем `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="4350c-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>



# <a name="http"></a>[<span data-ttu-id="4350c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4350c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/12348410-67f3-4d4c-b946-6989e050be19
Content-Type: application/json
Content-length: 730

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```
# <a name="c"></a>[<span data-ttu-id="4350c-147">C#</span><span class="sxs-lookup"><span data-stu-id="4350c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4350c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4350c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4350c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4350c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4350c-150">Java</span><span class="sxs-lookup"><span data-stu-id="4350c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="4350c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4350c-151">Response</span></span>
><span data-ttu-id="4350c-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4350c-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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
