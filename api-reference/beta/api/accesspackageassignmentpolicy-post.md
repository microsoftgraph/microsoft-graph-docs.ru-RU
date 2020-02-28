---
title: Создание Акцесспаккажеассигнментполици
description: Используйте этот API для создания нового Акцесспаккажеассигнментполици.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ffa1b1ac1519c933e9ca352ec90b45a5161d2a43
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331194"
---
# <a name="create-accesspackageassignmentpolicy"></a><span data-ttu-id="9afc1-103">Создание Акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="9afc1-103">Create accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9afc1-104">В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)используйте этот API, чтобы создать новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="9afc1-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), use this API to create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9afc1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9afc1-105">Permissions</span></span>

<span data-ttu-id="9afc1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9afc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9afc1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9afc1-108">Permission type</span></span>                        | <span data-ttu-id="9afc1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9afc1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9afc1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9afc1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9afc1-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9afc1-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="9afc1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9afc1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9afc1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9afc1-113">Not supported.</span></span> |
| <span data-ttu-id="9afc1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9afc1-114">Application</span></span>                            | <span data-ttu-id="9afc1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9afc1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9afc1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9afc1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="request-headers"></a><span data-ttu-id="9afc1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9afc1-117">Request headers</span></span>

| <span data-ttu-id="9afc1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9afc1-118">Name</span></span>          | <span data-ttu-id="9afc1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9afc1-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9afc1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9afc1-120">Authorization</span></span> | <span data-ttu-id="9afc1-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="9afc1-121">Bearer \{token\}.</span></span> <span data-ttu-id="9afc1-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="9afc1-122">Required.</span></span> |
| <span data-ttu-id="9afc1-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9afc1-123">Content-Type</span></span>  | <span data-ttu-id="9afc1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9afc1-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9afc1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9afc1-125">Request body</span></span>

<span data-ttu-id="9afc1-126">В тексте запроса добавьте представление объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9afc1-126">In the request body, supply a JSON representation of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9afc1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9afc1-127">Response</span></span>

<span data-ttu-id="9afc1-128">В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9afc1-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9afc1-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="9afc1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9afc1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9afc1-130">Request</span></span>

<span data-ttu-id="9afc1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9afc1-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9afc1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9afc1-132">HTTP</span></span>](#tab/http)
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
  "isDenyPolicy": false,
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
# <a name="c"></a>[<span data-ttu-id="9afc1-133">C#</span><span class="sxs-lookup"><span data-stu-id="9afc1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9afc1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9afc1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9afc1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9afc1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentpolicy-from-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9afc1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9afc1-136">Response</span></span>

<span data-ttu-id="9afc1-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9afc1-137">The following is an example of the response.</span></span>

> <span data-ttu-id="9afc1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9afc1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "direct assignments by administrator",
  "isDenyPolicy": false
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
