---
title: Создание Унифиедролеассигнмент
description: Создание нового объекта Унифиедролеассигнмент.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef1fbbf7c23e7ee79582d1b1c949b0f013f15713
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975160"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="2c003-103">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="2c003-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="2c003-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c003-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c003-105">Создание нового объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2c003-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c003-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c003-106">Permissions</span></span>

<span data-ttu-id="2c003-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c003-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c003-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c003-109">Permission type</span></span>                        | <span data-ttu-id="2c003-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c003-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c003-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c003-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c003-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="2c003-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="2c003-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c003-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c003-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c003-114">Not supported.</span></span> |
| <span data-ttu-id="2c003-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="2c003-115">Application</span></span>                            | <span data-ttu-id="2c003-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="2c003-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c003-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c003-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="2c003-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c003-118">Request headers</span></span>

| <span data-ttu-id="2c003-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2c003-119">Name</span></span>          | <span data-ttu-id="2c003-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2c003-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2c003-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2c003-121">Authorization</span></span> | <span data-ttu-id="2c003-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2c003-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c003-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c003-123">Request body</span></span>

<span data-ttu-id="2c003-124">В тексте запроса добавьте представление объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c003-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="2c003-125">В запросе должна быть область, определенная в Azure AD, например `directoryScopeId` , или область, зависящая от приложения, например `appScopeId` .</span><span class="sxs-lookup"><span data-stu-id="2c003-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="2c003-126">Примеры областей Azure AD: клиент ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="2c003-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="2c003-127">Дополнительные сведения см. в разделе [аппскопе](../resources/appscope.md).</span><span class="sxs-lookup"><span data-stu-id="2c003-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="2c003-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c003-128">Response</span></span>

<span data-ttu-id="2c003-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2c003-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c003-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="2c003-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="2c003-131">Пример 1: Создание назначения роли на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="2c003-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="2c003-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c003-132">Request</span></span>

<span data-ttu-id="2c003-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2c003-133">The following is an example of the request.</span></span> <span data-ttu-id="2c003-134">Обратите внимание на использование параметра Ролетемплатеид для Роледефинитионид.</span><span class="sxs-lookup"><span data-stu-id="2c003-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="2c003-135">Роледефинитионид может быть либо идентификатором шаблона на уровне службы, либо Роледефинитионид, зависящим от каталога.</span><span class="sxs-lookup"><span data-stu-id="2c003-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c003-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c003-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c003-137">C#</span><span class="sxs-lookup"><span data-stu-id="2c003-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c003-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c003-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c003-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c003-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c003-140">Java</span><span class="sxs-lookup"><span data-stu-id="2c003-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c003-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c003-141">Response</span></span>

<span data-ttu-id="2c003-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c003-142">The following is an example of the response.</span></span>

> <span data-ttu-id="2c003-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c003-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="2c003-145">Пример 2: Создание назначения роли на уровне административной единицы</span><span class="sxs-lookup"><span data-stu-id="2c003-145">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="2c003-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c003-146">Request</span></span>

<span data-ttu-id="2c003-147">В следующем примере роль администратора основного пользователя назначается административной единице.</span><span class="sxs-lookup"><span data-stu-id="2c003-147">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="2c003-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c003-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2c003-149">C#</span><span class="sxs-lookup"><span data-stu-id="2c003-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c003-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c003-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c003-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c003-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c003-152">Java</span><span class="sxs-lookup"><span data-stu-id="2c003-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroleassignment-over-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c003-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c003-153">Response</span></span>

<span data-ttu-id="2c003-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2c003-154">The following is an example of the response.</span></span>

> <span data-ttu-id="2c003-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c003-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


