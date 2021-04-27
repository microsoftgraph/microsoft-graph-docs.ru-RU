---
title: 'accessReviewInstance: acceptRecommendations'
description: 'Позволяет принимать рекомендации по всем не рассмотренным решениям в экземпляре проверки доступа, на который они являются рецензентом. '
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2e9505a0cf7e3b0e52d54c45ed7d85ee4e09651e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048437"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="908a0-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="908a0-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="908a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="908a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="908a0-105">Позволяет принимать рекомендации для всех не рассмотренных [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) на [accessReviewInstance,](../resources/accessreviewinstance.md) на который они являются рецензентом.</span><span class="sxs-lookup"><span data-stu-id="908a0-105">Allows the acceptance of recommendations on all not reviewed [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) on an [accessReviewInstance](../resources/accessreviewinstance.md) that they are the reviewer on.</span></span>

## <a name="permissions"></a><span data-ttu-id="908a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="908a0-106">Permissions</span></span>
<span data-ttu-id="908a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="908a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="908a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="908a0-109">Permission type</span></span>                        | <span data-ttu-id="908a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="908a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="908a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="908a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="908a0-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="908a0-112">AccessReview.ReadWrite.All</span></span> |
| <span data-ttu-id="908a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="908a0-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="908a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="908a0-114">Not supported.</span></span> |

<span data-ttu-id="908a0-115">В accessReviewInstance пользователь должен также быть рецензентом.</span><span class="sxs-lookup"><span data-stu-id="908a0-115">The signed-in user must also be a reviewer on the accessReviewInstance.</span></span>

## <a name="http-request"></a><span data-ttu-id="908a0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="908a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/pendingAccessReviewInstances/{instance-id}/acceptRecommendations
```
## <a name="request-headers"></a><span data-ttu-id="908a0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="908a0-117">Request headers</span></span>
<span data-ttu-id="908a0-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="908a0-118">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="908a0-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="908a0-119">Request body</span></span>
<span data-ttu-id="908a0-120">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="908a0-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="908a0-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="908a0-121">Response</span></span>
<span data-ttu-id="908a0-p102">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="908a0-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="908a0-124">Примеры</span><span class="sxs-lookup"><span data-stu-id="908a0-124">Examples</span></span>
### <a name="request"></a><span data-ttu-id="908a0-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="908a0-125">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="908a0-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="908a0-126">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "acceptrecommendations_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="908a0-127">C#</span><span class="sxs-lookup"><span data-stu-id="908a0-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/acceptrecommendations-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="908a0-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="908a0-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/acceptrecommendations-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="908a0-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="908a0-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/acceptrecommendations-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="908a0-130">Java</span><span class="sxs-lookup"><span data-stu-id="908a0-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/acceptrecommendations-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="908a0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="908a0-131">Response</span></span>
><span data-ttu-id="908a0-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="908a0-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Accept recommendations accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
