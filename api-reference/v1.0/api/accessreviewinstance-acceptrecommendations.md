---
title: 'accessReviewInstance: acceptRecommendations'
description: Позволяет принимать рекомендации по решениям для экземпляра проверки доступа, который не был рассмотрен пользователем, который является рецензентом.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d8548340af184f703e89fcfd8aeda469d81cb566
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208168"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="807f0-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="807f0-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="807f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="807f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="807f0-105">Позволяет принимать рекомендации по всем [объектам accessReviewInstanceDecisionItem,](../resources/accessreviewinstancedecisionitem.md) которые не были рассмотрены на [объекте accessReviewInstance,](../resources/accessreviewinstance.md) для которого вызываемого пользователя является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="807f0-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed on an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="807f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="807f0-106">Permissions</span></span>
<span data-ttu-id="807f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="807f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="807f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="807f0-109">Permission type</span></span>|<span data-ttu-id="807f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="807f0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="807f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="807f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="807f0-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="807f0-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="807f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="807f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="807f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="807f0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="807f0-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="807f0-115">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/acceptRecommendations
```

## <a name="request-headers"></a><span data-ttu-id="807f0-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="807f0-116">Request headers</span></span>
|<span data-ttu-id="807f0-117">Имя</span><span class="sxs-lookup"><span data-stu-id="807f0-117">Name</span></span>|<span data-ttu-id="807f0-118">Описание</span><span class="sxs-lookup"><span data-stu-id="807f0-118">Description</span></span>|
|:---|:---|
|<span data-ttu-id="807f0-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="807f0-119">Authorization</span></span>|<span data-ttu-id="807f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="807f0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="807f0-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="807f0-122">Request body</span></span>
<span data-ttu-id="807f0-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="807f0-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="807f0-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="807f0-124">Response</span></span>

<span data-ttu-id="807f0-125">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="807f0-125">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="807f0-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="807f0-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="807f0-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="807f0-127">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="807f0-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="807f0-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_acceptrecommendations"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f91006/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="807f0-129">C#</span><span class="sxs-lookup"><span data-stu-id="807f0-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-acceptrecommendations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="807f0-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="807f0-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-acceptrecommendations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="807f0-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="807f0-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-acceptrecommendations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="807f0-132">Java</span><span class="sxs-lookup"><span data-stu-id="807f0-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-acceptrecommendations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="807f0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="807f0-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
