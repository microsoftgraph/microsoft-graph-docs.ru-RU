---
title: 'accessReviewInstance: batchRecordDecisions'
description: Позволяет рецензентам просмотреть все accessReviewInstanceDecisionItems пакетами.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ea22d510bb70ab8d7047f952f7b4c0e265d57197
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031333"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="a4f39-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="a4f39-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="a4f39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4f39-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4f39-105">Позволяет рецензентам просмотреть все [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) пакетами с помощью **principalId,** **resourceId** или ни того, ни другго.</span><span class="sxs-lookup"><span data-stu-id="a4f39-105">Enables reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using **principalId**, **resourceId**, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4f39-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f39-106">Permissions</span></span>
<span data-ttu-id="a4f39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4f39-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f39-109">Permission type</span></span>|<span data-ttu-id="a4f39-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4f39-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4f39-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4f39-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4f39-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f39-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="a4f39-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4f39-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4f39-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a4f39-114">Not supported</span></span>|
|<span data-ttu-id="a4f39-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4f39-115">Application</span></span>|<span data-ttu-id="a4f39-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f39-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4f39-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4f39-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="a4f39-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4f39-118">Request headers</span></span>
|<span data-ttu-id="a4f39-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a4f39-119">Name</span></span>|<span data-ttu-id="a4f39-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f39-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4f39-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4f39-121">Authorization</span></span>|<span data-ttu-id="a4f39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f39-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a4f39-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4f39-124">Content-Type</span></span>|<span data-ttu-id="a4f39-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f39-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4f39-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4f39-127">Request body</span></span>
<span data-ttu-id="a4f39-128">В теле запроса подарите JSON представление [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span><span class="sxs-lookup"><span data-stu-id="a4f39-128">In the request body, supply a JSON representation of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="a4f39-129">В следующей таблице перечислены свойства, которые можно использовать для просмотра [объектов accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="a4f39-129">The following table lists the properties that you can use to review [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

|<span data-ttu-id="a4f39-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="a4f39-130">Parameter</span></span>|<span data-ttu-id="a4f39-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a4f39-131">Type</span></span>|<span data-ttu-id="a4f39-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f39-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4f39-133">решение</span><span class="sxs-lookup"><span data-stu-id="a4f39-133">decision</span></span>|<span data-ttu-id="a4f39-134">String</span><span class="sxs-lookup"><span data-stu-id="a4f39-134">String</span></span>|<span data-ttu-id="a4f39-135">Решение о доступе для проверяемого объекта.</span><span class="sxs-lookup"><span data-stu-id="a4f39-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="a4f39-136">Возможные значения: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="a4f39-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="a4f39-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f39-137">Required.</span></span>|
|<span data-ttu-id="a4f39-138">обоснование</span><span class="sxs-lookup"><span data-stu-id="a4f39-138">justification</span></span>|<span data-ttu-id="a4f39-139">String</span><span class="sxs-lookup"><span data-stu-id="a4f39-139">String</span></span>|<span data-ttu-id="a4f39-140">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="a4f39-140">Context of the review provided to admins.</span></span> <span data-ttu-id="a4f39-141">Требуется, **если обоснованиеRequiredOnApproval** свойства параметров **accessReviewScheduleDefinition** является `true` .</span><span class="sxs-lookup"><span data-stu-id="a4f39-141">Required if **justificationRequiredOnApproval** of the settings property of the **accessReviewScheduleDefinition** is `true` .</span></span>|
|<span data-ttu-id="a4f39-142">principalId</span><span class="sxs-lookup"><span data-stu-id="a4f39-142">principalId</span></span>|<span data-ttu-id="a4f39-143">String</span><span class="sxs-lookup"><span data-stu-id="a4f39-143">String</span></span>|<span data-ttu-id="a4f39-144">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **значениям principalId.**</span><span class="sxs-lookup"><span data-stu-id="a4f39-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** values will be reviewed in this batch.</span></span> <span data-ttu-id="a4f39-145">Если они не будут предоставлены, **все accessReviewInstanceDecisionItems** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="a4f39-145">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|
|<span data-ttu-id="a4f39-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="a4f39-146">resourceId</span></span>|<span data-ttu-id="a4f39-147">String</span><span class="sxs-lookup"><span data-stu-id="a4f39-147">String</span></span>|<span data-ttu-id="a4f39-148">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **resourceId.**</span><span class="sxs-lookup"><span data-stu-id="a4f39-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="a4f39-149">Если они не будут предоставлены, **все accessReviewInstanceDecisionItems** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="a4f39-149">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|

## <a name="response"></a><span data-ttu-id="a4f39-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4f39-150">Response</span></span>

<span data-ttu-id="a4f39-151">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a4f39-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a4f39-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4f39-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4f39-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4f39-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-6778-8868-9999c7f4cc06/batchRecordDecisions
Content-type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```

### <a name="response"></a><span data-ttu-id="a4f39-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f39-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
