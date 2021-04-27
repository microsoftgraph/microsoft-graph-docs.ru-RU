---
title: Создание unifiedRoleAssignment
description: Создайте новый объект unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 87b0f474181a8bb622eea401f7df285b9be3b665
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051013"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="096d3-103">Создание unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="096d3-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="096d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="096d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="096d3-105">Создайте новый [объект unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="096d3-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="096d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="096d3-106">Permissions</span></span>

<span data-ttu-id="096d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="096d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="096d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="096d3-109">Permission type</span></span>                        | <span data-ttu-id="096d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="096d3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="096d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="096d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="096d3-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="096d3-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="096d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="096d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="096d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="096d3-114">Not supported.</span></span> |
| <span data-ttu-id="096d3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="096d3-115">Application</span></span>                            | <span data-ttu-id="096d3-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="096d3-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="096d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="096d3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="096d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="096d3-118">Request headers</span></span>

| <span data-ttu-id="096d3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="096d3-119">Name</span></span>          | <span data-ttu-id="096d3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="096d3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="096d3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="096d3-121">Authorization</span></span> | <span data-ttu-id="096d3-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="096d3-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="096d3-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="096d3-123">Request body</span></span>

<span data-ttu-id="096d3-124">В теле запроса поставляем представление JSON объекта [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="096d3-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="096d3-125">Запрос должен иметь область, определенную в Azure AD, например область, определенную приложению, например `directoryScopeId` `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="096d3-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="096d3-126">Примерами области Azure AD являются клиенты ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="096d3-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="096d3-127">Дополнительные сведения см. [в appScope.](../resources/appscope.md)</span><span class="sxs-lookup"><span data-stu-id="096d3-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="096d3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="096d3-128">Response</span></span>

<span data-ttu-id="096d3-129">В случае успешного выполнения этот метод возвращает код отклика и новый объект `201 Created` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="096d3-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="096d3-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="096d3-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="096d3-131">Пример 1. Создание назначения ролей в области клиента</span><span class="sxs-lookup"><span data-stu-id="096d3-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="096d3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="096d3-132">Request</span></span>

<span data-ttu-id="096d3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="096d3-133">The following is an example of the request.</span></span> <span data-ttu-id="096d3-134">Обратите внимание на использование ролиTemplateId для roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="096d3-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="096d3-135">roleDefinitionId может быть как ИД-шаблона для всей службы, так и каталогом ролейDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="096d3-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="096d3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="096d3-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="096d3-137">C#</span><span class="sxs-lookup"><span data-stu-id="096d3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="096d3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="096d3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="096d3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="096d3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="096d3-140">Java</span><span class="sxs-lookup"><span data-stu-id="096d3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="096d3-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="096d3-141">Response</span></span>

<span data-ttu-id="096d3-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="096d3-142">The following is an example of the response.</span></span>

> <span data-ttu-id="096d3-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="096d3-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="096d3-144">Пример 2. Создание назначения ролей над областью административного подразделения</span><span class="sxs-lookup"><span data-stu-id="096d3-144">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="096d3-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="096d3-145">Request</span></span>

<span data-ttu-id="096d3-146">В следующем примере назначается основная роль администратора пользователя над административным подразделением.</span><span class="sxs-lookup"><span data-stu-id="096d3-146">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="096d3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="096d3-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="096d3-148">C#</span><span class="sxs-lookup"><span data-stu-id="096d3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="096d3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="096d3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="096d3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="096d3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="096d3-151">Java</span><span class="sxs-lookup"><span data-stu-id="096d3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="096d3-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="096d3-152">Response</span></span>

<span data-ttu-id="096d3-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="096d3-153">The following is an example of the response.</span></span>

> <span data-ttu-id="096d3-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="096d3-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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


