---
title: 'accessReviewInstance: resetDecisions'
description: Сбрасывает все объекты accessReviewInstanceDecisionItem на accessReviewInstance для `notReviewed` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cfe9e5c0fe7390a9c2204678b7a926ef225154cf
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031501"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="5c6c7-103">accessReviewInstance: resetDecisions</span><span class="sxs-lookup"><span data-stu-id="5c6c7-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="5c6c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c6c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c6c7-105">Сбрасывает решения всех [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) в [accessReviewInstance.](../resources/accessreviewinstance.md) `notReviewed`</span><span class="sxs-lookup"><span data-stu-id="5c6c7-105">Resets decisions of all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c6c7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c6c7-106">Permissions</span></span>
<span data-ttu-id="5c6c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c6c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c6c7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c6c7-109">Permission type</span></span>|<span data-ttu-id="5c6c7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c6c7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c6c7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c6c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c6c7-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6c7-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="5c6c7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c6c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c6c7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c6c7-114">Not supported.</span></span>|
|<span data-ttu-id="5c6c7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5c6c7-115">Application</span></span>|<span data-ttu-id="5c6c7-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6c7-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c6c7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c6c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="5c6c7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c6c7-118">Request headers</span></span>
|<span data-ttu-id="5c6c7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5c6c7-119">Name</span></span>|<span data-ttu-id="5c6c7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c6c7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c6c7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c6c7-121">Authorization</span></span>|<span data-ttu-id="5c6c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c6c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c6c7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c6c7-124">Request body</span></span>
<span data-ttu-id="5c6c7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c6c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c6c7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c6c7-126">Response</span></span>

<span data-ttu-id="5c6c7-127">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5c6c7-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5c6c7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5c6c7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c6c7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c6c7-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-44b5-ae36-41b923c3bf87/resetDecisions
```


### <a name="response"></a><span data-ttu-id="5c6c7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c6c7-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
