---
title: Создание unifiedRoleAssignment
description: Создайте новый объект unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a7587bf4dea653b86b4f93632e5719bcec4aaaaa
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351113"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="4c373-103">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4c373-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="4c373-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c373-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c373-105">Создайте новый [объект unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4c373-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c373-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c373-106">Permissions</span></span>

<span data-ttu-id="4c373-107">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4c373-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="4c373-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c373-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="4c373-109">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="4c373-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="4c373-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c373-110">Permission type</span></span>      | <span data-ttu-id="4c373-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c373-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c373-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c373-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c373-113">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="4c373-113">RoleManagement.ReadWrite.Directory</span></span>   |
|<span data-ttu-id="4c373-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c373-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c373-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c373-115">Not supported.</span></span>    |
|<span data-ttu-id="4c373-116">Application</span><span class="sxs-lookup"><span data-stu-id="4c373-116">Application</span></span> | <span data-ttu-id="4c373-117">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="4c373-117">RoleManagement.ReadWrite.Directory</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="4c373-118">Поставщик прав на управление правами</span><span class="sxs-lookup"><span data-stu-id="4c373-118">For Entitlement management provider</span></span>

|<span data-ttu-id="4c373-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c373-119">Permission type</span></span>      | <span data-ttu-id="4c373-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c373-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c373-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c373-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c373-122">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c373-122">EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="4c373-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c373-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c373-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c373-124">Not supported.</span></span>    |
|<span data-ttu-id="4c373-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c373-125">Application</span></span> | <span data-ttu-id="4c373-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c373-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c373-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c373-127">HTTP request</span></span>

<span data-ttu-id="4c373-128">Создание назначения ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="4c373-128">Create a role assignment for the directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

<span data-ttu-id="4c373-129">Создайте назначение ролей для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="4c373-129">Create a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/entitlementManagement/roleAssignments
```


## <a name="request-headers"></a><span data-ttu-id="4c373-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c373-130">Request headers</span></span>

| <span data-ttu-id="4c373-131">Имя</span><span class="sxs-lookup"><span data-stu-id="4c373-131">Name</span></span>          | <span data-ttu-id="4c373-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c373-132">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4c373-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c373-133">Authorization</span></span> | <span data-ttu-id="4c373-134">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4c373-134">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c373-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c373-135">Request body</span></span>

<span data-ttu-id="4c373-136">В теле запроса поставляем представление JSON объекта [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4c373-136">In the request body, supply a JSON representation of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="4c373-137">Запрос должен иметь область, определенную в Azure AD, например **directoryScopeId,** или область приложения, например **appScopeId.**</span><span class="sxs-lookup"><span data-stu-id="4c373-137">The request must have either a scope defined in Azure AD, such as **directoryScopeId**, or an application-specific scope, such as **appScopeId**.</span></span> <span data-ttu-id="4c373-138">Примерами областей Azure AD являются клиенты ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="4c373-138">Examples of Azure AD scopes are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="4c373-139">Управление правами использует области каталога клиентов ("/") и пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="4c373-139">Entitlement management uses tenant ("/") and access package catalog scopes.</span></span> <span data-ttu-id="4c373-140">Дополнительные сведения см. [в appScope.](../resources/appscope.md)</span><span class="sxs-lookup"><span data-stu-id="4c373-140">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="4c373-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c373-141">Response</span></span>

<span data-ttu-id="4c373-142">В случае успешного выполнения этот метод возвращает код отклика и новый объект `201 Created` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4c373-142">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4c373-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="4c373-143">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="4c373-144">Пример 1. Создание назначения ролей в области клиента</span><span class="sxs-lookup"><span data-stu-id="4c373-144">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="4c373-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c373-145">Request</span></span>

<span data-ttu-id="4c373-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c373-146">The following is an example of the request.</span></span> <span data-ttu-id="4c373-147">Обратите внимание на использование ролиTemplateId для roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="4c373-147">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="4c373-148">roleDefinitionId может быть как ИД-шаблона для всей службы, так и каталогом ролейDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="4c373-148">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="4c373-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c373-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```
# <a name="c"></a>[<span data-ttu-id="4c373-150">C#</span><span class="sxs-lookup"><span data-stu-id="4c373-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c373-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c373-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c373-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c373-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c373-153">Java</span><span class="sxs-lookup"><span data-stu-id="4c373-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c373-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c373-154">Response</span></span>

<span data-ttu-id="4c373-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c373-155">The following is an example of the response.</span></span>

> <span data-ttu-id="4c373-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c373-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/"
}
```

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="4c373-157">Пример 2. Создание назначения ролей над областью административного подразделения</span><span class="sxs-lookup"><span data-stu-id="4c373-157">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="4c373-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c373-158">Request</span></span>

<span data-ttu-id="4c373-159">В следующем примере назначается основная роль администратора пользователя над административным подразделением.</span><span class="sxs-lookup"><span data-stu-id="4c373-159">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="4c373-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c373-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_over_administrativeunit"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1", //template id of User Account Administrator
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
}
```
# <a name="c"></a>[<span data-ttu-id="4c373-161">C#</span><span class="sxs-lookup"><span data-stu-id="4c373-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c373-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c373-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c373-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c373-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c373-164">Java</span><span class="sxs-lookup"><span data-stu-id="4c373-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4c373-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c373-165">Response</span></span>

<span data-ttu-id="4c373-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c373-166">The following is an example of the response.</span></span>

> <span data-ttu-id="4c373-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c373-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "BH21sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHIWb7-1",
    "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1",
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScopeId": "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
}
```


### <a name="example-3-create-a-role-assignment-at-access-package-catalog-scope"></a><span data-ttu-id="4c373-168">Пример 3. Создание назначения ролей в области каталога пакетов доступа</span><span class="sxs-lookup"><span data-stu-id="4c373-168">Example 3: Create a role assignment at access package catalog scope</span></span>

#### <a name="request"></a><span data-ttu-id="4c373-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c373-169">Request</span></span>

<span data-ttu-id="4c373-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c373-170">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment3_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/entitlementManagement/roleAssignments
Content-type: application/json

{
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```

#### <a name="response"></a><span data-ttu-id="4c373-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c373-171">Response</span></span>

<span data-ttu-id="4c373-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c373-172">The following is an example of the response.</span></span>

> <span data-ttu-id="4c373-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c373-173">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/entitlementManagement/roleAssignments/$entity",
    "id": "f3092518-7874-462e-93e9-0cd6c11ffc52",
    "principalId": "679a9213-c497-48a4-830a-8d3d25d94ddc",
    "roleDefinitionId": "ae79f266-94d4-4dab-b730-feca7e132178",
    "appScopeId": "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

