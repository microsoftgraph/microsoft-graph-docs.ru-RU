---
title: Удаление рецензента accessReview
description: Удаление рецензента обзоров доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6f08fcd2b7b913de9dbe8d44f07f99d646f41560
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751038"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="80e40-103">Удаление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="80e40-103">Remove accessReview reviewer</span></span>

<span data-ttu-id="80e40-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80e40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80e40-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) обновите существующий объект [accessReview,](../resources/accessreview.md) чтобы удалить пользователя в качестве рецензента.</span><span class="sxs-lookup"><span data-stu-id="80e40-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="80e40-106">Эта операция разрешена только для еще не завершенного обзора доступа и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="80e40-106">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="80e40-107">Эта операция не разрешается для проверки доступа, в которой пользователи рассматривают собственный доступ, и не предназначена для проверки доступа, в которой владельцы групп назначены в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="80e40-107">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="80e40-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80e40-108">Permissions</span></span>
<span data-ttu-id="80e40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80e40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80e40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80e40-111">Permission type</span></span>                        | <span data-ttu-id="80e40-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80e40-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="80e40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80e40-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="80e40-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80e40-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="80e40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80e40-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80e40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80e40-116">Not supported.</span></span> |
|<span data-ttu-id="80e40-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="80e40-117">Application</span></span>                            | <span data-ttu-id="80e40-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="80e40-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="80e40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80e40-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="80e40-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80e40-120">Request headers</span></span>
| <span data-ttu-id="80e40-121">Имя</span><span class="sxs-lookup"><span data-stu-id="80e40-121">Name</span></span>         | <span data-ttu-id="80e40-122">Тип</span><span class="sxs-lookup"><span data-stu-id="80e40-122">Type</span></span>        | <span data-ttu-id="80e40-123">Описание</span><span class="sxs-lookup"><span data-stu-id="80e40-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="80e40-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="80e40-124">Authorization</span></span> | <span data-ttu-id="80e40-125">string</span><span class="sxs-lookup"><span data-stu-id="80e40-125">string</span></span> | <span data-ttu-id="80e40-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80e40-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80e40-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80e40-128">Request body</span></span>
<span data-ttu-id="80e40-129">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="80e40-129">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="80e40-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="80e40-130">Response</span></span>
<span data-ttu-id="80e40-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80e40-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80e40-132">Пример</span><span class="sxs-lookup"><span data-stu-id="80e40-132">Example</span></span>

<span data-ttu-id="80e40-133">Это пример обновления разового (не повторяемого) обзора доступа, чтобы удалить ненужный рецензент.</span><span class="sxs-lookup"><span data-stu-id="80e40-133">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="80e40-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="80e40-134">Request</span></span>
<span data-ttu-id="80e40-135">В URL-адрес запроса поставляют id объекта accessReview, а затем id объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="80e40-135">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="80e40-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="80e40-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="80e40-137">C#</span><span class="sxs-lookup"><span data-stu-id="80e40-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80e40-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80e40-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80e40-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80e40-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80e40-140">Java</span><span class="sxs-lookup"><span data-stu-id="80e40-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80e40-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="80e40-141">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


