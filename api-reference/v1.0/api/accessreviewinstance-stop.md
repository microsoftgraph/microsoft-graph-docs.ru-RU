---
title: 'accessReviewInstance: остановка'
description: Остановите активный в настоящее время accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e119d3c914a793bfc083722fb329bd18a72b46df
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031292"
---
# <a name="accessreviewinstance-stop"></a><span data-ttu-id="e7f76-103">accessReviewInstance: остановка</span><span class="sxs-lookup"><span data-stu-id="e7f76-103">accessReviewInstance: stop</span></span>
<span data-ttu-id="e7f76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7f76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7f76-105">Остановите активный в настоящее [время accessReviewInstance.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="e7f76-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="e7f76-106">После остановки экземпляра проверки доступа состояние экземпляра помечено как , рецензенты больше не могут вводить ввод и применяются `Completed` решения о проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="e7f76-106">After the access review instance stops, the instance status is marked as `Completed`, the reviewers can no longer give input, and the access review decisions are applied.</span></span>

<span data-ttu-id="e7f76-107">Остановка экземпляра не остановит будущие экземпляры.</span><span class="sxs-lookup"><span data-stu-id="e7f76-107">Stopping an instance will not stop future instances.</span></span> <span data-ttu-id="e7f76-108">Чтобы предотвратить повторный обзор доступа при [](accessreviewscheduledefinition-update.md) запуске будущих экземпляров, обнови определение расписания, чтобы изменить запланированную дату окончания.</span><span class="sxs-lookup"><span data-stu-id="e7f76-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7f76-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7f76-109">Permissions</span></span>
<span data-ttu-id="e7f76-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7f76-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7f76-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7f76-112">Permission type</span></span>|<span data-ttu-id="e7f76-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7f76-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7f76-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7f76-114">Delegated (work or school account)</span></span>|<span data-ttu-id="e7f76-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7f76-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="e7f76-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7f76-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7f76-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7f76-117">Not supported.</span></span>|
|<span data-ttu-id="e7f76-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7f76-118">Application</span></span>|<span data-ttu-id="e7f76-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7f76-119">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7f76-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7f76-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stop
```

## <a name="request-headers"></a><span data-ttu-id="e7f76-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7f76-121">Request headers</span></span>
|<span data-ttu-id="e7f76-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e7f76-122">Name</span></span>|<span data-ttu-id="e7f76-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e7f76-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e7f76-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e7f76-124">Authorization</span></span>|<span data-ttu-id="e7f76-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7f76-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7f76-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e7f76-127">Request body</span></span>
<span data-ttu-id="e7f76-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e7f76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7f76-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7f76-129">Response</span></span>

<span data-ttu-id="e7f76-130">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e7f76-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="e7f76-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e7f76-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e7f76-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7f76-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_stop"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/stop
```


### <a name="response"></a><span data-ttu-id="e7f76-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7f76-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
