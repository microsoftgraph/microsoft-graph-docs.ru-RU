---
title: Создание unifiedRoleAssignmentMultiple
description: Создайте новый объект unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9883ea3666b22ddaa21de349b56e361a02d99396
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334607"
---
# <a name="create-unifiedroleassignmentmultiple"></a><span data-ttu-id="569dd-103">Создание unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="569dd-103">Create unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="569dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="569dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="569dd-105">Создайте [новый объект unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="569dd-105">Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object for an RBAC provider.</span></span> 

<span data-ttu-id="569dd-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="569dd-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="569dd-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="569dd-107">cloud PC</span></span> 
- <span data-ttu-id="569dd-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="569dd-108">device management (Intune)</span></span>

<span data-ttu-id="569dd-109">Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="569dd-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="569dd-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="569dd-110">Permissions</span></span>

<span data-ttu-id="569dd-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="569dd-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="569dd-112">Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="569dd-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="569dd-113">Поставщик облачных ПК</span><span class="sxs-lookup"><span data-stu-id="569dd-113">For Cloud PC provider</span></span>

|<span data-ttu-id="569dd-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="569dd-114">Permission type</span></span>      | <span data-ttu-id="569dd-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="569dd-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="569dd-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="569dd-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="569dd-117">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569dd-117">CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="569dd-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="569dd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="569dd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="569dd-119">Not supported.</span></span>    |
|<span data-ttu-id="569dd-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="569dd-120">Application</span></span> | <span data-ttu-id="569dd-121">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569dd-121">CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="569dd-122">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="569dd-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="569dd-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="569dd-123">Permission type</span></span>      | <span data-ttu-id="569dd-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="569dd-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="569dd-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="569dd-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="569dd-126">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569dd-126">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="569dd-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="569dd-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="569dd-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="569dd-128">Not supported.</span></span>    |
|<span data-ttu-id="569dd-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="569dd-129">Application</span></span> | <span data-ttu-id="569dd-130">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569dd-130">DeviceManagementRBAC.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="569dd-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="569dd-131">HTTP request</span></span>

<span data-ttu-id="569dd-132">Чтобы создать назначение ролей для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="569dd-132">To create role assignment for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/cloudPC/roleAssignments
```

<span data-ttu-id="569dd-133">Создание назначения ролей для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="569dd-133">To create role assignment for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="569dd-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="569dd-134">Request headers</span></span>

| <span data-ttu-id="569dd-135">Имя</span><span class="sxs-lookup"><span data-stu-id="569dd-135">Name</span></span> | <span data-ttu-id="569dd-136">Описание</span><span class="sxs-lookup"><span data-stu-id="569dd-136">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="569dd-137">Авторизация</span><span class="sxs-lookup"><span data-stu-id="569dd-137">Authorization</span></span> | <span data-ttu-id="569dd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="569dd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="569dd-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="569dd-140">Content-type</span></span> | <span data-ttu-id="569dd-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="569dd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="569dd-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="569dd-143">Request body</span></span>

<span data-ttu-id="569dd-144">В теле запроса поставляем представление JSON объекта [unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="569dd-144">In the request body, supply a JSON representation of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="569dd-145">Запрос должен иметь область, определенную в Azure AD, например область, определенную приложению, например `directoryScopeIds` `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="569dd-145">The request must have either a scope defined in Azure AD, such as `directoryScopeIds`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="569dd-146">Примерами области Azure AD являются клиенты ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="569dd-146">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> 

## <a name="response"></a><span data-ttu-id="569dd-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="569dd-147">Response</span></span>

<span data-ttu-id="569dd-148">В случае успешного выполнения этот метод возвращает код ответа и новый объект `201 Created` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="569dd-148">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="569dd-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="569dd-149">Examples</span></span>

### <a name="example-1-create-a-role-assignment-in-intune-over-two-scope-groups-which-are-azure-ad-objects"></a><span data-ttu-id="569dd-150">Пример 1. Создание назначения ролей в Intune над двумя группами областей (которые являются объектами Azure AD)</span><span class="sxs-lookup"><span data-stu-id="569dd-150">Example 1: Create a role assignment in Intune over two scope groups (which are Azure AD objects)</span></span>

#### <a name="request"></a><span data-ttu-id="569dd-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="569dd-151">Request</span></span>

<span data-ttu-id="569dd-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="569dd-152">The following is an example of the request.</span></span>
> <span data-ttu-id="569dd-153">**Примечание:** использование **ролиTemplateId** для **roleDefinitionId**.</span><span class="sxs-lookup"><span data-stu-id="569dd-153">**Note:** the use of the **roleTemplateId** for **roleDefinitionId**.</span></span> <span data-ttu-id="569dd-154">**RoleDefinitionId** может быть как ИД шаблона для всей службы, так и ролью, определенной для **каталогаDefinitionId.**</span><span class="sxs-lookup"><span data-stu-id="569dd-154">**roleDefinitionId** can be either the service-wide template ID or the directory-specific **roleDefinitionId**.</span></span>


# <a name="http"></a>[<span data-ttu-id="569dd-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="569dd-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="569dd-156">C#</span><span class="sxs-lookup"><span data-stu-id="569dd-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="569dd-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="569dd-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="569dd-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="569dd-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="569dd-159">Java</span><span class="sxs-lookup"><span data-stu-id="569dd-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="569dd-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="569dd-160">Response</span></span>

<span data-ttu-id="569dd-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="569dd-161">The following is an example of the response.</span></span>
> <span data-ttu-id="569dd-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="569dd-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-a-role-assignment-in-intune-at-intune-specific-scope-of-all-devices"></a><span data-ttu-id="569dd-163">Пример 2. Создание назначения ролей в Intune в области Intune для "всех устройств"</span><span class="sxs-lookup"><span data-stu-id="569dd-163">Example 2: Create a role assignment in Intune at Intune-specific scope of "all Devices"</span></span>

<span data-ttu-id="569dd-164">Используйте следующую информацию для создания назначений ролей Intune:</span><span class="sxs-lookup"><span data-stu-id="569dd-164">Use the following information for creating Intune role assignments:</span></span>
- <span data-ttu-id="569dd-165">Чтобы разрешить назначения на всех устройствах Intune, используйте `AllDevices` значение **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="569dd-165">To allow assignments over all Intune devices, use the `AllDevices` value in **appScopeIds**.</span></span>
- <span data-ttu-id="569dd-166">Чтобы разрешить назначения всем лицензированным пользователям Intune, используйте значение `AllLicensedUsers` **в appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="569dd-166">To allow assignments over all Intune licensed users, use the `AllLicensedUsers` value in **appScopeIds**.</span></span>
- <span data-ttu-id="569dd-167">Чтобы разрешить назначения для всех устройств Intune и лицензированных пользователей, используйте значение `/` **в directoryScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="569dd-167">To allow assignments over all Intune devices and licensed users, use the `/` value in **directoryScopeIds**.</span></span>

#### <a name="request"></a><span data-ttu-id="569dd-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="569dd-168">Request</span></span>

<span data-ttu-id="569dd-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="569dd-169">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="569dd-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="569dd-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="569dd-171">C#</span><span class="sxs-lookup"><span data-stu-id="569dd-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-intune-specific-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="569dd-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="569dd-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-intune-specific-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="569dd-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="569dd-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-intune-specific-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="569dd-174">Java</span><span class="sxs-lookup"><span data-stu-id="569dd-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-intune-specific-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="569dd-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="569dd-175">Response</span></span>

<span data-ttu-id="569dd-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="569dd-176">The following is an example of the response.</span></span>
> <span data-ttu-id="569dd-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="569dd-177">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-create-a-role-assignment-for-a-cloud-pc-provider"></a><span data-ttu-id="569dd-178">Пример 3. Создание назначения ролей для поставщика облачных ПК</span><span class="sxs-lookup"><span data-stu-id="569dd-178">Example 3: Create a role assignment for a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="569dd-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="569dd-179">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="569dd-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="569dd-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="569dd-181">C#</span><span class="sxs-lookup"><span data-stu-id="569dd-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="569dd-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="569dd-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="569dd-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="569dd-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="569dd-184">Java</span><span class="sxs-lookup"><span data-stu-id="569dd-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignmentmultiple-from-rbacapplication-cloudpc-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="569dd-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="569dd-185">Response</span></span>

<span data-ttu-id="569dd-186">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="569dd-186">The following is an example of the response.</span></span>
> <span data-ttu-id="569dd-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="569dd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


