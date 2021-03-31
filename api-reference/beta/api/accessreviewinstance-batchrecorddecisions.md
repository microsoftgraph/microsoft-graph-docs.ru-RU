---
title: 'accessReviewInstance: batchRecordDecisions'
description: Emable reviewers to review all accessReviewInstanceDecisionItems in batches.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e9573dabd24b414b55fc4ec961999c43896fc687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469753"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="ac5fe-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="ac5fe-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="ac5fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac5fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac5fe-105">Включить рецензенты для просмотра всех [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) пакетами с помощью `principalId` , или ни `resourceId` один.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-105">Enable reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using `principalId`, `resourceId`, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac5fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac5fe-106">Permissions</span></span>
<span data-ttu-id="ac5fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac5fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac5fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac5fe-109">Permission type</span></span>|<span data-ttu-id="ac5fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac5fe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac5fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac5fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ac5fe-112">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5fe-112">AccessReviews.ReadWrite.All</span></span>|
|<span data-ttu-id="ac5fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac5fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac5fe-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ac5fe-114">Not supported</span></span>|
|<span data-ttu-id="ac5fe-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ac5fe-115">Application</span></span>|<span data-ttu-id="ac5fe-116">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5fe-116">AccessReviews.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac5fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac5fe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="ac5fe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac5fe-118">Request headers</span></span>
|<span data-ttu-id="ac5fe-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ac5fe-119">Name</span></span>|<span data-ttu-id="ac5fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ac5fe-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ac5fe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac5fe-121">Authorization</span></span>|<span data-ttu-id="ac5fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ac5fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ac5fe-124">Content-Type</span></span>|<span data-ttu-id="ac5fe-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac5fe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac5fe-127">Request body</span></span>
<span data-ttu-id="ac5fe-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ac5fe-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ac5fe-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="ac5fe-130">Parameter</span></span>|<span data-ttu-id="ac5fe-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ac5fe-131">Type</span></span>|<span data-ttu-id="ac5fe-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ac5fe-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="ac5fe-133">решение</span><span class="sxs-lookup"><span data-stu-id="ac5fe-133">decision</span></span>  | <span data-ttu-id="ac5fe-134">String</span><span class="sxs-lookup"><span data-stu-id="ac5fe-134">String</span></span> | <span data-ttu-id="ac5fe-135">Решение о доступе для проверяемого объекта.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="ac5fe-136">Возможные значения: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="ac5fe-137">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-137">Required.</span></span>  |
|  <span data-ttu-id="ac5fe-138">обоснование</span><span class="sxs-lookup"><span data-stu-id="ac5fe-138">justification</span></span> | <span data-ttu-id="ac5fe-139">String</span><span class="sxs-lookup"><span data-stu-id="ac5fe-139">String</span></span> | <span data-ttu-id="ac5fe-140">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-140">Context of the review provided to admins.</span></span> <span data-ttu-id="ac5fe-141">Обязательно, **если justificationRequiredOnApproval** находится `True` на **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-141">Required if **justificationRequiredOnApproval** is `True` on the **accessReviewScheduleDefinition**.</span></span>  |
|<span data-ttu-id="ac5fe-142">principalId</span><span class="sxs-lookup"><span data-stu-id="ac5fe-142">principalId</span></span>|<span data-ttu-id="ac5fe-143">String</span><span class="sxs-lookup"><span data-stu-id="ac5fe-143">String</span></span>|<span data-ttu-id="ac5fe-144">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **principalId.**</span><span class="sxs-lookup"><span data-stu-id="ac5fe-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** will be reviewed in this batch.</span></span> <span data-ttu-id="ac5fe-145">Если они не будут предоставлены, все **principalIds** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-145">If not supplied, all **principalIds** will be reviewed.</span></span>|
|<span data-ttu-id="ac5fe-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="ac5fe-146">resourceId</span></span>|<span data-ttu-id="ac5fe-147">String</span><span class="sxs-lookup"><span data-stu-id="ac5fe-147">String</span></span>|<span data-ttu-id="ac5fe-148">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **resourceId.**</span><span class="sxs-lookup"><span data-stu-id="ac5fe-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="ac5fe-149">Если они не будут предоставлены, **все resourceIds** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-149">If not supplied, all **resourceIds** will be reviewed.</span></span>|



## <a name="response"></a><span data-ttu-id="ac5fe-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac5fe-150">Response</span></span>

<span data-ttu-id="ac5fe-151">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ac5fe-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ac5fe-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac5fe-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac5fe-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac5fe-153">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json
Content-length: 113

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```


### <a name="response"></a><span data-ttu-id="ac5fe-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac5fe-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
