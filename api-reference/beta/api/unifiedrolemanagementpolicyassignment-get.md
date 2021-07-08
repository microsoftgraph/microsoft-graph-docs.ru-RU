---
title: Get unifiedRoleManagementPolicyAssignment
description: Ознакомьтесь с свойствами и отношениями единого объектаRoleManagementPolicyAssignment.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bd84b1c03c0ffadd8efa4d904bd2c38f9f041434
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334649"
---
# <a name="get-unifiedrolemanagementpolicyassignment"></a><span data-ttu-id="423c4-103">Get unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="423c4-103">Get unifiedRoleManagementPolicyAssignment</span></span>
<span data-ttu-id="423c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="423c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="423c4-105">Ознакомьтесь с свойствами и отношениями единого [объектаRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="423c4-105">Read the properties and relationships of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="423c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="423c4-106">Permissions</span></span>
<span data-ttu-id="423c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="423c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="423c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="423c4-109">Permission type</span></span>|<span data-ttu-id="423c4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="423c4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="423c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="423c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="423c4-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="423c4-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="423c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="423c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="423c4-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="423c4-114">Not supported</span></span>|
|<span data-ttu-id="423c4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="423c4-115">Application</span></span>|<span data-ttu-id="423c4-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="423c4-116">RoleManagement.Read.All, RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="423c4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="423c4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments/{unifiedRoleManagementPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="423c4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="423c4-118">Optional query parameters</span></span>
<span data-ttu-id="423c4-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="423c4-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="423c4-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="423c4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="423c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="423c4-121">Request headers</span></span>
|<span data-ttu-id="423c4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="423c4-122">Name</span></span>|<span data-ttu-id="423c4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="423c4-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="423c4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="423c4-124">Authorization</span></span>|<span data-ttu-id="423c4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="423c4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="423c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="423c4-127">Request body</span></span>
<span data-ttu-id="423c4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="423c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="423c4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="423c4-129">Response</span></span>

<span data-ttu-id="423c4-130">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [унифицированный объектRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="423c4-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="423c4-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="423c4-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="423c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="423c4-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="423c4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="423c4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments/d6e4112f-112f-d6e4-2f11-e4d62f11e4d6
```
# <a name="c"></a>[<span data-ttu-id="423c4-134">C#</span><span class="sxs-lookup"><span data-stu-id="423c4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicyassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="423c4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="423c4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicyassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="423c4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="423c4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicyassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="423c4-137">Java</span><span class="sxs-lookup"><span data-stu-id="423c4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicyassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="423c4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="423c4-138">Response</span></span>
<span data-ttu-id="423c4-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="423c4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "policyId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
    "scopeType": "subscription",
    "roleDefinitionId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"
  }
}
```

