---
title: 'accessReviewInstance: acceptRecommendations'
description: 'Позволяет принимать рекомендации по всем решениям, которые не были рассмотрены для экземпляра проверки доступа, для которого вызываемого пользователя является рецензентом. '
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b955bc637c3f536ca5cb8a3e24ad65990296ab2e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030756"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="0742f-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="0742f-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="0742f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0742f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0742f-105">Позволяет принимать рекомендации по всем объектам [accessReviewInstanceDecisionItem,](../resources/accessreviewinstancedecisionitem.md) которые не были рассмотрены для объекта [accessReviewInstance,](../resources/accessreviewinstance.md) для которого вызываемого пользователя является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="0742f-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed for an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span> <span data-ttu-id="0742f-106">Рекомендации, если **рекомендацииEnabled** находятся `true` на [объекте accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0742f-106">Recommendations are generated if **recommendationsEnabled** is `true` on the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span> <span data-ttu-id="0742f-107">Если рекомендации по объекту [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) нет, решение не будет записано.</span><span class="sxs-lookup"><span data-stu-id="0742f-107">If there is not a recommendation on an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object no decision will be recorded.</span></span>

## <a name="permissions"></a><span data-ttu-id="0742f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0742f-108">Permissions</span></span>
<span data-ttu-id="0742f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0742f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0742f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0742f-111">Permission type</span></span>                        | <span data-ttu-id="0742f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0742f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0742f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0742f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0742f-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0742f-114">AccessReview.ReadWrite.All</span></span> |
| <span data-ttu-id="0742f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0742f-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0742f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0742f-116">Not supported.</span></span> |

<span data-ttu-id="0742f-117">В accessReviewInstance пользователь должен также быть рецензентом.</span><span class="sxs-lookup"><span data-stu-id="0742f-117">The signed-in user must also be a reviewer on the accessReviewInstance.</span></span>

## <a name="http-request"></a><span data-ttu-id="0742f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0742f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/pendingAccessReviewInstances/{instance-id}/acceptRecommendations
```
## <a name="request-headers"></a><span data-ttu-id="0742f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0742f-119">Request headers</span></span>
<span data-ttu-id="0742f-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="0742f-120">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="0742f-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0742f-121">Request body</span></span>
<span data-ttu-id="0742f-122">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0742f-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0742f-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="0742f-123">Response</span></span>
<span data-ttu-id="0742f-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0742f-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0742f-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="0742f-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="0742f-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="0742f-127">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0742f-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="0742f-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "acceptrecommendations_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="0742f-129">C#</span><span class="sxs-lookup"><span data-stu-id="0742f-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/acceptrecommendations-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0742f-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0742f-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/acceptrecommendations-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0742f-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0742f-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/acceptrecommendations-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0742f-132">Java</span><span class="sxs-lookup"><span data-stu-id="0742f-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/acceptrecommendations-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0742f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0742f-133">Response</span></span>
><span data-ttu-id="0742f-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0742f-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
