---
title: 'accessReviewInstance: sendReminder'
description: Отправляет напоминание рецензентам активного доступаReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 00608ba03cbf3106b9707fc0e236328f2dfd1e65
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210965"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="dae51-103">accessReviewInstance: sendReminder</span><span class="sxs-lookup"><span data-stu-id="dae51-103">accessReviewInstance: sendReminder</span></span>
<span data-ttu-id="dae51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dae51-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dae51-105">Отправьте напоминание рецензентам активного [accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="dae51-105">Send a reminder to the reviewers of an active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dae51-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dae51-106">Permissions</span></span>
<span data-ttu-id="dae51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dae51-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dae51-109">Permission type</span></span>|<span data-ttu-id="dae51-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dae51-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dae51-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dae51-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dae51-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae51-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="dae51-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dae51-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dae51-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dae51-114">Not supported.</span></span>|
|<span data-ttu-id="dae51-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dae51-115">Application</span></span>|<span data-ttu-id="dae51-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae51-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dae51-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dae51-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/sendReminder
```

## <a name="request-headers"></a><span data-ttu-id="dae51-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dae51-118">Request headers</span></span>
|<span data-ttu-id="dae51-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dae51-119">Name</span></span>|<span data-ttu-id="dae51-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dae51-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dae51-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dae51-121">Authorization</span></span>|<span data-ttu-id="dae51-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dae51-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dae51-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dae51-124">Request body</span></span>
<span data-ttu-id="dae51-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dae51-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dae51-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="dae51-126">Response</span></span>

<span data-ttu-id="dae51-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dae51-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dae51-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="dae51-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dae51-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="dae51-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dae51-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dae51-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_sendreminder"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="dae51-131">C#</span><span class="sxs-lookup"><span data-stu-id="dae51-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-sendreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dae51-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dae51-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-sendreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dae51-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dae51-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-sendreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dae51-134">Java</span><span class="sxs-lookup"><span data-stu-id="dae51-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-sendreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dae51-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="dae51-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
