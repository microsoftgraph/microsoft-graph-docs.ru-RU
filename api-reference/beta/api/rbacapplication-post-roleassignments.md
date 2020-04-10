---
title: Создание Унифиедролеассигнмент
description: Создание нового объекта Унифиедролеассигнмент.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7df79449d044963382b9a095b81c96e699f2ffdf
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43216738"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="be3f1-103">Создание Унифиедролеассигнмент</span><span class="sxs-lookup"><span data-stu-id="be3f1-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="be3f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be3f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be3f1-105">Создание нового объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="be3f1-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be3f1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be3f1-106">Permissions</span></span>

<span data-ttu-id="be3f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be3f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be3f1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be3f1-109">Permission type</span></span>                        | <span data-ttu-id="be3f1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="be3f1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be3f1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be3f1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be3f1-112">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="be3f1-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="be3f1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be3f1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be3f1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be3f1-114">Not supported.</span></span> |
| <span data-ttu-id="be3f1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be3f1-115">Application</span></span>                            | <span data-ttu-id="be3f1-116">Ролеманажемент. Read. Directory, Ролеманажемент. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="be3f1-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="be3f1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be3f1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="be3f1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be3f1-118">Request headers</span></span>

| <span data-ttu-id="be3f1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="be3f1-119">Name</span></span>          | <span data-ttu-id="be3f1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="be3f1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="be3f1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be3f1-121">Authorization</span></span> | <span data-ttu-id="be3f1-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="be3f1-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="be3f1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="be3f1-123">Request body</span></span>

<span data-ttu-id="be3f1-124">В тексте запроса добавьте представление объекта [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be3f1-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span> <span data-ttu-id="be3f1-125">В запросе должна быть область, определенная в Azure AD, например `directoryScopeId`, или область, зависящая от `appScopeId`приложения, например.</span><span class="sxs-lookup"><span data-stu-id="be3f1-125">The request must have either a scope defined in Azure AD, such as `directoryScopeId`, or an application-specific scope, such as `appScopeId`.</span></span> <span data-ttu-id="be3f1-126">Примеры областей Azure AD: клиент ("/"), административные единицы или приложения.</span><span class="sxs-lookup"><span data-stu-id="be3f1-126">Examples of Azure AD scope are tenant ("/"), administrative units, or applications.</span></span> <span data-ttu-id="be3f1-127">Дополнительные сведения см. в разделе [аппскопе](../resources/appscope.md).</span><span class="sxs-lookup"><span data-stu-id="be3f1-127">For more information, see [appScope](../resources/appscope.md).</span></span>

## <a name="response"></a><span data-ttu-id="be3f1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="be3f1-128">Response</span></span>

<span data-ttu-id="be3f1-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [унифиедролеассигнмент](../resources/unifiedroleassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be3f1-129">If successful, this method returns a `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be3f1-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="be3f1-130">Examples</span></span>

### <a name="example-1-create-a-role-assignment-at-tenant-scope"></a><span data-ttu-id="be3f1-131">Пример 1: Создание назначения роли на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="be3f1-131">Example 1: Create a role assignment at tenant scope</span></span>

#### <a name="request"></a><span data-ttu-id="be3f1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="be3f1-132">Request</span></span>

<span data-ttu-id="be3f1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be3f1-133">The following is an example of the request.</span></span> <span data-ttu-id="be3f1-134">Обратите внимание на использование параметра Ролетемплатеид для Роледефинитионид.</span><span class="sxs-lookup"><span data-stu-id="be3f1-134">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="be3f1-135">Роледефинитионид может быть либо идентификатором шаблона на уровне службы, либо Роледефинитионид, зависящим от каталога.</span><span class="sxs-lookup"><span data-stu-id="be3f1-135">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>


# <a name="http"></a>[<span data-ttu-id="be3f1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="be3f1-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="be3f1-137">C#</span><span class="sxs-lookup"><span data-stu-id="be3f1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be3f1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be3f1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be3f1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be3f1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be3f1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="be3f1-140">Response</span></span>

<span data-ttu-id="be3f1-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be3f1-141">The following is an example of the response.</span></span>

> <span data-ttu-id="be3f1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be3f1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2--create-a-role-assignment-over-an-administrative-unit-scope"></a><span data-ttu-id="be3f1-144">Пример 2: Создание назначения роли на уровне административной единицы</span><span class="sxs-lookup"><span data-stu-id="be3f1-144">Example 2 : Create a role assignment over an administrative unit scope</span></span>

#### <a name="request"></a><span data-ttu-id="be3f1-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="be3f1-145">Request</span></span>

<span data-ttu-id="be3f1-146">В следующем примере роль администратора основного пользователя назначается административной единице.</span><span class="sxs-lookup"><span data-stu-id="be3f1-146">The following example assigns a principal User Admin role over an administrative unit.</span></span>


# <a name="http"></a>[<span data-ttu-id="be3f1-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="be3f1-147">HTTP</span></span>](#tab/http)
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
    "directoryScopeId": "5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
}
```
# <a name="c"></a>[<span data-ttu-id="be3f1-148">C#</span><span class="sxs-lookup"><span data-stu-id="be3f1-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-over-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be3f1-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be3f1-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-over-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be3f1-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be3f1-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-over-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="be3f1-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="be3f1-151">Response</span></span>

<span data-ttu-id="be3f1-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="be3f1-152">The following is an example of the response.</span></span>

> <span data-ttu-id="be3f1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be3f1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "directoryScopeId": "5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
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
