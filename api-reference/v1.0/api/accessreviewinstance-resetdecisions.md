---
title: 'accessReviewInstance: resetDecisions'
description: Сбрасывает все объекты accessReviewInstanceDecisionItem на accessReviewInstance для `notReviewed` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 269c3f4891fb62d9191991ffa50dc70635268020
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209768"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="d4b5d-103">accessReviewInstance: resetDecisions</span><span class="sxs-lookup"><span data-stu-id="d4b5d-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="d4b5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4b5d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4b5d-105">Сбрасывает [все объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) на [accessReviewInstance](../resources/accessreviewinstance.md) для `notReviewed` .</span><span class="sxs-lookup"><span data-stu-id="d4b5d-105">Resets all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4b5d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4b5d-106">Permissions</span></span>
<span data-ttu-id="d4b5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4b5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4b5d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4b5d-109">Permission type</span></span>|<span data-ttu-id="d4b5d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4b5d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4b5d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4b5d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4b5d-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4b5d-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d4b5d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4b5d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4b5d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4b5d-114">Not supported.</span></span>|
|<span data-ttu-id="d4b5d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4b5d-115">Application</span></span>|<span data-ttu-id="d4b5d-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4b5d-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4b5d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4b5d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="d4b5d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4b5d-118">Request headers</span></span>
|<span data-ttu-id="d4b5d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d4b5d-119">Name</span></span>|<span data-ttu-id="d4b5d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4b5d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4b5d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4b5d-121">Authorization</span></span>|<span data-ttu-id="d4b5d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4b5d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4b5d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4b5d-124">Request body</span></span>
<span data-ttu-id="d4b5d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4b5d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4b5d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4b5d-126">Response</span></span>

<span data-ttu-id="d4b5d-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d4b5d-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d4b5d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4b5d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4b5d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4b5d-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d4b5d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4b5d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="d4b5d-131">C#</span><span class="sxs-lookup"><span data-stu-id="d4b5d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-resetdecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4b5d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4b5d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-resetdecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4b5d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4b5d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-resetdecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4b5d-134">Java</span><span class="sxs-lookup"><span data-stu-id="d4b5d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-resetdecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d4b5d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4b5d-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
