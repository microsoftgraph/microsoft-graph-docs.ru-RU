---
title: Get unifiedRoleAssignment
description: Извлечение свойств и связей объекта unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 238b2e1d6049ec53d779fddba830338b13b6f781
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351043"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="f845a-103">Get unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f845a-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="f845a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f845a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f845a-105">Извлечение свойств и связей объекта [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f845a-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f845a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f845a-106">Permissions</span></span>

<span data-ttu-id="f845a-107">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f845a-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="f845a-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f845a-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="f845a-109">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="f845a-109">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="f845a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f845a-110">Permission type</span></span>      | <span data-ttu-id="f845a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f845a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f845a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f845a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f845a-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f845a-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f845a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f845a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f845a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f845a-115">Not supported.</span></span>    |
|<span data-ttu-id="f845a-116">Application</span><span class="sxs-lookup"><span data-stu-id="f845a-116">Application</span></span> | <span data-ttu-id="f845a-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f845a-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="f845a-118">Поставщик прав на управление правами</span><span class="sxs-lookup"><span data-stu-id="f845a-118">For Entitlement management provider</span></span>

|<span data-ttu-id="f845a-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f845a-119">Permission type</span></span>      | <span data-ttu-id="f845a-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f845a-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f845a-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f845a-121">Delegated (work or school account)</span></span> |  <span data-ttu-id="f845a-122">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f845a-122">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
|<span data-ttu-id="f845a-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f845a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f845a-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f845a-124">Not supported.</span></span>    |
|<span data-ttu-id="f845a-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f845a-125">Application</span></span> | <span data-ttu-id="f845a-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f845a-126">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f845a-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f845a-127">HTTP request</span></span>

<span data-ttu-id="f845a-128">Назначение ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="f845a-128">Get a role assignment for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="f845a-129">Получение назначения ролей для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="f845a-129">Get a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f845a-130">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f845a-130">Optional query parameters</span></span>

<span data-ttu-id="f845a-131">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f845a-131">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="f845a-132">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f845a-132">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f845a-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f845a-133">Request headers</span></span>

| <span data-ttu-id="f845a-134">Имя</span><span class="sxs-lookup"><span data-stu-id="f845a-134">Name</span></span>      |<span data-ttu-id="f845a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f845a-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f845a-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="f845a-136">Authorization</span></span> | <span data-ttu-id="f845a-137">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f845a-137">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f845a-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f845a-138">Request body</span></span>

<span data-ttu-id="f845a-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f845a-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f845a-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="f845a-140">Response</span></span>

<span data-ttu-id="f845a-141">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f845a-141">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f845a-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="f845a-142">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="f845a-143">Пример 1. Сведения о назначении ролей</span><span class="sxs-lookup"><span data-stu-id="f845a-143">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="f845a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="f845a-144">Request</span></span>

<span data-ttu-id="f845a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f845a-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f845a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="f845a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="f845a-147">C#</span><span class="sxs-lookup"><span data-stu-id="f845a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f845a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f845a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f845a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f845a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f845a-150">Java</span><span class="sxs-lookup"><span data-stu-id="f845a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f845a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="f845a-151">Response</span></span>

<span data-ttu-id="f845a-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f845a-152">The following is an example of the response.</span></span>

> <span data-ttu-id="f845a-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f845a-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0"
}
```

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="f845a-154">Пример 2. Сведения о назначении ролей с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="f845a-154">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="f845a-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="f845a-155">Request</span></span>

<span data-ttu-id="f845a-156">Ниже приводится пример запроса с `$expand` параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="f845a-156">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="f845a-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="f845a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="f845a-158">C#</span><span class="sxs-lookup"><span data-stu-id="f845a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f845a-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f845a-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f845a-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f845a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f845a-161">Java</span><span class="sxs-lookup"><span data-stu-id="f845a-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f845a-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="f845a-162">Response</span></span>

<span data-ttu-id="f845a-163">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f845a-163">The following is an example of the response.</span></span>
> <span data-ttu-id="f845a-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f845a-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "roleDefinition": {
      "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
      "displayName": "Billing Administrator",
      "description": "Can perform common billing related tasks like updating payment information.",
      "rolePermissions": [
        {
          "allowedResourceActions": [
            "microsoft.commerce.billing/allEntities/allTasks",
            "microsoft.directory/organization/basic/update",
          ],
          "excludedResourceActions": []
        }],
      "isEnabled": true,
      },
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "principal": {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d ",
      "userPrincipalName": "alice@contoso.com",
      "displayName": "Alice Smith"
    },
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScope": {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Contoso_Seattle_Admins"
    }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


