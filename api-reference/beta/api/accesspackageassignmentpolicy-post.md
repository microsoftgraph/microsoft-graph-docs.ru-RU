---
title: Создание accessPackageAssignmentPolicy
description: Используйте этот API для создания нового accessPackageAssignmentPolicy.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6868c48fd2fdfba309a0af5849451a039bae1769
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439704"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="fa649-103">Создание accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="fa649-103">Create accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="fa649-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa649-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa649-105">В [управлении правами Azure AD](../resources/entitlementmanagement-root.md)создайте новый [объект accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa649-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa649-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa649-106">Permissions</span></span>

<span data-ttu-id="fa649-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa649-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa649-109">Permission type</span></span>                        | <span data-ttu-id="fa649-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa649-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa649-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa649-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa649-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa649-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="fa649-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa649-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa649-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa649-114">Not supported.</span></span> |
| <span data-ttu-id="fa649-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fa649-115">Application</span></span>                            | <span data-ttu-id="fa649-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa649-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa649-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa649-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="fa649-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa649-118">Request headers</span></span>

| <span data-ttu-id="fa649-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fa649-119">Name</span></span>          | <span data-ttu-id="fa649-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fa649-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fa649-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa649-121">Authorization</span></span> | <span data-ttu-id="fa649-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="fa649-122">Bearer \{token\}.</span></span> <span data-ttu-id="fa649-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="fa649-123">Required.</span></span> |
| <span data-ttu-id="fa649-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa649-124">Content-Type</span></span>  | <span data-ttu-id="fa649-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa649-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa649-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa649-127">Request body</span></span>

<span data-ttu-id="fa649-128">В теле запроса поставляем представление JSON объекта [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fa649-128">In the request body, supply a JSON representation of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fa649-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa649-129">Response</span></span>

<span data-ttu-id="fa649-130">В случае успешного выполнения этот метод возвращает код отклика из 200 серий и новый [объект accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fa649-130">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa649-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa649-131">Examples</span></span>

### <a name="example-1-create-a-direct-assignment-policy"></a><span data-ttu-id="fa649-132">Пример 1. Создание политики прямого назначения</span><span class="sxs-lookup"><span data-stu-id="fa649-132">Example 1: Create a direct assignment policy</span></span>

<span data-ttu-id="fa649-133">Политика прямого назначения полезна, когда запросы на назначение пакетов доступа будут создаваться только администратором, а не самими пользователями.</span><span class="sxs-lookup"><span data-stu-id="fa649-133">A direct assignment policy is useful when access package assignment requests will only be created by an administrator, not by users themselves.</span></span>

#### <a name="request"></a><span data-ttu-id="fa649-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa649-134">Request</span></span>

<span data-ttu-id="fa649-135">В следующем примере показан запрос на создание политики назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="fa649-135">The following example shows a request to create an access package assignment policy.</span></span> <span data-ttu-id="fa649-136">В этой политике пользователи не могут запрашивать, не требуется утверждение и нет отзывов доступа.</span><span class="sxs-lookup"><span data-stu-id="fa649-136">In this policy, no users can request, no approval is required, and there are no access reviews.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa649-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa649-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "NoSubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```
# <a name="c"></a>[<span data-ttu-id="fa649-138">C#</span><span class="sxs-lookup"><span data-stu-id="fa649-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa649-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa649-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa649-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa649-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa649-141">Java</span><span class="sxs-lookup"><span data-stu-id="fa649-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="fa649-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa649-142">Response</span></span>

<span data-ttu-id="fa649-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa649-143">The following is an example of the response.</span></span>

> <span data-ttu-id="fa649-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa649-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "displayName": "direct",
  "description": "direct assignments by administrator"
}
```

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a><span data-ttu-id="fa649-146">Пример 2. Создание политики для запроса пользователями из других организаций</span><span class="sxs-lookup"><span data-stu-id="fa649-146">Example 2: Create a policy for users from other organizations to request</span></span>

<span data-ttu-id="fa649-147">В следующем примере показана более сложная политика с двух этапами утверждений и обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="fa649-147">The following example shows a more complex policy with two-stage approvals and access reviews.</span></span>

#### <a name="request"></a><span data-ttu-id="fa649-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa649-148">Request</span></span>

<span data-ttu-id="fa649-149">Ниже приводится пример запроса на создание политики назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="fa649-149">The following is an example of the request to create an access package assignment policy.</span></span> 


# <a name="http"></a>[<span data-ttu-id="fa649-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa649-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies_multistage"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
    "accessPackageId": "string (identifier)",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true,
        "allowedRequestors": []
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "Serial",
        "approvalStages": [
            {
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ],
                "escalationApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "user if the external sponsor does not respond"
                    }
                ]
            },
            {
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "group for users from connected organizations which have no internal sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.internalSponsors",
                        "isBackup": false
                    }
                ],
                "escalationApprovers": [
                    {
                        "@odata.type": "#microsoft.graph.singleUser",
                        "isBackup": true,
                        "id": "string (identifier)",
                        "description": "user if the internal sponsor does not respond"
                    }
                ]
            }
        ]
    },
    "accessReviewSettings": {
        "isEnabled": true,
        "recurrenceType": "quarterly",
        "reviewerType": "Self",
        "startDateTime": "2020-04-01T07:59:59.998Z",
        "durationInDays": 25,
        "reviewers": []
    }
}
```
# <a name="c"></a>[<span data-ttu-id="fa649-151">C#</span><span class="sxs-lookup"><span data-stu-id="fa649-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa649-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa649-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa649-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa649-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa649-154">Java</span><span class="sxs-lookup"><span data-stu-id="fa649-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="fa649-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa649-155">Response</span></span>

<span data-ttu-id="fa649-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa649-156">The following is an example of the response.</span></span>

> <span data-ttu-id="fa649-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa649-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "string (identifier)",
  "displayName": "Users from connected organizations can request",
  "description": "Allow users from configured connected organizations to request and be approved by their sponsors"
}
```

### <a name="example-3-create-assignment-policy-with-questions"></a><span data-ttu-id="fa649-159">Пример 3. Создание политики назначения с помощью вопросов</span><span class="sxs-lookup"><span data-stu-id="fa649-159">Example 3: Create assignment policy with questions</span></span>

<span data-ttu-id="fa649-160">Вопросы, настроенные в политике назначения, будут задаваться запрашивателям в области политики.</span><span class="sxs-lookup"><span data-stu-id="fa649-160">Questions configured in an assignment policy will be asked to requestors in scope of the policy.</span></span> <span data-ttu-id="fa649-161">Их ответы будут показаны их утверждениям.</span><span class="sxs-lookup"><span data-stu-id="fa649-161">Their answers will be shown to their approvers.</span></span> <span data-ttu-id="fa649-162">ID-вопросы являются только для чтения и включаются в ответ по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fa649-162">Question IDs are read-only and are included in the response by default.</span></span>

#### <a name="request"></a><span data-ttu-id="fa649-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa649-163">Request</span></span>

<span data-ttu-id="fa649-164">В следующем примере показан запрос на создание политики назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="fa649-164">The following example shows a request to create an access package assignment policy.</span></span> 



# <a name="http"></a>[<span data-ttu-id="fa649-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa649-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies_questions"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
    "accessPackageId": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "displayName": "Users from connected organizations can request",
    "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
    "canExtend": false,
    "durationInDays": 365,
    "expirationDateTime": null,
    "requestorSettings": {
        "scopeType": "AllExistingConnectedOrganizationSubjects",
        "acceptRequests": true
    },
    "requestApprovalSettings": {
        "isApprovalRequired": true,
        "isApprovalRequiredForExtension": false,
        "isRequestorJustificationRequired": true,
        "approvalMode": "SingleStage",
        "approvalStages": [{
                "approvalStageTimeOutInDays": 14,
                "isApproverJustificationRequired": true,
                "isEscalationEnabled": true,
                "escalationTimeInMinutes": 11520,
                "primaryApprovers": [{
                        "@odata.type": "#microsoft.graph.groupMembers",
                        "isBackup": true,
                        "id": "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
                        "description": "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        "@odata.type": "#microsoft.graph.externalSponsors",
                        "isBackup": false
                    }
                ]
            }
        ]
    },
    "accessReviewSettings": {
        "isEnabled": false
    },
    "questions": [{
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
}
```
# <a name="c"></a>[<span data-ttu-id="fa649-166">C#</span><span class="sxs-lookup"><span data-stu-id="fa649-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa649-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa649-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa649-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa649-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa649-169">Java</span><span class="sxs-lookup"><span data-stu-id="fa649-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-questions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---

#### <a name="response"></a><span data-ttu-id="fa649-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa649-170">Response</span></span>

<span data-ttu-id="fa649-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa649-171">The following is an example of the response.</span></span>

> <span data-ttu-id="fa649-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa649-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "4c02f928-7752-49aa-8fc8-e286d973a965",
  "accessPackageId": "string (identifier)",
  "displayName": "Users from connected organizations can request",
  "description": "Allow users from configured connected organizations to request and be approved by their sponsors",
  "questions": [{
        "id" : "BD3F6B95-458D-4BC8-A9A6-8D4B29F64F3D",
        "isRequired": false,
        "text": {
            "defaultText": "what state are you from?",
            "localizedTexts": [{
                "text": "¿De qué estado eres?",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        "choices": [{
            "actualValue": "AZ",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Arizona?",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "CA",
            "displayValue": {
                "localizedTexts": [{
                    "text": "California",
                    "languageCode": "es"
                }]
            }
        }, {
            "actualValue": "OH",
            "displayValue": {
                "localizedTexts": [{
                    "text": "Ohio",
                    "languageCode": "es"
                }]
            }
        }],
        "allowsMultipleSelection": false
    }, {
        "id" : "F652C13C-A660-4E4C-A1E0-CE9FEC6EE57A",
        "isRequired": false,
        "text": {
            "defaultText": "Who is your manager?",
            "localizedTexts": [{
                "text": "por qué necesita acceso a este paquete",
                "languageCode": "es"
            }]
        },
        "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
        "isSingleLineQuestion": false
    }]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


