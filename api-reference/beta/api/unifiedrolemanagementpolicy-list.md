---
title: Список унифицированныхRoleManagementPolicies
description: Получите список объектов unifiedRoleManagementPolicy и их свойств.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 051cb20b85f44282b82a3e4c0a855f627d517e4f
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334642"
---
# <a name="list-unifiedrolemanagementpolicies"></a><span data-ttu-id="3b828-103">Список унифицированныхRoleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="3b828-103">List unifiedRoleManagementPolicies</span></span>
<span data-ttu-id="3b828-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b828-105">Получите список объектов [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="3b828-105">Get a list of the [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b828-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b828-106">Permissions</span></span>
<span data-ttu-id="3b828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b828-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b828-109">Permission type</span></span>|<span data-ttu-id="3b828-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b828-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b828-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b828-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b828-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="3b828-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="3b828-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b828-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b828-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3b828-114">Not supported</span></span>|
|<span data-ttu-id="3b828-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3b828-115">Application</span></span>|<span data-ttu-id="3b828-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="3b828-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b828-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b828-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b828-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b828-118">Optional query parameters</span></span>
<span data-ttu-id="3b828-119">Этот метод поддерживает все параметры запроса OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="3b828-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3b828-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3b828-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b828-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b828-121">Request headers</span></span>
|<span data-ttu-id="3b828-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3b828-122">Name</span></span>|<span data-ttu-id="3b828-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3b828-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3b828-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b828-124">Authorization</span></span>|<span data-ttu-id="3b828-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b828-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b828-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b828-127">Request body</span></span>
<span data-ttu-id="3b828-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b828-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b828-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b828-129">Response</span></span>

<span data-ttu-id="3b828-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3b828-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b828-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3b828-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3b828-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b828-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3b828-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b828-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies
```
# <a name="c"></a>[<span data-ttu-id="3b828-134">C#</span><span class="sxs-lookup"><span data-stu-id="3b828-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b828-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b828-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b828-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b828-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3b828-137">Java</span><span class="sxs-lookup"><span data-stu-id="3b828-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3b828-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b828-138">Response</span></span>
<span data-ttu-id="3b828-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3b828-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "displayName": "Policy1",
      "description": "Policy for all privileged admins",
      "isOrganizationDefault": false,
      "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "scopeType": "subscription",
      "lastModifiedDateTime": "2020-09-09T21:35:27.91Z",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identity"
      }
    }
  ]
}
```

