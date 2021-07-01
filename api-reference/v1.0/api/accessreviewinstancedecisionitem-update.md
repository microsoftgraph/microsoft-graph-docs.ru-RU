---
title: Обновление accessReviewInstanceDecisionItem
description: Обновление свойств объекта accessReviewInstanceDecisionItem.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ca2f5c24f10bd287b73502ec3d8ba5b6c399da18
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209621"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="86af1-103">Обновление accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="86af1-103">Update accessReviewInstanceDecisionItem</span></span>
<span data-ttu-id="86af1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86af1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86af1-105">Обновление свойств объекта [accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="86af1-105">Update the properties of an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="86af1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86af1-106">Permissions</span></span>
<span data-ttu-id="86af1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86af1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86af1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86af1-109">Permission type</span></span>|<span data-ttu-id="86af1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86af1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86af1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86af1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86af1-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86af1-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="86af1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86af1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86af1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86af1-114">Not supported.</span></span>|
|<span data-ttu-id="86af1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="86af1-115">Application</span></span>|<span data-ttu-id="86af1-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86af1-116">AccessReview.ReadWrite.All</span></span>|

<span data-ttu-id="86af1-117">Обновить **accessReviewInstanceDecisionItem** может только пользователь вызовов, который указан в качестве рецензента для родительского доступаReviewInstanceDecisionItem. [](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="86af1-117">Only a calling user who is listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md) can update the **accessReviewInstanceDecisionItem**.</span></span>

## <a name="http-request"></a><span data-ttu-id="86af1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86af1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="86af1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86af1-119">Request headers</span></span>
|<span data-ttu-id="86af1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="86af1-120">Name</span></span>|<span data-ttu-id="86af1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="86af1-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86af1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86af1-122">Authorization</span></span>|<span data-ttu-id="86af1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86af1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86af1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86af1-125">Content-Type</span></span>|<span data-ttu-id="86af1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86af1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86af1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86af1-128">Request body</span></span>
<span data-ttu-id="86af1-129">В теле запроса подарите JSON представление [объекта accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="86af1-129">In the request body, supply a JSON representation of the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object.</span></span>

<span data-ttu-id="86af1-130">В следующей таблице показаны свойства, которые принимаются при обновлении [accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)</span><span class="sxs-lookup"><span data-stu-id="86af1-130">The following table shows the properties that are accepted when you update the [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md).</span></span>

|<span data-ttu-id="86af1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="86af1-131">Property</span></span>|<span data-ttu-id="86af1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="86af1-132">Type</span></span>|<span data-ttu-id="86af1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="86af1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86af1-134">решение</span><span class="sxs-lookup"><span data-stu-id="86af1-134">decision</span></span>|<span data-ttu-id="86af1-135">String</span><span class="sxs-lookup"><span data-stu-id="86af1-135">String</span></span>|<span data-ttu-id="86af1-136">Проверятель голосует о том, должен ли директор иметь доступ к просматриваемом ресурсу.</span><span class="sxs-lookup"><span data-stu-id="86af1-136">The reviewer's vote on whether the principal should have access to the resource under review.</span></span> <span data-ttu-id="86af1-137">Возможные значения: `Approve` `Deny` , или `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="86af1-137">Possible values: `Approve`, `Deny`, or `DontKnow`.</span></span> <span data-ttu-id="86af1-138">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="86af1-138">Required.</span></span>|
|<span data-ttu-id="86af1-139">обоснование</span><span class="sxs-lookup"><span data-stu-id="86af1-139">justification</span></span>|<span data-ttu-id="86af1-140">String</span><span class="sxs-lookup"><span data-stu-id="86af1-140">String</span></span>|<span data-ttu-id="86af1-141">Причина принятия решения рецензентом.</span><span class="sxs-lookup"><span data-stu-id="86af1-141">The reviewer's reason for decision.</span></span> <span data-ttu-id="86af1-142">Требуется, если **обоснованиеRequiredOnApproval** свойства параметров [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) `true` является .</span><span class="sxs-lookup"><span data-stu-id="86af1-142">Required if the **justificationRequiredOnApproval** of the settings property of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="86af1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="86af1-143">Response</span></span>

<span data-ttu-id="86af1-144">В случае успешного выполнения этот метод возвращает код отклика `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="86af1-144">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="86af1-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="86af1-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86af1-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="86af1-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="86af1-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="86af1-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstancedecisionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555
Content-Type: application/json
Content-length: 691

{
  "decision": "Approve",
  "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
}
```
# <a name="c"></a>[<span data-ttu-id="86af1-148">C#</span><span class="sxs-lookup"><span data-stu-id="86af1-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86af1-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86af1-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86af1-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86af1-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86af1-151">Java</span><span class="sxs-lookup"><span data-stu-id="86af1-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="86af1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="86af1-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
