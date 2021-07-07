---
title: Get unifiedRoleDefinition
description: Извлечение свойств и связей объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 07b9aff276c46fbdcca56b365d11e7ac12066408
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317079"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="75f1d-103">Get unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="75f1d-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="75f1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f1d-105">Получите свойства и связи объекта [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="75f1d-105">Get the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="75f1d-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="75f1d-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="75f1d-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="75f1d-107">cloud PC</span></span> 
- <span data-ttu-id="75f1d-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="75f1d-108">device management (Intune)</span></span>
- <span data-ttu-id="75f1d-109">directory (роли каталога Azure AD)</span><span class="sxs-lookup"><span data-stu-id="75f1d-109">directory (Azure AD directory roles)</span></span>
- <span data-ttu-id="75f1d-110">управление правами (управление правами Azure AD)</span><span class="sxs-lookup"><span data-stu-id="75f1d-110">entitlement management (Azure AD entitlement management)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="75f1d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75f1d-111">Permissions</span></span>

<span data-ttu-id="75f1d-112">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="75f1d-112">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="75f1d-113">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75f1d-113">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="75f1d-114">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="75f1d-114">Supported provider</span></span>      | <span data-ttu-id="75f1d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75f1d-115">Delegated (work or school account)</span></span>  | <span data-ttu-id="75f1d-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75f1d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75f1d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75f1d-117">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="75f1d-118">Облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="75f1d-118">Cloud PC</span></span> | <span data-ttu-id="75f1d-119">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f1d-119">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="75f1d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f1d-120">Not supported.</span></span> | <span data-ttu-id="75f1d-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f1d-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="75f1d-122">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="75f1d-122">Device management</span></span> | <span data-ttu-id="75f1d-123">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f1d-123">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="75f1d-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f1d-124">Not supported.</span></span> | <span data-ttu-id="75f1d-125">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f1d-125">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="75f1d-126">Каталог</span><span class="sxs-lookup"><span data-stu-id="75f1d-126">Directory</span></span> | <span data-ttu-id="75f1d-127">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75f1d-127">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="75f1d-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f1d-128">Not supported.</span></span>| <span data-ttu-id="75f1d-129">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f1d-129">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="75f1d-130">Управление правами</span><span class="sxs-lookup"><span data-stu-id="75f1d-130">Entitlement management</span></span> | <span data-ttu-id="75f1d-131">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75f1d-131">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="75f1d-132">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f1d-132">Not supported.</span></span> | <span data-ttu-id="75f1d-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75f1d-133">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75f1d-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75f1d-134">HTTP request</span></span>

<span data-ttu-id="75f1d-135">Получите определение роли для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="75f1d-135">Get a role definition for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleDefinitions/{id}
```

<span data-ttu-id="75f1d-136">Получите определение роли для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="75f1d-136">Get a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="75f1d-137">Получите определение роли для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="75f1d-137">Get a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions/{id}
```

<span data-ttu-id="75f1d-138">Получение определения роли для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="75f1d-138">Get a role definition for the entitlement management provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75f1d-139">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="75f1d-139">Optional query parameters</span></span>

<span data-ttu-id="75f1d-140">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="75f1d-140">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="75f1d-141">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="75f1d-141">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="75f1d-142">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75f1d-142">Request headers</span></span>

| <span data-ttu-id="75f1d-143">Имя</span><span class="sxs-lookup"><span data-stu-id="75f1d-143">Name</span></span>      |<span data-ttu-id="75f1d-144">Описание</span><span class="sxs-lookup"><span data-stu-id="75f1d-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75f1d-145">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75f1d-145">Authorization</span></span> | <span data-ttu-id="75f1d-146">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="75f1d-146">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="75f1d-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75f1d-147">Request body</span></span>

<span data-ttu-id="75f1d-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75f1d-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75f1d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f1d-149">Response</span></span>

<span data-ttu-id="75f1d-150">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75f1d-150">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75f1d-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="75f1d-151">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-custom-role-for-a-directory-provider"></a><span data-ttu-id="75f1d-152">Пример 1. Определение настраиваемой роли поставщика каталогов</span><span class="sxs-lookup"><span data-stu-id="75f1d-152">Example 1: Get the definition of a custom role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="75f1d-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f1d-153">Request</span></span>

<span data-ttu-id="75f1d-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75f1d-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="75f1d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f1d-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custom_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```
# <a name="c"></a>[<span data-ttu-id="75f1d-156">C#</span><span class="sxs-lookup"><span data-stu-id="75f1d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custom-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f1d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f1d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custom-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f1d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f1d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custom-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75f1d-159">Java</span><span class="sxs-lookup"><span data-stu-id="75f1d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custom-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="75f1d-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f1d-160">Response</span></span>

<span data-ttu-id="75f1d-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75f1d-161">The following is an example of the response.</span></span>

> <span data-ttu-id="75f1d-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75f1d-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-built-in-role-for-a-directory-provider"></a><span data-ttu-id="75f1d-163">Пример 2. Определение встроенной роли поставщика каталогов</span><span class="sxs-lookup"><span data-stu-id="75f1d-163">Example 2: Get the definition of a built-in role for a directory provider</span></span>

#### <a name="request"></a><span data-ttu-id="75f1d-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f1d-164">Request</span></span>

<span data-ttu-id="75f1d-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75f1d-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="75f1d-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f1d-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built_in_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c
```
# <a name="c"></a>[<span data-ttu-id="75f1d-167">C#</span><span class="sxs-lookup"><span data-stu-id="75f1d-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f1d-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f1d-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f1d-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f1d-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75f1d-170">Java</span><span class="sxs-lookup"><span data-stu-id="75f1d-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="75f1d-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f1d-171">Response</span></span>

<span data-ttu-id="75f1d-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75f1d-172">The following is an example of the response.</span></span>

> <span data-ttu-id="75f1d-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75f1d-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-3-get-the-definition-of-an-azure-ad-built-in-role-and-expand-on-the-role-it-inherits-from"></a><span data-ttu-id="75f1d-174">Пример 3. Определение встроенной роли Azure AD и $expand роли, которую она наследует</span><span class="sxs-lookup"><span data-stu-id="75f1d-174">Example 3: Get the definition of an Azure AD built-in role and $expand on the role it inherits from</span></span>

#### <a name="request"></a><span data-ttu-id="75f1d-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f1d-175">Request</span></span>

<span data-ttu-id="75f1d-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75f1d-176">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="75f1d-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f1d-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_inheritsFrom_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c?$expand=inheritsPermissionsFrom
```
# <a name="c"></a>[<span data-ttu-id="75f1d-178">C#</span><span class="sxs-lookup"><span data-stu-id="75f1d-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-inheritsfrom-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f1d-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f1d-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-inheritsfrom-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f1d-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f1d-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-inheritsfrom-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75f1d-181">Java</span><span class="sxs-lookup"><span data-stu-id="75f1d-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-inheritsfrom-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="75f1d-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f1d-182">Response</span></span>

<span data-ttu-id="75f1d-183">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75f1d-183">The following is an example of the response.</span></span>

> <span data-ttu-id="75f1d-184">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75f1d-184">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-definition-of-a-built-in-role-for-a-cloud-pc-provider"></a><span data-ttu-id="75f1d-185">Пример 4. Определение роли встроенного компьютера для поставщика облачных ПК</span><span class="sxs-lookup"><span data-stu-id="75f1d-185">Example 4: Get the definition of a built-in role for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="75f1d-186">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f1d-186">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="75f1d-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f1d-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_built-in_cloudpc_role_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleDefinitions/d40368cb-fbf4-4965-bbc1-f17b3a78e510
```
# <a name="c"></a>[<span data-ttu-id="75f1d-188">C#</span><span class="sxs-lookup"><span data-stu-id="75f1d-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-built-in-cloudpc-role-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f1d-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f1d-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-built-in-cloudpc-role-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f1d-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f1d-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-built-in-cloudpc-role-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75f1d-191">Java</span><span class="sxs-lookup"><span data-stu-id="75f1d-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-built-in-cloudpc-role-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="75f1d-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f1d-192">Response</span></span>
> <span data-ttu-id="75f1d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75f1d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleDefinitions/$entity",
    "id": "d40368cb-fbf4-4965-bbc1-f17b3a78e510",
    "description": "Have read-only access all Cloud PC features.",
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
                "Microsoft.CloudPC/Roles/Read",
                "Microsoft.CloudPC/SelfServiceSettings/Read"
            ],
            "condition": null
        }
    ]
}
```

## <a name="example-5-get-the-definition-of-a-built-in-role-for-the-entitlement-management-provider"></a><span data-ttu-id="75f1d-195">Пример 5. Получение определения встроенной роли поставщика управления правами</span><span class="sxs-lookup"><span data-stu-id="75f1d-195">Example 5: Get the definition of a built-in role for the entitlement management provider</span></span>

#### <a name="request"></a><span data-ttu-id="75f1d-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="75f1d-196">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_built-in_entitlementmanagement_role_unifiedroledefinition"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleDefinitions/ba92d953-d8e0-4e39-a797-0cbedb0a89e8
```


#### <a name="response"></a><span data-ttu-id="75f1d-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="75f1d-197">Response</span></span>
> <span data-ttu-id="75f1d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75f1d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleDefinitions/$entity",
    "id": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
    "displayName": "Catalog creator",
    "description": "Catalog creator",
    "isBuiltIn": true,
    "isEnabled": true,
    "templateId": "ba92d953-d8e0-4e39-a797-0cbedb0a89e8",
    "version": "1.0",
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.entitlementManagement/AccessPackageCatalog/Create"
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


