---
title: Список унифицированныхRoleDefinitions
description: Получите список объектов unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3b49093e1eeba4618bc36737e789a9484c5a5142
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317212"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="06d96-103">Список унифицированныхRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="06d96-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="06d96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06d96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06d96-105">Получите список объектов [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="06d96-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for an RBAC provider.</span></span>

<span data-ttu-id="06d96-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="06d96-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="06d96-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="06d96-107">cloud PC</span></span> 
- <span data-ttu-id="06d96-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="06d96-108">device management (Intune)</span></span>
- <span data-ttu-id="06d96-109">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="06d96-109">directory (Azure AD)</span></span> 
- <span data-ttu-id="06d96-110">управление правами (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="06d96-110">entitlement management (Azure AD)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="06d96-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06d96-111">Permissions</span></span>

<span data-ttu-id="06d96-112">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="06d96-112">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="06d96-113">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06d96-113">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="06d96-114">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="06d96-114">Supported provider</span></span>      | <span data-ttu-id="06d96-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06d96-115">Delegated (work or school account)</span></span>  | <span data-ttu-id="06d96-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06d96-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06d96-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06d96-117">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="06d96-118">Облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="06d96-118">Cloud PC</span></span> | <span data-ttu-id="06d96-119">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d96-119">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="06d96-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d96-120">Not supported.</span></span> | <span data-ttu-id="06d96-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d96-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="06d96-122">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="06d96-122">Device management</span></span> | <span data-ttu-id="06d96-123">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d96-123">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="06d96-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d96-124">Not supported.</span></span> | <span data-ttu-id="06d96-125">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d96-125">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="06d96-126">Каталог</span><span class="sxs-lookup"><span data-stu-id="06d96-126">Directory</span></span> | <span data-ttu-id="06d96-127">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06d96-127">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="06d96-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d96-128">Not supported.</span></span>| <span data-ttu-id="06d96-129">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d96-129">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="06d96-130">Управление правами</span><span class="sxs-lookup"><span data-stu-id="06d96-130">Entitlement management</span></span> | <span data-ttu-id="06d96-131">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06d96-131">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="06d96-132">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d96-132">Not supported.</span></span> | <span data-ttu-id="06d96-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06d96-133">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="06d96-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06d96-134">HTTP request</span></span>

<span data-ttu-id="06d96-135">Список определений ролей для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="06d96-135">To list role definitions for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions
```

<span data-ttu-id="06d96-136">Список определений ролей для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="06d96-136">To list role definitions for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="06d96-137">Список определений ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="06d96-137">To list role definitions for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/directory/roleDefinitions
```

<span data-ttu-id="06d96-138">Список определений ролей для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="06d96-138">To list role definitions for the entitlement management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/entitlementManagement/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06d96-139">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06d96-139">Optional query parameters</span></span>
<span data-ttu-id="06d96-140">Этот метод поддерживает параметр `$filter` запроса `id` и `displayName` `isBuiltIn` свойства.</span><span class="sxs-lookup"><span data-stu-id="06d96-140">This method supports `$filter` query parameter on `id`, `displayName`, and `isBuiltIn` properties.</span></span> <span data-ttu-id="06d96-141">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="06d96-141">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="06d96-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06d96-142">Request headers</span></span>

| <span data-ttu-id="06d96-143">Имя</span><span class="sxs-lookup"><span data-stu-id="06d96-143">Name</span></span>      |<span data-ttu-id="06d96-144">Описание</span><span class="sxs-lookup"><span data-stu-id="06d96-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06d96-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06d96-145">Authorization</span></span> | <span data-ttu-id="06d96-146">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="06d96-146">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="06d96-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06d96-147">Request body</span></span>

<span data-ttu-id="06d96-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06d96-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06d96-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d96-149">Response</span></span>

<span data-ttu-id="06d96-150">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="06d96-150">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06d96-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="06d96-151">Examples</span></span>

### <a name="example-1-list-role-definitions-for-a-directory-provider"></a><span data-ttu-id="06d96-152">Пример 1. Список определений ролей для поставщика каталогов</span><span class="sxs-lookup"><span data-stu-id="06d96-152">Example 1: List role definitions for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="06d96-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d96-153">Request</span></span>

<span data-ttu-id="06d96-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06d96-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="06d96-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="06d96-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_directory"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="06d96-156">C#</span><span class="sxs-lookup"><span data-stu-id="06d96-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06d96-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06d96-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06d96-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06d96-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06d96-159">Java</span><span class="sxs-lookup"><span data-stu-id="06d96-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="06d96-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d96-160">Response</span></span>

<span data-ttu-id="06d96-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="06d96-161">The following is an example of the response.</span></span>

> <span data-ttu-id="06d96-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06d96-162">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_directory",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('729827e3-9c14-49f7-bb1b-9608f156bbb8')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f023fd81-a637-4b56-95fd-791ac0226033')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('b0f54661-2d74-4c50-afa3-1ec803f12efe')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        }
    ]
}
```

### <a name="example-2-list-role-definitions-for-a-cloud-pc-provider"></a><span data-ttu-id="06d96-163">Пример 2. Список определений ролей для поставщика облачных ПК</span><span class="sxs-lookup"><span data-stu-id="06d96-163">Example 2: List role definitions for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="06d96-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d96-164">Request</span></span>

<span data-ttu-id="06d96-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06d96-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="06d96-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="06d96-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_cloudpc"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="06d96-167">C#</span><span class="sxs-lookup"><span data-stu-id="06d96-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06d96-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06d96-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06d96-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06d96-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06d96-170">Java</span><span class="sxs-lookup"><span data-stu-id="06d96-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="06d96-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d96-171">Response</span></span>

<span data-ttu-id="06d96-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="06d96-172">The following is an example of the response.</span></span>

> <span data-ttu-id="06d96-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06d96-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_cloudpc",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleDefinitions",
    "value": [
        {
            "id": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "description": "Cloud PC Administrator has read and write access to all Cloud PC features located within the Cloud PC blade.",
            "displayName": "Cloud PC Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "version": null,
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "Microsoft.CloudPC/CloudPCs/Read",
                        "Microsoft.CloudPC/CloudPCs/Reprovision",
                        "Microsoft.CloudPC/DeviceImages/Create",
                        "Microsoft.CloudPC/DeviceImages/Delete",
                        "Microsoft.CloudPC/DeviceImages/Read",
                        "Microsoft.CloudPC/OnPremisesConnections/Create",
                        "Microsoft.CloudPC/OnPremisesConnections/Delete",
                        "Microsoft.CloudPC/OnPremisesConnections/Read",
                        "Microsoft.CloudPC/OnPremisesConnections/Update",
                        "Microsoft.CloudPC/OnPremisesConnections/RunHealthChecks",
                        "Microsoft.CloudPC/OnPremisesConnections/UpdateAdDomainPassword",
                        "Microsoft.CloudPC/ProvisioningPolicies/Assign",
                        "Microsoft.CloudPC/ProvisioningPolicies/Create",
                        "Microsoft.CloudPC/ProvisioningPolicies/Delete",
                        "Microsoft.CloudPC/ProvisioningPolicies/Read",
                        "Microsoft.CloudPC/ProvisioningPolicies/Update",
                        "Microsoft.CloudPC/RoleAssignments/Create",
                        "Microsoft.CloudPC/RoleAssignments/Update",
                        "Microsoft.CloudPC/RoleAssignments/Delete",
                        "Microsoft.CloudPC/Roles/Read"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
            "description": "Cloud PC Reader has read access to all Cloud PC features located within the Cloud PC blade.",
            "displayName": "Cloud PC Reader",
            "isBuiltIn": true,
            "isEnabled": true,
            "resourceScopes": [
                "/"
            ],
            "templateId": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
            "version": null,
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "Microsoft.CloudPC/CloudPCs/Read",
                        "Microsoft.CloudPC/DeviceImages/Read",
                        "Microsoft.CloudPC/OnPremisesConnections/Read",
                        "Microsoft.CloudPC/ProvisioningPolicies/Read",
                        "Microsoft.CloudPC/Roles/Read"
                    ],
                    "condition": null
                }
            ]
        }
    ]
}
```

### <a name="example-3-list-role-definitions-for-the-entitlement-management-provider"></a><span data-ttu-id="06d96-174">Пример 3. Список определений ролей для поставщика управления правами</span><span class="sxs-lookup"><span data-stu-id="06d96-174">Example 3: List role definitions for the entitlement management provider</span></span>

#### <a name="request"></a><span data-ttu-id="06d96-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d96-175">Request</span></span>

<span data-ttu-id="06d96-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06d96-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_entitlementmanagement"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleDefinitions
```

#### <a name="response"></a><span data-ttu-id="06d96-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d96-177">Response</span></span>

<span data-ttu-id="06d96-178">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="06d96-178">The following is an example of the response.</span></span>

> <span data-ttu-id="06d96-179">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06d96-179">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roledefinitions_entitlementmanagement",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleDefinitions",
    "value": [
        {
            "id": "ae79f266-94d4-4dab-b730-feca7e132178",
            "displayName": "Catalog owner",
            "description": "Catalog owner",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "ae79f266-94d4-4dab-b730-feca7e132178",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/allEntities/allTasks"
                    ]
                }
            ]
        },
        {
            "id": "44272f93-9762-48e8-af59-1b5351b1d6b3",
            "displayName": "Catalog reader",
            "description": "Catalog reader",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "44272f93-9762-48e8-af59-1b5351b1d6b3",
            "version": "1.0",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.entitlementManagement/allEntities/Read"
                    ]
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
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


