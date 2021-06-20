---
title: 'accessReviewInstance: applyDecisions'
description: Применение решений для accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 93cc4d2e4f5c42ebe47bed00caf227779b579df2
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030333"
---
# <a name="accessreviewinstance-applydecisions"></a><span data-ttu-id="6135f-103">accessReviewInstance: applyDecisions</span><span class="sxs-lookup"><span data-stu-id="6135f-103">accessReviewInstance: applyDecisions</span></span>
<span data-ttu-id="6135f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6135f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6135f-105">Применение решений о проверке к ресурсу, рассмотренном в [accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="6135f-105">Apply review decisions to the resource reviewed in an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

<span data-ttu-id="6135f-106">Решения применяются автоматически, если **параметр autoApplyDecisionsEnabled** параметра [параметров accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) является  `true` .</span><span class="sxs-lookup"><span data-stu-id="6135f-106">Decisions are applied automatically if the **autoApplyDecisionsEnabled** of the **settings** parameter of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>

## <a name="permissions"></a><span data-ttu-id="6135f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6135f-107">Permissions</span></span>
<span data-ttu-id="6135f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6135f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6135f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6135f-110">Permission type</span></span>|<span data-ttu-id="6135f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6135f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6135f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6135f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6135f-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6135f-113">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="6135f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6135f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6135f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6135f-115">Not supported.</span></span>|
|<span data-ttu-id="6135f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6135f-116">Application</span></span>|<span data-ttu-id="6135f-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6135f-117">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6135f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6135f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/applyDecisions
```

## <a name="request-headers"></a><span data-ttu-id="6135f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6135f-119">Request headers</span></span>
|<span data-ttu-id="6135f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6135f-120">Name</span></span>|<span data-ttu-id="6135f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6135f-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6135f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6135f-122">Authorization</span></span>|<span data-ttu-id="6135f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6135f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6135f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6135f-125">Request body</span></span>
<span data-ttu-id="6135f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6135f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6135f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6135f-127">Response</span></span>

<span data-ttu-id="6135f-128">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6135f-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6135f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="6135f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6135f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6135f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_applydecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f49101/applyDecisions
```


### <a name="response"></a><span data-ttu-id="6135f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="6135f-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
