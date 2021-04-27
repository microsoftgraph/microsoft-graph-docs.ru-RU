---
title: Get unifiedRoleDefinition
description: Извлечение свойств и связей объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 367a88bc2563f8b62f66d812668871b1d84fb4b8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053407"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="10ddd-103">Get unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="10ddd-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="10ddd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ddd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10ddd-105">Извлечение свойств и связей объекта [unifiedRoleDefinition.](../resources/unifiedRoleDefinition.md)</span><span class="sxs-lookup"><span data-stu-id="10ddd-105">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="10ddd-106">В настоящее время "каталог" является единственным поддерживаемой приложением RBAC.</span><span class="sxs-lookup"><span data-stu-id="10ddd-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="10ddd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10ddd-107">Permissions</span></span>

<span data-ttu-id="10ddd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10ddd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ddd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10ddd-110">Permission type</span></span>      | <span data-ttu-id="10ddd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10ddd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10ddd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10ddd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10ddd-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10ddd-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10ddd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10ddd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10ddd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10ddd-115">Not supported.</span></span>    |
|<span data-ttu-id="10ddd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="10ddd-116">Application</span></span> | <span data-ttu-id="10ddd-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10ddd-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10ddd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10ddd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10ddd-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10ddd-119">Optional query parameters</span></span>

<span data-ttu-id="10ddd-120">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10ddd-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="10ddd-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="10ddd-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="10ddd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10ddd-122">Request headers</span></span>

| <span data-ttu-id="10ddd-123">Имя</span><span class="sxs-lookup"><span data-stu-id="10ddd-123">Name</span></span>      |<span data-ttu-id="10ddd-124">Описание</span><span class="sxs-lookup"><span data-stu-id="10ddd-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10ddd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10ddd-125">Authorization</span></span> | <span data-ttu-id="10ddd-126">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="10ddd-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="10ddd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10ddd-127">Request body</span></span>

<span data-ttu-id="10ddd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10ddd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ddd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ddd-129">Response</span></span>

<span data-ttu-id="10ddd-130">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="10ddd-130">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10ddd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="10ddd-131">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role"></a><span data-ttu-id="10ddd-132">Пример 1. Определение настраиваемой роли</span><span class="sxs-lookup"><span data-stu-id="10ddd-132">Example 1: Get the definition of a custom role</span></span>

#### <a name="request"></a><span data-ttu-id="10ddd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ddd-133">Request</span></span>

<span data-ttu-id="10ddd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ddd-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="10ddd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="10ddd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="10ddd-136">C#</span><span class="sxs-lookup"><span data-stu-id="10ddd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10ddd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10ddd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10ddd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10ddd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10ddd-139">Java</span><span class="sxs-lookup"><span data-stu-id="10ddd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10ddd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ddd-140">Response</span></span>

<span data-ttu-id="10ddd-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10ddd-141">The following is an example of the response.</span></span>

> <span data-ttu-id="10ddd-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10ddd-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "429c3819-053d-4250-9926-4c7dcb18ae17",
    "description": "Allows reading Application Registrations",
    "displayName": "Application Registration Reader",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "f189965f-f560-4c59-9101-933d4c87a91a",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/allProperties/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f189965f-f560-4c59-9101-933d4c87a91a')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

### <a name="example-2-get-the-definition-of-a-built-in-role"></a><span data-ttu-id="10ddd-143">Пример 2. Определение встроенной роли</span><span class="sxs-lookup"><span data-stu-id="10ddd-143">Example 2: Get the definition of a built-in role</span></span>

#### <a name="request"></a><span data-ttu-id="10ddd-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ddd-144">Request</span></span>

<span data-ttu-id="10ddd-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ddd-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="10ddd-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="10ddd-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="10ddd-147">C#</span><span class="sxs-lookup"><span data-stu-id="10ddd-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10ddd-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10ddd-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10ddd-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10ddd-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10ddd-150">Java</span><span class="sxs-lookup"><span data-stu-id="10ddd-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="10ddd-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ddd-151">Response</span></span>

<span data-ttu-id="10ddd-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10ddd-152">The following is an example of the response.</span></span>

> <span data-ttu-id="10ddd-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10ddd-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "description": "Members of this role can create/manage groups, create/manage groups settings like naming and expiration policies, and view groups activity and audit reports.",
    "displayName": "Groups Administrator",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "version": "1",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/groups/assignLicense",
                "microsoft.directory/groups/create",
                "microsoft.directory/groups/delete",
                "microsoft.directory/groups/hiddenMembers/read",
                "microsoft.directory/groups/reprocessLicenseAssignment",
                "microsoft.directory/groups/restore",
                "microsoft.directory/groups/basic/update",
                "microsoft.directory/groups/classification/update",
                "microsoft.directory/groups/dynamicMembershipRule/update",
                "microsoft.directory/groups/groupType/update",
                "microsoft.directory/groups/members/update",
                "microsoft.directory/groups/owners/update",
                "microsoft.directory/groups/settings/update",
                "microsoft.directory/groups/visibility/update",
                "microsoft.azure.serviceHealth/allEntities/allTasks",
                "microsoft.azure.supportTickets/allEntities/allTasks",
                "microsoft.office365.serviceHealth/allEntities/allTasks",
                "microsoft.office365.supportTickets/allEntities/allTasks",
                "microsoft.office365.webPortal/allEntities/standard/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('fdd7a751-b60b-444a-984c-02652fe8fa1c')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": [
        {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
        }
    ]
}
```
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="10ddd-154">Пример 3. Определение встроенной роли Azure AD и $expand роли, которую она наследует</span><span class="sxs-lookup"><span data-stu-id="10ddd-154">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="10ddd-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="10ddd-155">Request</span></span>

<span data-ttu-id="10ddd-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10ddd-156">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="10ddd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="10ddd-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="10ddd-158">C#</span><span class="sxs-lookup"><span data-stu-id="10ddd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10ddd-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10ddd-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10ddd-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10ddd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10ddd-161">Java</span><span class="sxs-lookup"><span data-stu-id="10ddd-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="10ddd-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="10ddd-162">Response</span></span>

<span data-ttu-id="10ddd-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10ddd-163">The following is an example of the response.</span></span>

> <span data-ttu-id="10ddd-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10ddd-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions(inheritsPermissionsFrom())/$entity",
    "id": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "description": "Members of this role can create/manage groups, create/manage groups settings like naming and expiration policies, and view groups activity and audit reports.",
    "displayName": "Groups Administrator",
    "isBuiltIn": true,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    "version": "1",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/groups/assignLicense",
                "microsoft.directory/groups/create",
                "microsoft.directory/groups/delete",
                "microsoft.directory/groups/hiddenMembers/read",
                "microsoft.directory/groups/reprocessLicenseAssignment",
                "microsoft.directory/groups/restore",
                "microsoft.directory/groups/basic/update",
                "microsoft.directory/groups/classification/update",
                "microsoft.directory/groups/dynamicMembershipRule/update",
                "microsoft.directory/groups/groupType/update",
                "microsoft.directory/groups/members/update",
                "microsoft.directory/groups/owners/update",
                "microsoft.directory/groups/settings/update",
                "microsoft.directory/groups/visibility/update",
                "microsoft.azure.serviceHealth/allEntities/allTasks",
                "microsoft.azure.supportTickets/allEntities/allTasks",
                "microsoft.office365.serviceHealth/allEntities/allTasks",
                "microsoft.office365.supportTickets/allEntities/allTasks",
                "microsoft.office365.webPortal/allEntities/standard/read"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('fdd7a751-b60b-444a-984c-02652fe8fa1c')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": [
        {
            "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
            "displayName": "Directory Readers",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/administrativeUnits/standard/read",
                        "microsoft.directory/administrativeUnits/members/read",
                        "microsoft.directory/applications/standard/read",
                        "microsoft.directory/applications/owners/read",
                        "microsoft.directory/applications/policies/read",
                        "microsoft.directory/contacts/standard/read",
                        "microsoft.directory/contacts/memberOf/read",
                        "microsoft.directory/contracts/standard/read",
                        "microsoft.directory/devices/standard/read",
                        "microsoft.directory/devices/memberOf/read",
                        "microsoft.directory/devices/registeredOwners/read",
                        "microsoft.directory/devices/registeredUsers/read",
                        "microsoft.directory/directoryRoles/standard/read",
                        "microsoft.directory/directoryRoles/eligibleMembers/read",
                        "microsoft.directory/directoryRoles/members/read",
                        "microsoft.directory/domains/standard/read",
                        "microsoft.directory/groups/standard/read",
                        "microsoft.directory/groups/appRoleAssignments/read",
                        "microsoft.directory/groups/memberOf/read",
                        "microsoft.directory/groups/members/read",
                        "microsoft.directory/groups/owners/read",
                        "microsoft.directory/groups/settings/read",
                        "microsoft.directory/groupSettings/standard/read",
                        "microsoft.directory/groupSettingTemplates/standard/read",
                        "microsoft.directory/oAuth2PermissionGrants/standard/read",
                        "microsoft.directory/organization/standard/read",
                        "microsoft.directory/organization/trustedCAsForPasswordlessAuth/read",
                        "microsoft.directory/applicationPolicies/standard/read",
                        "microsoft.directory/roleAssignments/standard/read",
                        "microsoft.directory/roleDefinitions/standard/read",
                        "microsoft.directory/servicePrincipals/appRoleAssignedTo/read",
                        "microsoft.directory/servicePrincipals/appRoleAssignments/read",
                        "microsoft.directory/servicePrincipals/standard/read",
                        "microsoft.directory/servicePrincipals/memberOf/read",
                        "microsoft.directory/servicePrincipals/oAuth2PermissionGrants/read",
                        "microsoft.directory/servicePrincipals/owners/read",
                        "microsoft.directory/servicePrincipals/ownedObjects/read",
                        "microsoft.directory/servicePrincipals/policies/read",
                        "microsoft.directory/subscribedSkus/standard/read",
                        "microsoft.directory/users/standard/read",
                        "microsoft.directory/users/appRoleAssignments/read",
                        "microsoft.directory/users/directReports/read",
                        "microsoft.directory/users/manager/read",
                        "microsoft.directory/users/memberOf/read",
                        "microsoft.directory/users/oAuth2PermissionGrants/read",
                        "microsoft.directory/users/ownedDevices/read",
                        "microsoft.directory/users/ownedObjects/read",
                        "microsoft.directory/users/registeredDevices/read"
                    ],
                    "condition": null
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


