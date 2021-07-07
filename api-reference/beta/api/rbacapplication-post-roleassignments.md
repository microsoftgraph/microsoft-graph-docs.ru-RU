---
title: Создание unifiedRoleAssignment
description: Создайте новый объект unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: aafcc34d288dcce1bcd0970802472a2e2e565e83
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317205"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="9fb4a-103">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9fb4a-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="9fb4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fb4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fb4a-105">Создайте новый [объект unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9fb4a-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fb4a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9fb4a-106">Permissions</span></span>

<span data-ttu-id="9fb4a-107">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="9fb4a-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fb4a-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fb4a-109">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="9fb4a-109">Supported provider</span></span>      | <span data-ttu-id="9fb4a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fb4a-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="9fb4a-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fb4a-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb4a-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fb4a-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="9fb4a-113">Каталог</span><span class="sxs-lookup"><span data-stu-id="9fb4a-113">Directory</span></span> | <span data-ttu-id="9fb4a-114">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9fb4a-114">RoleManagement.ReadWrite.Directory</span></span> | <span data-ttu-id="9fb4a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-115">Not supported.</span></span>| <span data-ttu-id="9fb4a-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9fb4a-116">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="9fb4a-117">Управление правами</span><span class="sxs-lookup"><span data-stu-id="9fb4a-117">Entitlement management</span></span> | <span data-ttu-id="9fb4a-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fb4a-118">EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="9fb4a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-119">Not supported.</span></span> | <span data-ttu-id="9fb4a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fb4a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fb4a-121">HTTP request</span></span>

<span data-ttu-id="9fb4a-122">Создание назначения ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="9fb4a-122">Create a role assignment for the directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

<span data-ttu-id="9fb4a-123">Создайте назначение ролей для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="9fb4a-123">Create a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/entitlementManagement/roleAssignments
```


## <a name="request-headers"></a><span data-ttu-id="9fb4a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fb4a-124">Request headers</span></span>

| <span data-ttu-id="9fb4a-125">Имя</span><span class="sxs-lookup"><span data-stu-id="9fb4a-125">Name</span></span>          | <span data-ttu-id="9fb4a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9fb4a-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9fb4a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fb4a-127">Authorization</span></span> | <span data-ttu-id="9fb4a-128">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="9fb4a-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fb4a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fb4a-129">Request body</span></span>

<span data-ttu-id="9fb4a-130">В теле запроса поставляем представление JSON объекта [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9fb4a-130">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="9fb4a-131">Запрос должен иметь область, определенную в Azure AD, например область, определенную приложению, например `directoryScopeId` `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="9fb4a-131">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="9fb4a-132">Примерами области Azure AD являются клиенты ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-132">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="9fb4a-133">Дополнительные сведения см. [в appScope.](../resources/appscope.md)</span><span class="sxs-lookup"><span data-stu-id="9fb4a-133">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="9fb4a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fb4a-134">Response</span></span>

<span data-ttu-id="9fb4a-135">В случае успешного выполнения этот метод возвращает код отклика и новый объект `201 Created` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-135">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9fb4a-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="9fb4a-136">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="9fb4a-137">Пример 1. Создание назначения ролей в области клиента</span><span class="sxs-lookup"><span data-stu-id="9fb4a-137">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="9fb4a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fb4a-138">Request</span></span>

<span data-ttu-id="9fb4a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-139">The following is an example of the request.</span></span> <span data-ttu-id="9fb4a-140">Обратите внимание на использование ролиTemplateId для roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-140">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="9fb4a-141">roleDefinitionId может быть как ИД-шаблона для всей службы, так и каталогом ролейDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-141">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="9fb4a-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb4a-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9fb4a-143">C#</span><span class="sxs-lookup"><span data-stu-id="9fb4a-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fb4a-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fb4a-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fb4a-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fb4a-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fb4a-146">Java</span><span class="sxs-lookup"><span data-stu-id="9fb4a-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9fb4a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fb4a-147">Response</span></span>

<span data-ttu-id="9fb4a-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-148">The following is an example of the response.</span></span>

> <span data-ttu-id="9fb4a-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="9fb4a-150">Пример 2. Создание назначения ролей над областью административного подразделения</span><span class="sxs-lookup"><span data-stu-id="9fb4a-150">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="9fb4a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fb4a-151">Request</span></span>

<span data-ttu-id="9fb4a-152">В следующем примере назначается основная роль администратора пользователя над административным подразделением.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-152">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="9fb4a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb4a-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9fb4a-154">C#</span><span class="sxs-lookup"><span data-stu-id="9fb4a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fb4a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fb4a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fb4a-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fb4a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fb4a-157">Java</span><span class="sxs-lookup"><span data-stu-id="9fb4a-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9fb4a-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fb4a-158">Response</span></span>

<span data-ttu-id="9fb4a-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-159">The following is an example of the response.</span></span>

> <span data-ttu-id="9fb4a-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9fb4a-160">**Note:** The response object shown here might be shortened for readability.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


