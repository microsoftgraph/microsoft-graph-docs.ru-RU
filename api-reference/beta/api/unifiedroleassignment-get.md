---
title: Get unifiedRoleAssignment
description: Извлечение свойств и связей объекта unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e24f9a2ae184502123cca58188902d0f66782b87
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317037"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="384a2-103">Get unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="384a2-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="384a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="384a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="384a2-105">Извлечение свойств и связей объекта [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="384a2-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="384a2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="384a2-106">Permissions</span></span>

<span data-ttu-id="384a2-107">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="384a2-107">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="384a2-108">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="384a2-108">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="384a2-109">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="384a2-109">Supported provider</span></span>      | <span data-ttu-id="384a2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="384a2-110">Delegated (work or school account)</span></span>  | <span data-ttu-id="384a2-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="384a2-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="384a2-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="384a2-112">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="384a2-113">Каталог</span><span class="sxs-lookup"><span data-stu-id="384a2-113">Directory</span></span> | <span data-ttu-id="384a2-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="384a2-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="384a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="384a2-115">Not supported.</span></span>| <span data-ttu-id="384a2-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="384a2-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="384a2-117">Управление правами</span><span class="sxs-lookup"><span data-stu-id="384a2-117">Entitlement management</span></span> | <span data-ttu-id="384a2-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="384a2-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> | <span data-ttu-id="384a2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="384a2-119">Not supported.</span></span> | <span data-ttu-id="384a2-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="384a2-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="384a2-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="384a2-121">HTTP request</span></span>

<span data-ttu-id="384a2-122">Назначение ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="384a2-122">Get a role assignment for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

<span data-ttu-id="384a2-123">Получение назначения ролей для поставщика управления правами:</span><span class="sxs-lookup"><span data-stu-id="384a2-123">Get a role assignment for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="384a2-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="384a2-124">Optional query parameters</span></span>

<span data-ttu-id="384a2-125">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="384a2-125">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="384a2-126">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="384a2-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="384a2-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="384a2-127">Request headers</span></span>

| <span data-ttu-id="384a2-128">Имя</span><span class="sxs-lookup"><span data-stu-id="384a2-128">Name</span></span>      |<span data-ttu-id="384a2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="384a2-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="384a2-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="384a2-130">Authorization</span></span> | <span data-ttu-id="384a2-131">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="384a2-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="384a2-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="384a2-132">Request body</span></span>

<span data-ttu-id="384a2-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="384a2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="384a2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="384a2-134">Response</span></span>

<span data-ttu-id="384a2-135">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="384a2-135">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="384a2-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="384a2-136">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="384a2-137">Пример 1. Сведения о назначении ролей</span><span class="sxs-lookup"><span data-stu-id="384a2-137">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="384a2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="384a2-138">Request</span></span>

<span data-ttu-id="384a2-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="384a2-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="384a2-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="384a2-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="384a2-141">C#</span><span class="sxs-lookup"><span data-stu-id="384a2-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="384a2-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="384a2-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="384a2-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="384a2-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="384a2-144">Java</span><span class="sxs-lookup"><span data-stu-id="384a2-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="384a2-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="384a2-145">Response</span></span>

<span data-ttu-id="384a2-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="384a2-146">The following is an example of the response.</span></span>

> <span data-ttu-id="384a2-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="384a2-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="384a2-148">Пример 2. Сведения о назначении ролей с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="384a2-148">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="384a2-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="384a2-149">Request</span></span>

<span data-ttu-id="384a2-150">Ниже приводится пример запроса с `$expand` параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="384a2-150">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="384a2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="384a2-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="384a2-152">C#</span><span class="sxs-lookup"><span data-stu-id="384a2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="384a2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="384a2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="384a2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="384a2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="384a2-155">Java</span><span class="sxs-lookup"><span data-stu-id="384a2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="384a2-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="384a2-156">Response</span></span>

<span data-ttu-id="384a2-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="384a2-157">The following is an example of the response.</span></span>
> <span data-ttu-id="384a2-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="384a2-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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


