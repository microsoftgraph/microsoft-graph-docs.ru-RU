---
title: Список унифицированныхRoleManagementPolicyAssignments
description: Получите список объектов unifiedRoleManagementPolicyAssignment и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3c9f6ed4d21a49a3b17bb22340f4d8350f1471bc
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475446"
---
# <a name="list-unifiedrolemanagementpolicyassignments"></a><span data-ttu-id="90cfe-103">Список унифицированныхRoleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="90cfe-103">List unifiedRoleManagementPolicyAssignments</span></span>
<span data-ttu-id="90cfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90cfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90cfe-105">Получите список объектов [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="90cfe-105">Get a list of the [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="90cfe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90cfe-106">Permissions</span></span>
<span data-ttu-id="90cfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90cfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90cfe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90cfe-109">Permission type</span></span>|<span data-ttu-id="90cfe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90cfe-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90cfe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90cfe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90cfe-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="90cfe-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="90cfe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90cfe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90cfe-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="90cfe-114">Not supported</span></span>|
|<span data-ttu-id="90cfe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90cfe-115">Application</span></span>|<span data-ttu-id="90cfe-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="90cfe-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="90cfe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90cfe-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicyAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90cfe-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="90cfe-118">Optional query parameters</span></span>
<span data-ttu-id="90cfe-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="90cfe-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="90cfe-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="90cfe-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="90cfe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90cfe-121">Request headers</span></span>
|<span data-ttu-id="90cfe-122">Имя</span><span class="sxs-lookup"><span data-stu-id="90cfe-122">Name</span></span>|<span data-ttu-id="90cfe-123">Описание</span><span class="sxs-lookup"><span data-stu-id="90cfe-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="90cfe-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90cfe-124">Authorization</span></span>|<span data-ttu-id="90cfe-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90cfe-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="90cfe-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90cfe-127">Request body</span></span>
<span data-ttu-id="90cfe-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90cfe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90cfe-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90cfe-129">Response</span></span>

<span data-ttu-id="90cfe-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="90cfe-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90cfe-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="90cfe-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90cfe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="90cfe-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="90cfe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="90cfe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicyAssignments
```
# <a name="c"></a>[<span data-ttu-id="90cfe-134">C#</span><span class="sxs-lookup"><span data-stu-id="90cfe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90cfe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90cfe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90cfe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90cfe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90cfe-137">Java</span><span class="sxs-lookup"><span data-stu-id="90cfe-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="90cfe-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="90cfe-138">Response</span></span>
<span data-ttu-id="90cfe-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="90cfe-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyAssignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
      "policyId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
      "scopeId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6",
      "scopeType": "subscription",
      "roleDefinitionId": "d6e4112f-112f-d6e4-2f11-e4d62f11e4d6"
    }
  ]
}
```

