---
title: Сброс accessReview
description: В функции обзоров доступа Azure AD сброшены решения действующего в настоящее время accessReview.  Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.  Предыдущие решения больше не записываются, но рецензенты могут продолжать обновлять решения.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ee7c54ef785c53489e9512b52b8ed0789a0e59a0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048479"
---
# <a name="reset-accessreview"></a><span data-ttu-id="8c07e-105">Сброс accessReview</span><span class="sxs-lookup"><span data-stu-id="8c07e-105">Reset accessReview</span></span>

<span data-ttu-id="8c07e-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c07e-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c07e-107">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) сброшены решения активного в настоящее время [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="8c07e-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="8c07e-108">Целевой объект может быть либо одноразовой проверкой доступа, либо экземпляром повторного обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="8c07e-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="8c07e-109">Предыдущие решения больше не записываются, но рецензенты могут продолжать обновлять решения.</span><span class="sxs-lookup"><span data-stu-id="8c07e-109">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c07e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c07e-110">Permissions</span></span>
<span data-ttu-id="8c07e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c07e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c07e-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c07e-113">Permission type</span></span>                        | <span data-ttu-id="8c07e-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c07e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c07e-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c07e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c07e-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c07e-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="8c07e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c07e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c07e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c07e-118">Not supported.</span></span> |
|<span data-ttu-id="8c07e-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c07e-119">Application</span></span>                            | <span data-ttu-id="8c07e-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="8c07e-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c07e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c07e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/resetDecisions
```
## <a name="request-headers"></a><span data-ttu-id="8c07e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c07e-122">Request headers</span></span>
| <span data-ttu-id="8c07e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="8c07e-123">Name</span></span>         | <span data-ttu-id="8c07e-124">Тип</span><span class="sxs-lookup"><span data-stu-id="8c07e-124">Type</span></span>        | <span data-ttu-id="8c07e-125">Описание</span><span class="sxs-lookup"><span data-stu-id="8c07e-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8c07e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c07e-126">Authorization</span></span> | <span data-ttu-id="8c07e-127">string</span><span class="sxs-lookup"><span data-stu-id="8c07e-127">string</span></span> | <span data-ttu-id="8c07e-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c07e-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c07e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c07e-130">Request body</span></span>
<span data-ttu-id="8c07e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c07e-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8c07e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c07e-132">Response</span></span>
<span data-ttu-id="8c07e-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c07e-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c07e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8c07e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c07e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c07e-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8c07e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c07e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="8c07e-138">C#</span><span class="sxs-lookup"><span data-stu-id="8c07e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c07e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c07e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c07e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c07e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c07e-141">Java</span><span class="sxs-lookup"><span data-stu-id="8c07e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c07e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c07e-142">Response</span></span>
><span data-ttu-id="8c07e-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c07e-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


