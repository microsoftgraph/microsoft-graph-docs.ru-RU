---
title: Добавление рецензента accessReview
description: 'В функции обзоров доступа Azure AD обновим существующий объект accessReview, чтобы добавить другого пользователя в качестве рецензента.  Эта операция разрешена только для еще не завершенного обзора доступа и только для проверки доступа, в которой явно указаны рецензенты. Эта операция не разрешается для проверки доступа, в которой пользователи рассматривают собственный доступ, и не предназначена для проверки доступа, в которой владельцы групп назначены в качестве рецензентов. '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 86ea5525745933e40121a2906cd4a90fdb7f3179
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439452"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="d86f1-105">Добавление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="d86f1-105">Add accessReview reviewer</span></span>

<span data-ttu-id="d86f1-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d86f1-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d86f1-107">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) обновим существующий [объект accessReview,](../resources/accessreview.md) чтобы добавить другого пользователя в качестве рецензента.</span><span class="sxs-lookup"><span data-stu-id="d86f1-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="d86f1-108">Эта операция разрешена только для еще не завершенного обзора доступа и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="d86f1-108">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="d86f1-109">Эта операция не разрешается для проверки доступа, в которой пользователи рассматривают собственный доступ, и не предназначена для проверки доступа, в которой владельцы групп назначены в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="d86f1-109">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d86f1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d86f1-110">Permissions</span></span>
<span data-ttu-id="d86f1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d86f1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d86f1-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d86f1-113">Permission type</span></span>                        | <span data-ttu-id="d86f1-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d86f1-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d86f1-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d86f1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="d86f1-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d86f1-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d86f1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d86f1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d86f1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86f1-118">Not supported.</span></span> |
|<span data-ttu-id="d86f1-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="d86f1-119">Application</span></span>                            | <span data-ttu-id="d86f1-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="d86f1-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="d86f1-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d86f1-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="d86f1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d86f1-122">Request headers</span></span>
| <span data-ttu-id="d86f1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d86f1-123">Name</span></span>         | <span data-ttu-id="d86f1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d86f1-124">Type</span></span>        | <span data-ttu-id="d86f1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d86f1-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d86f1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d86f1-126">Authorization</span></span> | <span data-ttu-id="d86f1-127">string</span><span class="sxs-lookup"><span data-stu-id="d86f1-127">string</span></span> | <span data-ttu-id="d86f1-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d86f1-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d86f1-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d86f1-130">Request body</span></span>
<span data-ttu-id="d86f1-131">В теле запроса укажи JSON представление ID пользователя, который будет рецензентом.</span><span class="sxs-lookup"><span data-stu-id="d86f1-131">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="d86f1-132">В следующей таблице показаны свойства, которые можно получить при обновлении accessReview.</span><span class="sxs-lookup"><span data-stu-id="d86f1-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="d86f1-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="d86f1-133">Property</span></span>     | <span data-ttu-id="d86f1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="d86f1-134">Type</span></span>        | <span data-ttu-id="d86f1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="d86f1-135">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="d86f1-136">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="d86f1-136">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="d86f1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d86f1-137">Response</span></span>
<span data-ttu-id="d86f1-138">В случае успешной работы этот метод возвращает `201, Created` код ответа.</span><span class="sxs-lookup"><span data-stu-id="d86f1-138">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="d86f1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d86f1-139">Example</span></span>

<span data-ttu-id="d86f1-140">Это пример обновления разового (не повторяемого) обзора доступа с помощью дополнительного рецензента.</span><span class="sxs-lookup"><span data-stu-id="d86f1-140">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="d86f1-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d86f1-141">Request</span></span>
<span data-ttu-id="d86f1-142">В теле запроса укажи JSON представление id объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="d86f1-142">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="d86f1-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d86f1-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
Content-Type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```
# <a name="c"></a>[<span data-ttu-id="d86f1-144">C#</span><span class="sxs-lookup"><span data-stu-id="d86f1-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d86f1-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d86f1-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d86f1-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d86f1-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d86f1-147">Java</span><span class="sxs-lookup"><span data-stu-id="d86f1-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d86f1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d86f1-148">Response</span></span>
><span data-ttu-id="d86f1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d86f1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


