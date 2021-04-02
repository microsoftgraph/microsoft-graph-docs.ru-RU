---
title: 'accessReviewInstance: batchRecordDecisions'
description: Emable reviewers to review all accessReviewInstanceDecisionItems in batches.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a8bd6778d54100340b0c846230fd8b91b696f1fb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507503"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="dc3f4-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="dc3f4-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="dc3f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc3f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc3f4-105">Включить рецензенты для просмотра всех [объектов accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) пакетами с помощью `principalId` , или ни `resourceId` один.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-105">Enable reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using `principalId`, `resourceId`, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc3f4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc3f4-106">Permissions</span></span>
<span data-ttu-id="dc3f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc3f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc3f4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc3f4-109">Permission type</span></span>|<span data-ttu-id="dc3f4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc3f4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc3f4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc3f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc3f4-112">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc3f4-112">AccessReviews.ReadWrite.All</span></span>|
|<span data-ttu-id="dc3f4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc3f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc3f4-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc3f4-114">Not supported</span></span>|
|<span data-ttu-id="dc3f4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="dc3f4-115">Application</span></span>|<span data-ttu-id="dc3f4-116">AccessReviews.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc3f4-116">AccessReviews.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc3f4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc3f4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="dc3f4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc3f4-118">Request headers</span></span>
|<span data-ttu-id="dc3f4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="dc3f4-119">Name</span></span>|<span data-ttu-id="dc3f4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dc3f4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dc3f4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc3f4-121">Authorization</span></span>|<span data-ttu-id="dc3f4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dc3f4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc3f4-124">Content-Type</span></span>|<span data-ttu-id="dc3f4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc3f4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc3f4-127">Request body</span></span>
<span data-ttu-id="dc3f4-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="dc3f4-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="dc3f4-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="dc3f4-130">Parameter</span></span>|<span data-ttu-id="dc3f4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dc3f4-131">Type</span></span>|<span data-ttu-id="dc3f4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dc3f4-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="dc3f4-133">решение</span><span class="sxs-lookup"><span data-stu-id="dc3f4-133">decision</span></span>  | <span data-ttu-id="dc3f4-134">String</span><span class="sxs-lookup"><span data-stu-id="dc3f4-134">String</span></span> | <span data-ttu-id="dc3f4-135">Решение о доступе для проверяемого объекта.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="dc3f4-136">Возможные значения: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="dc3f4-137">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-137">Required.</span></span>  |
|  <span data-ttu-id="dc3f4-138">обоснование</span><span class="sxs-lookup"><span data-stu-id="dc3f4-138">justification</span></span> | <span data-ttu-id="dc3f4-139">String</span><span class="sxs-lookup"><span data-stu-id="dc3f4-139">String</span></span> | <span data-ttu-id="dc3f4-140">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-140">Context of the review provided to admins.</span></span> <span data-ttu-id="dc3f4-141">Обязательно, **если justificationRequiredOnApproval** находится `True` на **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-141">Required if **justificationRequiredOnApproval** is `True` on the **accessReviewScheduleDefinition**.</span></span>  |
|<span data-ttu-id="dc3f4-142">principalId</span><span class="sxs-lookup"><span data-stu-id="dc3f4-142">principalId</span></span>|<span data-ttu-id="dc3f4-143">String</span><span class="sxs-lookup"><span data-stu-id="dc3f4-143">String</span></span>|<span data-ttu-id="dc3f4-144">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **principalId.**</span><span class="sxs-lookup"><span data-stu-id="dc3f4-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** will be reviewed in this batch.</span></span> <span data-ttu-id="dc3f4-145">Если они не будут предоставлены, все **principalIds** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-145">If not supplied, all **principalIds** will be reviewed.</span></span>|
|<span data-ttu-id="dc3f4-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="dc3f4-146">resourceId</span></span>|<span data-ttu-id="dc3f4-147">String</span><span class="sxs-lookup"><span data-stu-id="dc3f4-147">String</span></span>|<span data-ttu-id="dc3f4-148">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **resourceId.**</span><span class="sxs-lookup"><span data-stu-id="dc3f4-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="dc3f4-149">Если они не будут предоставлены, **все resourceIds** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-149">If not supplied, all **resourceIds** will be reviewed.</span></span>|



## <a name="response"></a><span data-ttu-id="dc3f4-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc3f4-150">Response</span></span>

<span data-ttu-id="dc3f4-151">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc3f4-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="dc3f4-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="dc3f4-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc3f4-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc3f4-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dc3f4-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc3f4-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dc3f4-155">C#</span><span class="sxs-lookup"><span data-stu-id="dc3f4-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc3f4-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc3f4-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc3f4-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc3f4-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc3f4-158">Java</span><span class="sxs-lookup"><span data-stu-id="dc3f4-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dc3f4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc3f4-159">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
