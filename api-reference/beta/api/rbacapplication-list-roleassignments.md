---
title: Список unifiedRoleAssignments
description: Получите список объектов unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5c58ce5123bf7ea3bb29af5b5e67fb5e259d6c75
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351064"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="50869-103">Список unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="50869-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="50869-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50869-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50869-105">Получите список объектов [unifiedRoleAssignment](../resources/unifiedroleassignment.md) для поставщика.</span><span class="sxs-lookup"><span data-stu-id="50869-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

<span data-ttu-id="50869-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="50869-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="50869-107">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="50869-107">directory (Azure AD)</span></span>
- <span data-ttu-id="50869-108">управление правами (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="50869-108">entitlement management (Azure AD)</span></span>

## <a name="permissions"></a><span data-ttu-id="50869-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50869-109">Permissions</span></span>


<span data-ttu-id="50869-110">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="50869-110">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="50869-111">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50869-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="50869-112">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="50869-112">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="50869-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50869-113">Permission type</span></span>      | <span data-ttu-id="50869-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50869-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50869-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50869-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="50869-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50869-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="50869-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50869-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50869-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50869-118">Not supported.</span></span>    |
|<span data-ttu-id="50869-119">Application</span><span class="sxs-lookup"><span data-stu-id="50869-119">Application</span></span> | <span data-ttu-id="50869-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50869-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="50869-121">Поставщик прав на управление правами</span><span class="sxs-lookup"><span data-stu-id="50869-121">For Entitlement management provider</span></span>

|<span data-ttu-id="50869-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50869-122">Permission type</span></span>      | <span data-ttu-id="50869-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50869-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50869-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50869-124">Delegated (work or school account)</span></span> |  <span data-ttu-id="50869-125">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50869-125">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="50869-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50869-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50869-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50869-127">Not supported.</span></span>    |
|<span data-ttu-id="50869-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50869-128">Application</span></span> | <span data-ttu-id="50869-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50869-129">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="50869-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50869-130">HTTP request</span></span>

<span data-ttu-id="50869-131">Список назначений ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="50869-131">To list role assignments for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments?$filter=principalId eq '{principal id}'

GET /roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '{roleDefinition id}'
```

<span data-ttu-id="50869-132">Список назначений ролей для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="50869-132">To list role assignments for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments?$filter=principalId eq '{principal id}'

GET /roleManagement/entitlementManagement/roleAssignments?$filter=roleDefinitionId eq '{roleDefinition id}'
```

## <a name="query-parameters"></a><span data-ttu-id="50869-133">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="50869-133">Query parameters</span></span>

<span data-ttu-id="50869-134">Эта операция требует `$filter` параметра запроса.</span><span class="sxs-lookup"><span data-stu-id="50869-134">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="50869-135">Вы можете фильтровать свойства `roleDefinitionId` или `principalId` свойства.</span><span class="sxs-lookup"><span data-stu-id="50869-135">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="50869-136">Свойство `roleDefinitionId` может быть как ИД объекта роли, так и объектом шаблона ролей.</span><span class="sxs-lookup"><span data-stu-id="50869-136">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="50869-137">Параметр `$expand` запроса также поддерживается в **основном**.</span><span class="sxs-lookup"><span data-stu-id="50869-137">The `$expand` query parameter is also supported on **principal**.</span></span> <span data-ttu-id="50869-138">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="50869-138">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="50869-139">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50869-139">Request headers</span></span>

| <span data-ttu-id="50869-140">Имя</span><span class="sxs-lookup"><span data-stu-id="50869-140">Name</span></span>      |<span data-ttu-id="50869-141">Описание</span><span class="sxs-lookup"><span data-stu-id="50869-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50869-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="50869-142">Authorization</span></span> | <span data-ttu-id="50869-143">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="50869-143">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="50869-144">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="50869-144">Request body</span></span>

<span data-ttu-id="50869-145">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50869-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50869-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="50869-146">Response</span></span>

<span data-ttu-id="50869-147">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="50869-147">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50869-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="50869-148">Examples</span></span>

### <a name="example-1-request-using-filter-on-role-definition-id-and-expand-principal"></a><span data-ttu-id="50869-149">Пример 1. Запрос $filter на ID определения ролей и расширение основного</span><span class="sxs-lookup"><span data-stu-id="50869-149">Example 1: Request using $filter on role definition ID and expand principal</span></span>

#### <a name="request"></a><span data-ttu-id="50869-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="50869-150">Request</span></span>

<span data-ttu-id="50869-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50869-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50869-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="50869-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=principal
```
# <a name="c"></a>[<span data-ttu-id="50869-153">C#</span><span class="sxs-lookup"><span data-stu-id="50869-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50869-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50869-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50869-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50869-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50869-156">Java</span><span class="sxs-lookup"><span data-stu-id="50869-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="50869-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="50869-157">Response</span></span>

<span data-ttu-id="50869-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="50869-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments(principal())",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMmO4KwRqtpKkUWt3wOYIz4-1",
            "principalId": "ace08ec9-aa11-4ada-9145-addf0398233e",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "ace08ec9-aa11-4ada-9145-addf0398233e",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": "Redmond",
                "createdDateTime": "2019-02-22T20:29:07Z",
                "creationType": null,
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": "US",
                "department": "Office of the CEO",
                "displayName": "Joey Cruz",
                "employeeId": null,
                "faxNumber": null,
                "givenName": "Joey",
                "imAddresses": [
                    "joeyc@woodgrove.ms"
                ],
                "infoCatalogs": [],
                "isResourceAccount": null,
                "jobTitle": "Chief Security Officer",
                "legalAgeGroupClassification": null,
                "mail": "joeyc@woodgrove.ms",
                "mailNickname": "joeyc",
                "mobilePhone": null,
                "onPremisesDistinguishedName": null,
                "officeLocation": null,
                "userType": "Member",   

            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEC6Xh29-LklLmYDrOIi9z-E-1",
            "principalId": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-07-18T01:38:36Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Kalyan Krishna",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
    
            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMgc_BA2rIZBuZsM-BSqLdU-1",
            "principalId": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-11-13T21:54:27Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Markie Downing",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
        
            }
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="50869-159">Пример 2. Запрос на использование фильтра для основного ID</span><span class="sxs-lookup"><span data-stu-id="50869-159">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="50869-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="50869-160">Request</span></span>

<span data-ttu-id="50869-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50869-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="50869-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="50869-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter = principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'
```
# <a name="c"></a>[<span data-ttu-id="50869-163">C#</span><span class="sxs-lookup"><span data-stu-id="50869-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50869-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50869-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50869-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50869-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50869-166">Java</span><span class="sxs-lookup"><span data-stu-id="50869-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="50869-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="50869-167">Response</span></span>

<span data-ttu-id="50869-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="50869-168">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEHJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "LJnv8vs6uUa3z6Em7nTEUXJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


