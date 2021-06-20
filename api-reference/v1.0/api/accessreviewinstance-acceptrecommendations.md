---
title: 'accessReviewInstance: acceptRecommendations'
description: Позволяет принимать рекомендации по решениям для экземпляра проверки доступа, который не был рассмотрен пользователем, который является рецензентом.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 60a9e59579f094e2c517c33ee96276220062599b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031352"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="1cff2-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="1cff2-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="1cff2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cff2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1cff2-105">Позволяет принимать рекомендации по всем [объектам accessReviewInstanceDecisionItem,](../resources/accessreviewinstancedecisionitem.md) которые не были рассмотрены на [объекте accessReviewInstance,](../resources/accessreviewinstance.md) для которого вызываемого пользователя является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="1cff2-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed on an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cff2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1cff2-106">Permissions</span></span>
<span data-ttu-id="1cff2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cff2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cff2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cff2-109">Permission type</span></span>|<span data-ttu-id="1cff2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cff2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cff2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cff2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1cff2-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cff2-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="1cff2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cff2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cff2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cff2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cff2-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cff2-115">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/acceptRecommendations
```

## <a name="request-headers"></a><span data-ttu-id="1cff2-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cff2-116">Request headers</span></span>
|<span data-ttu-id="1cff2-117">Имя</span><span class="sxs-lookup"><span data-stu-id="1cff2-117">Name</span></span>|<span data-ttu-id="1cff2-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1cff2-118">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1cff2-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cff2-119">Authorization</span></span>|<span data-ttu-id="1cff2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cff2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cff2-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cff2-122">Request body</span></span>
<span data-ttu-id="1cff2-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1cff2-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cff2-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cff2-124">Response</span></span>

<span data-ttu-id="1cff2-125">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1cff2-125">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1cff2-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="1cff2-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cff2-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cff2-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_acceptrecommendations"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f91006/acceptRecommendations
```


### <a name="response"></a><span data-ttu-id="1cff2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cff2-128">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
