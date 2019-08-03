---
title: Сброс Акцессревиев
description: В средстве проверки доступа Azure AD выполните сброс решений текущего активного Акцессревиев.  Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.  Предыдущие решения не записываются, но проверяющие могут продолжать обновлять решения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c8828daf4243ea7bc51a9492944e7fb0a0ed0bd2
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172746"
---
# <a name="reset-accessreview"></a><span data-ttu-id="821c8-105">Сброс Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="821c8-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="821c8-106">В средстве проверки [доступа](../resources/accessreviews-root.md) Azure AD выполните сброс решений текущего активного [акцессревиев](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="821c8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="821c8-107">Целевой объект может быть либо одноразовой проверкой доступом, либо экземпляром повторяющейся проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="821c8-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="821c8-108">Предыдущие решения не записываются, но проверяющие могут продолжать обновлять решения.</span><span class="sxs-lookup"><span data-stu-id="821c8-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="821c8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="821c8-109">Permissions</span></span>
<span data-ttu-id="821c8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="821c8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="821c8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="821c8-112">Permission type</span></span>                        | <span data-ttu-id="821c8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="821c8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="821c8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="821c8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="821c8-115">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="821c8-115">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="821c8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="821c8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="821c8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="821c8-117">Not supported.</span></span> |
|<span data-ttu-id="821c8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="821c8-118">Application</span></span>                            | <span data-ttu-id="821c8-119">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="821c8-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="821c8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="821c8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="821c8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="821c8-121">Request headers</span></span>
| <span data-ttu-id="821c8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="821c8-122">Name</span></span>         | <span data-ttu-id="821c8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="821c8-123">Type</span></span>        | <span data-ttu-id="821c8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="821c8-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="821c8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="821c8-125">Authorization</span></span> | <span data-ttu-id="821c8-126">string</span><span class="sxs-lookup"><span data-stu-id="821c8-126">string</span></span> | <span data-ttu-id="821c8-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="821c8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="821c8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="821c8-129">Request body</span></span>
<span data-ttu-id="821c8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="821c8-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="821c8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="821c8-131">Response</span></span>
<span data-ttu-id="821c8-p105">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="821c8-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="821c8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="821c8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="821c8-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="821c8-135">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="821c8-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="821c8-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/resetDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="821c8-137">C#</span><span class="sxs-lookup"><span data-stu-id="821c8-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reset-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="821c8-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="821c8-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reset-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="821c8-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="821c8-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reset-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="821c8-140">Java</span><span class="sxs-lookup"><span data-stu-id="821c8-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reset-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="821c8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="821c8-141">Response</span></span>
><span data-ttu-id="821c8-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="821c8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
