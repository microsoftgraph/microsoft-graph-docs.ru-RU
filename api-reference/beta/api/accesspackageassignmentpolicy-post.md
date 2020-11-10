---
title: Создание Акцесспаккажеассигнментполици
description: Используйте этот API для создания нового Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1551c886d814336cff44aa50c0713840a55239bf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952214"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="6578e-103">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="6578e-103">Create accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="6578e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6578e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6578e-105">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)создайте новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6578e-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6578e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6578e-106">Permissions</span></span>

<span data-ttu-id="6578e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6578e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6578e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6578e-109">Permission type</span></span>                        | <span data-ttu-id="6578e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6578e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6578e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6578e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6578e-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6578e-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="6578e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6578e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6578e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6578e-114">Not supported.</span></span> |
| <span data-ttu-id="6578e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6578e-115">Application</span></span>                            | <span data-ttu-id="6578e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6578e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6578e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6578e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="6578e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6578e-118">Request headers</span></span>

| <span data-ttu-id="6578e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6578e-119">Name</span></span>          | <span data-ttu-id="6578e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6578e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6578e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6578e-121">Authorization</span></span> | <span data-ttu-id="6578e-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="6578e-122">Bearer \{token\}.</span></span> <span data-ttu-id="6578e-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6578e-123">Required.</span></span> |
| <span data-ttu-id="6578e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6578e-124">Content-Type</span></span>  | <span data-ttu-id="6578e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6578e-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6578e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6578e-127">Request body</span></span>

<span data-ttu-id="6578e-128">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6578e-128">In the request body, supply a JSON representation of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6578e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6578e-129">Response</span></span>

<span data-ttu-id="6578e-130">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6578e-130">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6578e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6578e-131">Examples</span></span>

### <a name="example-1-create-a-direct-assignment-policy"></a><span data-ttu-id="6578e-132">Пример 1: Создание политики прямого назначения</span><span class="sxs-lookup"><span data-stu-id="6578e-132">Example 1: Create a direct assignment policy</span></span>

<span data-ttu-id="6578e-133">Политика прямого назначения полезна, если доступ к запросам на назначение пакетов будет создавать только администратором, а не самим пользователями.</span><span class="sxs-lookup"><span data-stu-id="6578e-133">A direct assignment policy is useful when access package assignment requests will only be created by an administrator, not by users themselves.</span></span>

#### <a name="request"></a><span data-ttu-id="6578e-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6578e-134">Request</span></span>

<span data-ttu-id="6578e-135">В приведенном ниже примере показан запрос на создание политики назначения пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="6578e-135">The following example shows a request to create an access package assignment policy.</span></span> <span data-ttu-id="6578e-136">В этой политике пользователи, которые не могут запрашивать, не требуют утверждения и не просматривают проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="6578e-136">In this policy, no users can request, no approval is required, and there are no access reviews.</span></span>

# <a name="http"></a>[<span data-ttu-id="6578e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6578e-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6578e-138">C#</span><span class="sxs-lookup"><span data-stu-id="6578e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6578e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6578e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6578e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6578e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6578e-141">Java</span><span class="sxs-lookup"><span data-stu-id="6578e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6578e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="6578e-142">Response</span></span>

<span data-ttu-id="6578e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6578e-143">The following is an example of the response.</span></span>

> <span data-ttu-id="6578e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6578e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a><span data-ttu-id="6578e-146">Пример 2: Создание политики для пользователей из других организаций для запроса</span><span class="sxs-lookup"><span data-stu-id="6578e-146">Example 2: Create a policy for users from other organizations to request</span></span>

<span data-ttu-id="6578e-147">В приведенном ниже примере показана более сложная политика с разутверждениями и проверками доступа в двух стадиях.</span><span class="sxs-lookup"><span data-stu-id="6578e-147">The following example shows a more complex policy with two-stage approvals and access reviews.</span></span>

#### <a name="request"></a><span data-ttu-id="6578e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6578e-148">Request</span></span>

<span data-ttu-id="6578e-149">Ниже приведен пример запроса на создание политики назначения пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="6578e-149">The following is an example of the request to create an access package assignment policy.</span></span> 


# <a name="http"></a>[<span data-ttu-id="6578e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6578e-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6578e-151">C#</span><span class="sxs-lookup"><span data-stu-id="6578e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6578e-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6578e-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6578e-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6578e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6578e-154">Java</span><span class="sxs-lookup"><span data-stu-id="6578e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-multistage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="6578e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6578e-155">Response</span></span>

<span data-ttu-id="6578e-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6578e-156">The following is an example of the response.</span></span>

> <span data-ttu-id="6578e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6578e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


