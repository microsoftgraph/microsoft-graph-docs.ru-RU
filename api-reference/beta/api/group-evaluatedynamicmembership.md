---
title: 'группа: оценкаDynamicMembership'
description: Оцените, является ли пользователь или устройство членом динамической группы.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: de8e44a79644bcea5e3c44b214580e16359468e2
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681769"
---
# <a name="group-evaluatedynamicmembership"></a><span data-ttu-id="d9943-103">группа: оценкаDynamicMembership</span><span class="sxs-lookup"><span data-stu-id="d9943-103">group: evaluateDynamicMembership</span></span>

<span data-ttu-id="d9943-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9943-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9943-105">Определите, может ли пользователь или устройство являться членом динамической группы.</span><span class="sxs-lookup"><span data-stu-id="d9943-105">Evaluate whether a user or device is or would be a member of a dynamic group.</span></span> <span data-ttu-id="d9943-106">Правило членства возвращается вместе с другими сведениями, которые были использованы в оценке.</span><span class="sxs-lookup"><span data-stu-id="d9943-106">The membership rule is returned along with other details that were used in the evaluation.</span></span> <span data-ttu-id="d9943-107">Эту операцию можно выполнить следующими способами:</span><span class="sxs-lookup"><span data-stu-id="d9943-107">You can complete this operation in the following ways:</span></span> 

- <span data-ttu-id="d9943-108">Оцените, является ли пользователь или устройство членом указанной динамической группы.</span><span class="sxs-lookup"><span data-stu-id="d9943-108">Evaluate whether a user or device is a member of a specified dynamic group.</span></span>  
- <span data-ttu-id="d9943-109">Оцените, будет ли пользователь или устройство членом динамической группы на основе ID пользователя или устройства и правила членства.</span><span class="sxs-lookup"><span data-stu-id="d9943-109">Evaluate whether a user or device would be a member of a dynamic group based on the ID of the user or device and a membership rule.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9943-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9943-110">Permissions</span></span>

<span data-ttu-id="d9943-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9943-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a><span data-ttu-id="d9943-113">Оценка динамического членства с помощью ID участника и группового ИД</span><span class="sxs-lookup"><span data-stu-id="d9943-113">Evaluate dynamic membership with member ID and group ID</span></span>

| <span data-ttu-id="d9943-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9943-114">Permission type</span></span> | <span data-ttu-id="d9943-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9943-115">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="d9943-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9943-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d9943-117">Для пользователя: Group.Read.All и User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9943-117">For user: Group.Read.All and User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="d9943-118">Для устройства: Group.Read.All и Device.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9943-118">For device: Group.Read.All and Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="d9943-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9943-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9943-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9943-120">Not supported.</span></span> |
| <span data-ttu-id="d9943-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9943-121">Application</span></span>                            | <span data-ttu-id="d9943-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9943-122">Not supported.</span></span> |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a><span data-ttu-id="d9943-123">Оценка динамического членства с помощью ID и правила членства</span><span class="sxs-lookup"><span data-stu-id="d9943-123">Evaluate dynamic membership with member ID and membership rule</span></span>

| <span data-ttu-id="d9943-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9943-124">Permission type</span></span> | <span data-ttu-id="d9943-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9943-125">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="d9943-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9943-126">Delegated (work or school account)</span></span> | <span data-ttu-id="d9943-127">Для пользователя: User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9943-127">For user: User.Read.All, Directory.Read.All</span></span><br><span data-ttu-id="d9943-128">Для устройства: Device.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9943-128">For device: Device.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="d9943-129">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9943-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9943-130">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9943-130">Not supported.</span></span> |
| <span data-ttu-id="d9943-131">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9943-131">Application</span></span>                            | <span data-ttu-id="d9943-132">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9943-132">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9943-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9943-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a><span data-ttu-id="d9943-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9943-134">Request headers</span></span>

| <span data-ttu-id="d9943-135">Имя</span><span class="sxs-lookup"><span data-stu-id="d9943-135">Name</span></span> | <span data-ttu-id="d9943-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d9943-136">Description</span></span> |
| :--- | :---------- |
| <span data-ttu-id="d9943-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9943-137">Authorization</span></span> | <span data-ttu-id="d9943-138">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d9943-138">Bearer {token}</span></span> |
| <span data-ttu-id="d9943-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d9943-139">Content-type</span></span>  | <span data-ttu-id="d9943-140">application/json</span><span class="sxs-lookup"><span data-stu-id="d9943-140">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9943-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9943-141">Request body</span></span>

<span data-ttu-id="d9943-142">В теле запроса укажи необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="d9943-142">In the request body, supply the required properties.</span></span>

<span data-ttu-id="d9943-143">В следующей таблице перечислены свойства, необходимые при оценке членства в группе.</span><span class="sxs-lookup"><span data-stu-id="d9943-143">The following table lists the properties that are required when you evaluate group membership.</span></span>

| <span data-ttu-id="d9943-144">Параметр</span><span class="sxs-lookup"><span data-stu-id="d9943-144">Parameter</span></span> | <span data-ttu-id="d9943-145">Тип</span><span class="sxs-lookup"><span data-stu-id="d9943-145">Type</span></span> | <span data-ttu-id="d9943-146">Описание</span><span class="sxs-lookup"><span data-stu-id="d9943-146">Description</span></span> |
| :-------- | :--- | :---------- |
| <span data-ttu-id="d9943-147">memberId</span><span class="sxs-lookup"><span data-stu-id="d9943-147">memberId</span></span> | <span data-ttu-id="d9943-148">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d9943-148">String collection</span></span> | <span data-ttu-id="d9943-149">memberId — это объектный id пользователя или устройства, для оценки.</span><span class="sxs-lookup"><span data-stu-id="d9943-149">memberId is the object Id of the user or device to be evaluated.</span></span> |
| <span data-ttu-id="d9943-150">membershipRule</span><span class="sxs-lookup"><span data-stu-id="d9943-150">membershipRule</span></span> | <span data-ttu-id="d9943-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d9943-151">String collection</span></span> | <span data-ttu-id="d9943-152">Правило, которое используется для оценки членства.</span><span class="sxs-lookup"><span data-stu-id="d9943-152">The rule that is used for membership evaluation.</span></span> <span data-ttu-id="d9943-153">Если это свойство не предоставлено, оценивается правило для существующей группы.</span><span class="sxs-lookup"><span data-stu-id="d9943-153">If this property is not provided, the rule for the existing group is evaluated.</span></span> <span data-ttu-id="d9943-154">Если это свойство предоставлено, пользователь или устройство оцениваются для возможного членства в группе с тем же правилом.</span><span class="sxs-lookup"><span data-stu-id="d9943-154">If this property is provided, the user or device is evaluated for possible membership in a group with the same rule.</span></span> <span data-ttu-id="d9943-155">Дополнительные сведения см. в [программе Dynamic membership rules for groups in Azure Active Directory.](/azure/active-directory/users-groups-roles/groups-dynamic-membership)</span><span class="sxs-lookup"><span data-stu-id="d9943-155">For more information, see [Dynamic membership rules for groups in Azure Active Directory](/azure/active-directory/users-groups-roles/groups-dynamic-membership).</span></span>|

## <a name="response"></a><span data-ttu-id="d9943-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9943-156">Response</span></span>

<span data-ttu-id="d9943-157">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект evaluateDynamicMembershipResult.](../resources/evaluatedynamicmembershipresult.md)</span><span class="sxs-lookup"><span data-stu-id="d9943-157">If successful, this method returns a `200 OK` response code and an [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="d9943-158">Примеры</span><span class="sxs-lookup"><span data-stu-id="d9943-158">Examples</span></span>

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a><span data-ttu-id="d9943-159">Пример 1. Оценка того, является ли пользователь или устройство членом существующей группы</span><span class="sxs-lookup"><span data-stu-id="d9943-159">Example 1: Evaluate if a user or device is a member of an existing group</span></span>

#### <a name="request"></a><span data-ttu-id="d9943-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9943-160">Request</span></span>

<span data-ttu-id="d9943-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9943-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9943-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9943-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```
# <a name="c"></a>[<span data-ttu-id="d9943-163">C#</span><span class="sxs-lookup"><span data-stu-id="d9943-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9943-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9943-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9943-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9943-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9943-166">Java</span><span class="sxs-lookup"><span data-stu-id="d9943-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9943-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9943-167">Response</span></span>

<span data-ttu-id="d9943-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d9943-168">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a><span data-ttu-id="d9943-169">Пример 2. Оценка того, будет ли пользователь или устройство членом группы на основе правила членства</span><span class="sxs-lookup"><span data-stu-id="d9943-169">Example 2: Evaluate if a user or device would be a member of a group based on a membership rule</span></span>

#### <a name="request"></a><span data-ttu-id="d9943-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9943-170">Request</span></span>

<span data-ttu-id="d9943-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9943-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d9943-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9943-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_2"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership 
Content-type: application/json

{ 
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```
# <a name="c"></a>[<span data-ttu-id="d9943-173">C#</span><span class="sxs-lookup"><span data-stu-id="d9943-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9943-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9943-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9943-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9943-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9943-176">Java</span><span class="sxs-lookup"><span data-stu-id="d9943-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d9943-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9943-177">Response</span></span>

<span data-ttu-id="d9943-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d9943-178">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
