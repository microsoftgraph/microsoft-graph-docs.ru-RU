---
title: Создание Акцесспаккажеассигнментполици
description: Используйте этот API для создания нового Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c58e9e41a5b3ed89e3c4fb1a217a8470e947aa94
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534424"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="51746-103">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="51746-103">Create accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="51746-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="51746-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51746-105">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)создайте новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="51746-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51746-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51746-106">Permissions</span></span>

<span data-ttu-id="51746-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51746-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51746-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51746-109">Permission type</span></span>                        | <span data-ttu-id="51746-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51746-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51746-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51746-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="51746-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51746-112">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="51746-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51746-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51746-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51746-114">Not supported.</span></span> |
| <span data-ttu-id="51746-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51746-115">Application</span></span>                            | <span data-ttu-id="51746-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51746-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51746-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51746-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="51746-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51746-118">Request headers</span></span>

| <span data-ttu-id="51746-119">Имя</span><span class="sxs-lookup"><span data-stu-id="51746-119">Name</span></span>          | <span data-ttu-id="51746-120">Описание</span><span class="sxs-lookup"><span data-stu-id="51746-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="51746-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51746-121">Authorization</span></span> | <span data-ttu-id="51746-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="51746-122">Bearer \{token\}.</span></span> <span data-ttu-id="51746-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="51746-123">Required.</span></span> |
| <span data-ttu-id="51746-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51746-124">Content-Type</span></span>  | <span data-ttu-id="51746-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51746-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51746-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="51746-127">Request body</span></span>

<span data-ttu-id="51746-128">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51746-128">In the request body, supply a JSON representation of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="51746-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="51746-129">Response</span></span>

<span data-ttu-id="51746-130">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51746-130">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51746-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="51746-131">Examples</span></span>

### <a name="example-1-create-a-direct-assignment-policy"></a><span data-ttu-id="51746-132">Пример 1: Создание политики прямого назначения</span><span class="sxs-lookup"><span data-stu-id="51746-132">Example 1: Create a direct assignment policy</span></span>

<span data-ttu-id="51746-133">Политика прямого назначения полезна, если доступ к запросам на назначение пакетов будет создавать только администратором, а не самим пользователями.</span><span class="sxs-lookup"><span data-stu-id="51746-133">A direct assignment policy is useful when access package assignment requests will only be created by an administrator, not by users themselves.</span></span>

#### <a name="request"></a><span data-ttu-id="51746-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="51746-134">Request</span></span>

<span data-ttu-id="51746-135">В приведенном ниже примере показан запрос на создание политики назначения пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="51746-135">The following example shows a request to create an access package assignment policy.</span></span> <span data-ttu-id="51746-136">В этой политике пользователи, которые не могут запрашивать, не требуют утверждения и не просматривают проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="51746-136">In this policy, no users can request, no approval is required, and there are no access reviews.</span></span>

# <a name="http"></a>[<span data-ttu-id="51746-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="51746-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="51746-138">C#</span><span class="sxs-lookup"><span data-stu-id="51746-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51746-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51746-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51746-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51746-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="51746-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="51746-141">Response</span></span>

<span data-ttu-id="51746-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51746-142">The following is an example of the response.</span></span>

> <span data-ttu-id="51746-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51746-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-policy-for-users-from-other-organizations-to-request"></a><span data-ttu-id="51746-145">Пример 2: Создание политики для пользователей из других организаций для запроса</span><span class="sxs-lookup"><span data-stu-id="51746-145">Example 2: Create a policy for users from other organizations to request</span></span>

<span data-ttu-id="51746-146">В приведенном ниже примере показана более сложная политика с разутверждениями и проверками доступа в двух стадиях.</span><span class="sxs-lookup"><span data-stu-id="51746-146">The following example shows a more complex policy with two-stage approvals and access reviews.</span></span>

#### <a name="request"></a><span data-ttu-id="51746-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="51746-147">Request</span></span>

<span data-ttu-id="51746-148">Ниже приведен пример запроса на создание политики назначения пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="51746-148">The following is an example of the request to create an access package assignment policy.</span></span> 

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


#### <a name="response"></a><span data-ttu-id="51746-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="51746-149">Response</span></span>

<span data-ttu-id="51746-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51746-150">The following is an example of the response.</span></span>

> <span data-ttu-id="51746-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51746-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
