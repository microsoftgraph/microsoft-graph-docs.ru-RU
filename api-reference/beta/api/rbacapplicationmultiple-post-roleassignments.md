---
title: Создание unifiedRoleAssignmentMultiple
description: Создайте новый объект unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: bc09a9c514ab504d81f65983791ae947db313267
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868981"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="c3503-103">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="c3503-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="c3503-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3503-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3503-105">Создайте [новый объект unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="c3503-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object for an RBAC provider.</span></span> 

<span data-ttu-id="c3503-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="c3503-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="c3503-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="c3503-107">cloud PC</span></span> 
- <span data-ttu-id="c3503-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="c3503-108">device management (Intune)</span></span>

<span data-ttu-id="c3503-109">Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c3503-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="c3503-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3503-110">Permissions</span></span>

<span data-ttu-id="c3503-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c3503-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="c3503-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3503-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="c3503-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="c3503-113">Supported provider</span></span>      | <span data-ttu-id="c3503-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3503-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="c3503-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3503-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3503-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c3503-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="c3503-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="c3503-117">Cloud PC</span></span> | <span data-ttu-id="c3503-118">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3503-118">CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="c3503-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3503-119">Not supported.</span></span> | <span data-ttu-id="c3503-120">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3503-120">CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="c3503-121">Intune</span><span class="sxs-lookup"><span data-stu-id="c3503-121">Intune</span></span> | <span data-ttu-id="c3503-122">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3503-122">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="c3503-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3503-123">Not supported.</span></span>| <span data-ttu-id="c3503-124">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3503-124">DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3503-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3503-125">HTTP request</span></span>

<span data-ttu-id="c3503-126">Чтобы создать назначение ролей для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="c3503-126">To create role assignment for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="c3503-127">Создание назначения ролей для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="c3503-127">To create role assignment for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="c3503-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3503-128">Request headers</span></span>

| <span data-ttu-id="c3503-129">Имя</span><span class="sxs-lookup"><span data-stu-id="c3503-129">Name</span></span> | <span data-ttu-id="c3503-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c3503-130">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="c3503-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3503-131">Authorization</span></span> | <span data-ttu-id="c3503-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3503-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3503-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3503-134">Content-type</span></span> | <span data-ttu-id="c3503-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3503-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3503-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3503-137">Request body</span></span>

<span data-ttu-id="c3503-138">В теле запроса поставляем представление JSON объекта [unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="c3503-138">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="c3503-139">Запрос должен иметь область, определенную в Azure AD, например область, определенную приложению, например `directoryScopeIds` `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="c3503-139">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="c3503-140">Примерами области Azure AD являются клиенты ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="c3503-140">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="c3503-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3503-141">Response</span></span>

<span data-ttu-id="c3503-142">В случае успешного выполнения этот метод возвращает код ответа и новый объект `201 Created` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c3503-142">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3503-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="c3503-143">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="c3503-144">Пример 1. Создание назначения ролей в Intune над двумя группами областей (которые являются объектами Azure AD)</span><span class="sxs-lookup"><span data-stu-id="c3503-144">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="c3503-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3503-145">Request</span></span>

<span data-ttu-id="c3503-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3503-146">The following is an example of the request.</span></span>
> <span data-ttu-id="c3503-147">**Примечание:** использование **ролиTemplateId** для **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="c3503-147">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="c3503-148">**RoleDefinitionId** может быть как ИД шаблона для всей службы, так и ролью, определенной для **каталогаDefinitionId.**</span><span class="sxs-lookup"><span data-stu-id="c3503-148">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="c3503-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3503-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
}
```
# <a name="c"></a>[<span data-ttu-id="c3503-150">C#</span><span class="sxs-lookup"><span data-stu-id="c3503-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3503-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3503-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3503-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3503-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3503-153">Java</span><span class="sxs-lookup"><span data-stu-id="c3503-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c3503-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3503-154">Response</span></span>

<span data-ttu-id="c3503-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c3503-155">The following is an example of the response.</span></span>
> <span data-ttu-id="c3503-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3503-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="c3503-157">Пример 2. Создание назначения ролей в Intune в области Intune для "всех устройств"</span><span class="sxs-lookup"><span data-stu-id="c3503-157">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="c3503-158">Используйте следующую информацию для создания назначений ролей Intune:</span><span class="sxs-lookup"><span data-stu-id="c3503-158">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="c3503-159">Чтобы разрешить назначения на всех устройствах Intune, используйте `AllDevices` значение **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="c3503-159">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="c3503-160">Чтобы разрешить назначения всем лицензированным пользователям Intune, используйте значение `AllLicensedUsers` **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="c3503-160">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="c3503-161">Чтобы разрешить назначения для всех устройств Intune и лицензированных пользователей, используйте значение `/` **в directoryScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="c3503-161">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="c3503-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3503-162">Request</span></span>

<span data-ttu-id="c3503-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3503-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c3503-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3503-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_intune_specific"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```
# <a name="c"></a>[<span data-ttu-id="c3503-165">C#</span><span class="sxs-lookup"><span data-stu-id="c3503-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3503-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3503-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3503-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3503-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3503-168">Java</span><span class="sxs-lookup"><span data-stu-id="c3503-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c3503-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3503-169">Response</span></span>

<span data-ttu-id="c3503-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c3503-170">The following is an example of the response.</span></span>
> <span data-ttu-id="c3503-171">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c3503-171">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    "appScopeIds": ["allDevices"]
}
```

### <a name="example-3-create-a-role-assignment-for-a-cloud-pc-provider"></a><span data-ttu-id="c3503-172">Пример 3. Создание назначения ролей для поставщика облачных ПК</span><span class="sxs-lookup"><span data-stu-id="c3503-172">Example 3: Create a role assignment for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="c3503-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3503-173">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c3503-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3503-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignmentmultiple_from_rbacapplication_cloudpc"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "displayName": "My test role assignment 1",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"]
}
```
# <a name="c"></a>[<span data-ttu-id="c3503-175">C#</span><span class="sxs-lookup"><span data-stu-id="c3503-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3503-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3503-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3503-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3503-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3503-178">Java</span><span class="sxs-lookup"><span data-stu-id="c3503-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="c3503-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3503-179">Response</span></span>

<span data-ttu-id="c3503-180">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3503-180">The following is an example of the response.</span></span>
> <span data-ttu-id="c3503-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3503-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "47c88dcd-cc79-4b0c-ba7d-7af2199649c5",
    "displayName": "My role assignment",
    "description": "My role assignment description",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
        "c1518aa9-4da5-4c84-a902-a31404023890"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignmentMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


