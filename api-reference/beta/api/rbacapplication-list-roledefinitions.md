---
title: Список унифицированныхRoleDefinitions
description: Получите список объектов unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 595e88c54377f88fb4a0f239ab07483d4d5251aa
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334628"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="ebe42-103">Список унифицированныхRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ebe42-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="ebe42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebe42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebe42-105">Получите список объектов [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="ebe42-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for an RBAC provider.</span></span>

<span data-ttu-id="ebe42-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="ebe42-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="ebe42-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="ebe42-107">cloud PC</span></span> 
- <span data-ttu-id="ebe42-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="ebe42-108">device management (Intune)</span></span>
- <span data-ttu-id="ebe42-109">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="ebe42-109">directory (Azure AD)</span></span> 
- <span data-ttu-id="ebe42-110">управление правами (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="ebe42-110">entitlement management (Azure AD)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ebe42-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe42-111">Permissions</span></span>

<span data-ttu-id="ebe42-112">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ebe42-112">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="ebe42-113">Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="ebe42-113">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="ebe42-114">Поставщик облачных ПК</span><span class="sxs-lookup"><span data-stu-id="ebe42-114">For Cloud PC provider</span></span>

|<span data-ttu-id="ebe42-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe42-115">Permission type</span></span>      | <span data-ttu-id="ebe42-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebe42-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebe42-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebe42-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="ebe42-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe42-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="ebe42-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebe42-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebe42-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe42-120">Not supported.</span></span>    |
|<span data-ttu-id="ebe42-121">Приложение</span><span class="sxs-lookup"><span data-stu-id="ebe42-121">Application</span></span> | <span data-ttu-id="ebe42-122">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe42-122">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="ebe42-123">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="ebe42-123">For Device management (Intune) provider</span></span>

|<span data-ttu-id="ebe42-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe42-124">Permission type</span></span>      | <span data-ttu-id="ebe42-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebe42-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebe42-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebe42-126">Delegated (work or school account)</span></span> |  <span data-ttu-id="ebe42-127">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe42-127">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="ebe42-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebe42-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebe42-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe42-129">Not supported.</span></span>    |
|<span data-ttu-id="ebe42-130">Приложение</span><span class="sxs-lookup"><span data-stu-id="ebe42-130">Application</span></span> | <span data-ttu-id="ebe42-131">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe42-131">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="ebe42-132">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="ebe42-132">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="ebe42-133">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe42-133">Permission type</span></span>      | <span data-ttu-id="ebe42-134">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebe42-134">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebe42-135">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebe42-135">Delegated (work or school account)</span></span> |  <span data-ttu-id="ebe42-136">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ebe42-136">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="ebe42-137">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebe42-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebe42-138">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe42-138">Not supported.</span></span>    |
|<span data-ttu-id="ebe42-139">Приложение</span><span class="sxs-lookup"><span data-stu-id="ebe42-139">Application</span></span> | <span data-ttu-id="ebe42-140">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe42-140">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="ebe42-141">Поставщик прав на управление правами</span><span class="sxs-lookup"><span data-stu-id="ebe42-141">For Entitlement management provider</span></span>

|<span data-ttu-id="ebe42-142">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe42-142">Permission type</span></span>      | <span data-ttu-id="ebe42-143">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebe42-143">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebe42-144">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebe42-144">Delegated (work or school account)</span></span> |  <span data-ttu-id="ebe42-145">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe42-145">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="ebe42-146">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebe42-146">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebe42-147">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe42-147">Not supported.</span></span>    |
|<span data-ttu-id="ebe42-148">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebe42-148">Application</span></span> | <span data-ttu-id="ebe42-149">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebe42-149">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebe42-150">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebe42-150">HTTP request</span></span>

<span data-ttu-id="ebe42-151">Список определений ролей для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="ebe42-151">To list role definitions for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions
```

<span data-ttu-id="ebe42-152">Список определений ролей для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="ebe42-152">To list role definitions for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="ebe42-153">Список определений ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="ebe42-153">To list role definitions for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/directory/roleDefinitions
```

<span data-ttu-id="ebe42-154">Список определений ролей для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="ebe42-154">To list role definitions for the entitlement management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/entitlementManagement/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ebe42-155">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebe42-155">Optional query parameters</span></span>
<span data-ttu-id="ebe42-156">Этот метод поддерживает параметр `$filter` запроса `id` и `displayName` `isBuiltIn` свойства.</span><span class="sxs-lookup"><span data-stu-id="ebe42-156">This method supports `$filter` query parameter on `id`, `displayName`, and `isBuiltIn` properties.</span></span> <span data-ttu-id="ebe42-157">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ebe42-157">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebe42-158">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebe42-158">Request headers</span></span>

| <span data-ttu-id="ebe42-159">Имя</span><span class="sxs-lookup"><span data-stu-id="ebe42-159">Name</span></span>      |<span data-ttu-id="ebe42-160">Описание</span><span class="sxs-lookup"><span data-stu-id="ebe42-160">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ebe42-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebe42-161">Authorization</span></span> | <span data-ttu-id="ebe42-162">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ebe42-162">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebe42-163">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebe42-163">Request body</span></span>

<span data-ttu-id="ebe42-164">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebe42-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebe42-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebe42-165">Response</span></span>

<span data-ttu-id="ebe42-166">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ebe42-166">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ebe42-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="ebe42-167">Examples</span></span>

### <a name="example-1-list-role-definitions-for-a-directory-provider"></a><span data-ttu-id="ebe42-168">Пример 1. Список определений ролей для поставщика каталогов</span><span class="sxs-lookup"><span data-stu-id="ebe42-168">Example 1: List role definitions for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="ebe42-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebe42-169">Request</span></span>

<span data-ttu-id="ebe42-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebe42-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ebe42-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebe42-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_directory"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="ebe42-172">C#</span><span class="sxs-lookup"><span data-stu-id="ebe42-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebe42-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebe42-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebe42-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebe42-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebe42-175">Java</span><span class="sxs-lookup"><span data-stu-id="ebe42-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ebe42-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebe42-176">Response</span></span>

<span data-ttu-id="ebe42-177">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ebe42-177">The following is an example of the response.</span></span>

> <span data-ttu-id="ebe42-178">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebe42-178">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-role-definitions-for-a-cloud-pc-provider"></a><span data-ttu-id="ebe42-179">Пример 2. Список определений ролей для поставщика облачных ПК</span><span class="sxs-lookup"><span data-stu-id="ebe42-179">Example 2: List role definitions for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="ebe42-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebe42-180">Request</span></span>

<span data-ttu-id="ebe42-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebe42-181">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ebe42-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebe42-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_cloudpc"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions
```
# <a name="c"></a>[<span data-ttu-id="ebe42-183">C#</span><span class="sxs-lookup"><span data-stu-id="ebe42-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebe42-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebe42-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebe42-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebe42-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebe42-186">Java</span><span class="sxs-lookup"><span data-stu-id="ebe42-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roledefinitions-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ebe42-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebe42-187">Response</span></span>

<span data-ttu-id="ebe42-188">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ebe42-188">The following is an example of the response.</span></span>

> <span data-ttu-id="ebe42-189">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebe42-189">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-list-role-definitions-for-the-entitlement-management-provider"></a><span data-ttu-id="ebe42-190">Пример 3. Список определений ролей для поставщика управления правами</span><span class="sxs-lookup"><span data-stu-id="ebe42-190">Example 3: List role definitions for the entitlement management provider</span></span>

#### <a name="request"></a><span data-ttu-id="ebe42-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebe42-191">Request</span></span>

<span data-ttu-id="ebe42-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebe42-192">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_roledefinitions_entitlementmanagement"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleDefinitions
```

#### <a name="response"></a><span data-ttu-id="ebe42-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebe42-193">Response</span></span>

<span data-ttu-id="ebe42-194">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ebe42-194">The following is an example of the response.</span></span>

> <span data-ttu-id="ebe42-195">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebe42-195">**Note:** The response object shown here might be shortened for readability.</span></span>

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


