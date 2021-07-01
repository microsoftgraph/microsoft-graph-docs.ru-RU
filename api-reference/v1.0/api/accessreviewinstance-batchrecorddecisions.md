---
title: 'accessReviewInstance: batchRecordDecisions'
description: Позволяет рецензентам просмотреть все accessReviewInstanceDecisionItems пакетами.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8793838a67199a5d5d752e6865c2f8e3c97b262e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210629"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a><span data-ttu-id="79592-103">accessReviewInstance: batchRecordDecisions</span><span class="sxs-lookup"><span data-stu-id="79592-103">accessReviewInstance: batchRecordDecisions</span></span>
<span data-ttu-id="79592-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79592-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="79592-105">Позволяет рецензентам просмотреть все [объекты accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) пакетами с помощью **principalId,** **resourceId** или ни того, ни другго.</span><span class="sxs-lookup"><span data-stu-id="79592-105">Enables reviewers to review all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects in batches by using **principalId**, **resourceId**, or neither.</span></span>

## <a name="permissions"></a><span data-ttu-id="79592-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79592-106">Permissions</span></span>
<span data-ttu-id="79592-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79592-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79592-109">Permission type</span></span>|<span data-ttu-id="79592-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79592-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79592-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79592-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79592-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79592-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="79592-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79592-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79592-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="79592-114">Not supported</span></span>|
|<span data-ttu-id="79592-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="79592-115">Application</span></span>|<span data-ttu-id="79592-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79592-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79592-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79592-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a><span data-ttu-id="79592-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79592-118">Request headers</span></span>
|<span data-ttu-id="79592-119">Имя</span><span class="sxs-lookup"><span data-stu-id="79592-119">Name</span></span>|<span data-ttu-id="79592-120">Описание</span><span class="sxs-lookup"><span data-stu-id="79592-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="79592-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79592-121">Authorization</span></span>|<span data-ttu-id="79592-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79592-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="79592-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79592-124">Content-Type</span></span>|<span data-ttu-id="79592-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79592-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79592-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79592-127">Request body</span></span>
<span data-ttu-id="79592-128">В теле запроса подарите JSON представление [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span><span class="sxs-lookup"><span data-stu-id="79592-128">In the request body, supply a JSON representation of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

<span data-ttu-id="79592-129">В следующей таблице перечислены свойства, которые можно использовать для просмотра [объектов accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="79592-129">The following table lists the properties that you can use to review [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects.</span></span>

|<span data-ttu-id="79592-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="79592-130">Parameter</span></span>|<span data-ttu-id="79592-131">Тип</span><span class="sxs-lookup"><span data-stu-id="79592-131">Type</span></span>|<span data-ttu-id="79592-132">Описание</span><span class="sxs-lookup"><span data-stu-id="79592-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79592-133">решение</span><span class="sxs-lookup"><span data-stu-id="79592-133">decision</span></span>|<span data-ttu-id="79592-134">String</span><span class="sxs-lookup"><span data-stu-id="79592-134">String</span></span>|<span data-ttu-id="79592-135">Решение о доступе для проверяемого объекта.</span><span class="sxs-lookup"><span data-stu-id="79592-135">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="79592-136">Возможные значения: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span><span class="sxs-lookup"><span data-stu-id="79592-136">Possible values are: `Approve`, `Deny`, `NotReviewed`, `DontKnow`.</span></span> <span data-ttu-id="79592-137">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="79592-137">Required.</span></span>|
|<span data-ttu-id="79592-138">обоснование</span><span class="sxs-lookup"><span data-stu-id="79592-138">justification</span></span>|<span data-ttu-id="79592-139">String</span><span class="sxs-lookup"><span data-stu-id="79592-139">String</span></span>|<span data-ttu-id="79592-140">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="79592-140">Context of the review provided to admins.</span></span> <span data-ttu-id="79592-141">Требуется, **если обоснованиеRequiredOnApproval** свойства параметров **accessReviewScheduleDefinition** является `true` .</span><span class="sxs-lookup"><span data-stu-id="79592-141">Required if **justificationRequiredOnApproval** of the settings property of the **accessReviewScheduleDefinition** is `true` .</span></span>|
|<span data-ttu-id="79592-142">principalId</span><span class="sxs-lookup"><span data-stu-id="79592-142">principalId</span></span>|<span data-ttu-id="79592-143">String</span><span class="sxs-lookup"><span data-stu-id="79592-143">String</span></span>|<span data-ttu-id="79592-144">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **значениям principalId.**</span><span class="sxs-lookup"><span data-stu-id="79592-144">If supplied, all the **accessReviewInstanceDecisionItems** with matching **principalId** values will be reviewed in this batch.</span></span> <span data-ttu-id="79592-145">Если они не будут предоставлены, **все accessReviewInstanceDecisionItems** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="79592-145">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|
|<span data-ttu-id="79592-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="79592-146">resourceId</span></span>|<span data-ttu-id="79592-147">String</span><span class="sxs-lookup"><span data-stu-id="79592-147">String</span></span>|<span data-ttu-id="79592-148">В этом пакете будут рассмотрены все **accessReviewInstanceDecisionItems** с соответствием **resourceId.**</span><span class="sxs-lookup"><span data-stu-id="79592-148">If supplied, all the **accessReviewInstanceDecisionItems** with matching **resourceId** will be reviewed in this batch.</span></span> <span data-ttu-id="79592-149">Если они не будут предоставлены, **все accessReviewInstanceDecisionItems** будут рассмотрены.</span><span class="sxs-lookup"><span data-stu-id="79592-149">If not supplied, all **accessReviewInstanceDecisionItems** will be reviewed.</span></span>|

## <a name="response"></a><span data-ttu-id="79592-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="79592-150">Response</span></span>

<span data-ttu-id="79592-151">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="79592-151">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="79592-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="79592-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79592-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="79592-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="79592-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="79592-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="79592-155">C#</span><span class="sxs-lookup"><span data-stu-id="79592-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79592-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79592-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79592-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79592-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79592-158">Java</span><span class="sxs-lookup"><span data-stu-id="79592-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="79592-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="79592-159">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
