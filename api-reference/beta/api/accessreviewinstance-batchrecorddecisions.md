---
title: 'accessReviewInstance: batchRecordDecisions'
description: Позволяет рецензентам просмотреть все объекты accessReviewInstanceDecisionItem пакетами.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ab7e7e3580275aa127bbb01e34484a823d4b01bf
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030749"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="4e1af-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="4e1af-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="4e1af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e1af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e1af-105">Позволяет рецензентам просмотреть все [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) пакетами с помощью **principalId,** **resourceId** или ни того, ни другго.</span><span class="sxs-lookup"><span data-stu-id="4e1af-105">Enables reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using **principalId**, **resourceId**, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e1af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e1af-106">Permissions</span></span>
<span data-ttu-id="4e1af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e1af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e1af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e1af-109">Permission type</span></span>|<span data-ttu-id="4e1af-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e1af-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e1af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e1af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4e1af-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e1af-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="4e1af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e1af-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e1af-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4e1af-114">Not supported</span></span>|
|<span data-ttu-id="4e1af-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4e1af-115">Application</span></span>|<span data-ttu-id="4e1af-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e1af-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e1af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e1af-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="4e1af-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e1af-118">Request headers</span></span>
|<span data-ttu-id="4e1af-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4e1af-119">Name</span></span>|<span data-ttu-id="4e1af-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4e1af-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4e1af-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e1af-121">Authorization</span></span>|<span data-ttu-id="4e1af-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e1af-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4e1af-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e1af-124">Content-Type</span></span>|<span data-ttu-id="4e1af-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e1af-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e1af-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e1af-127">Request body</span></span>
<span data-ttu-id="4e1af-128">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e1af-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4e1af-129">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4e1af-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4e1af-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="4e1af-130">Parameter</span></span>|<span data-ttu-id="4e1af-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4e1af-131">Type</span></span>|<span data-ttu-id="4e1af-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4e1af-132">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="4e1af-133">решение</span><span class="sxs-lookup"><span data-stu-id="4e1af-133">decision</span></span>  | <span data-ttu-id="4e1af-134">String</span><span class="sxs-lookup"><span data-stu-id="4e1af-134">String</span></span> | <span data-ttu-id="4e1af-135">Решение о доступе для проверяемого объекта.</span><span class="sxs-lookup"><span data-stu-id="4e1af-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="4e1af-136">Возможные значения: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="4e1af-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="4e1af-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e1af-137">Required.</span></span>  |
|  <span data-ttu-id="4e1af-138">обоснование</span><span class="sxs-lookup"><span data-stu-id="4e1af-138">justification</span></span> | <span data-ttu-id="4e1af-139">String</span><span class="sxs-lookup"><span data-stu-id="4e1af-139">String</span></span> | <span data-ttu-id="4e1af-140">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="4e1af-140">Context of the review provided to admins.</span></span> <span data-ttu-id="4e1af-141">Обязательно, **если justificationRequiredOnApproval** находится `True` на **accessReviewScheduleDefinition**.</span><span class="sxs-lookup"><span data-stu-id="4e1af-141">Required if **justificationRequiredOnApproval** is `True` on the **accessReviewScheduleDefinition**.</span></span>  |
|<span data-ttu-id="4e1af-142">principalId</span><span class="sxs-lookup"><span data-stu-id="4e1af-142">principalId</span></span>|<span data-ttu-id="4e1af-143">String</span><span class="sxs-lookup"><span data-stu-id="4e1af-143">String</span></span>|<span data-ttu-id="4e1af-144">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **principalId.**</span><span class="sxs-lookup"><span data-stu-id="4e1af-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** will be reviewed in this batch.</span></span> <span data-ttu-id="4e1af-145">Если они не будут предоставлены, все **principalIds** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="4e1af-145">If not supplied, all **principalIds** will be reviewed.</span></span>|
|<span data-ttu-id="4e1af-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="4e1af-146">resourceId</span></span>|<span data-ttu-id="4e1af-147">String</span><span class="sxs-lookup"><span data-stu-id="4e1af-147">String</span></span>|<span data-ttu-id="4e1af-148">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **resourceId.**</span><span class="sxs-lookup"><span data-stu-id="4e1af-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="4e1af-149">Если они не будут предоставлены, **все resourceIds** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="4e1af-149">If not supplied, all **resourceIds** will be reviewed.</span></span>|



## <a name="response"></a><span data-ttu-id="4e1af-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="4e1af-150">Response</span></span>

<span data-ttu-id="4e1af-151">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4e1af-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4e1af-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="4e1af-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4e1af-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e1af-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4e1af-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e1af-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[<span data-ttu-id="4e1af-155">C#</span><span class="sxs-lookup"><span data-stu-id="4e1af-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e1af-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e1af-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e1af-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e1af-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e1af-158">Java</span><span class="sxs-lookup"><span data-stu-id="4e1af-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4e1af-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e1af-159">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
