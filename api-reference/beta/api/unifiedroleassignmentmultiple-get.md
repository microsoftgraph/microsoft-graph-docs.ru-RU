---
title: Получение unifiedRoleAssignmentMultiple
description: Извлечение свойств и связей объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4e249a334487538cc0c2c708bf94dddc26818457
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054765"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="7d1f6-103">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="7d1f6-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="7d1f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d1f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d1f6-105">Извлечение свойств и связей объекта [unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="7d1f6-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="7d1f6-106">Используйте этот объект для получения назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="7d1f6-107">Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d1f6-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d1f6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d1f6-108">Permissions</span></span>

<span data-ttu-id="7d1f6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d1f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d1f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d1f6-111">Permission type</span></span> | <span data-ttu-id="7d1f6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d1f6-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="7d1f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d1f6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7d1f6-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d1f6-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="7d1f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d1f6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d1f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-116">Not supported.</span></span> |
| <span data-ttu-id="7d1f6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d1f6-117">Application</span></span> | <span data-ttu-id="7d1f6-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d1f6-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d1f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d1f6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d1f6-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d1f6-120">Optional query parameters</span></span>

<span data-ttu-id="7d1f6-121">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="7d1f6-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7d1f6-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d1f6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d1f6-123">Request headers</span></span>

| <span data-ttu-id="7d1f6-124">Имя</span><span class="sxs-lookup"><span data-stu-id="7d1f6-124">Name</span></span>  | <span data-ttu-id="7d1f6-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7d1f6-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="7d1f6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d1f6-126">Authorization</span></span> | <span data-ttu-id="7d1f6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d1f6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d1f6-129">Request body</span></span>

<span data-ttu-id="7d1f6-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d1f6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d1f6-131">Response</span></span>

<span data-ttu-id="7d1f6-132">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d1f6-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d1f6-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="7d1f6-134">Пример 1. Получить роль в каталогеAssignmentMultiple в Intune</span><span class="sxs-lookup"><span data-stu-id="7d1f6-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="7d1f6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d1f6-135">Request</span></span>

<span data-ttu-id="7d1f6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d1f6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d1f6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="7d1f6-138">C#</span><span class="sxs-lookup"><span data-stu-id="7d1f6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d1f6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d1f6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d1f6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d1f6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d1f6-141">Java</span><span class="sxs-lookup"><span data-stu-id="7d1f6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d1f6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d1f6-142">Response</span></span>

<span data-ttu-id="7d1f6-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-143">The following is an example of the response.</span></span>
> <span data-ttu-id="7d1f6-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalIds[]": ["4ab0b690-479b-47ff-af8f-2576cf521872", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
    "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-get-a-roleassignmentmultiple-in-intune-assigned-to-a-group"></a><span data-ttu-id="7d1f6-145">Пример 2. Получить рольAssignmentMultiple в Intune, назначенной группе</span><span class="sxs-lookup"><span data-stu-id="7d1f6-145">Example 2: Get a roleAssignmentMultiple in Intune assigned to a group</span></span>

#### <a name="request"></a><span data-ttu-id="7d1f6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d1f6-146">Request</span></span>

<span data-ttu-id="7d1f6-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d1f6-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d1f6-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="7d1f6-149">C#</span><span class="sxs-lookup"><span data-stu-id="7d1f6-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d1f6-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d1f6-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d1f6-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d1f6-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d1f6-152">Java</span><span class="sxs-lookup"><span data-stu-id="7d1f6-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d1f6-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d1f6-153">Response</span></span>

<span data-ttu-id="7d1f6-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-154">The following is an example of the response.</span></span>
> <span data-ttu-id="7d1f6-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments",
    "@odata.count": 7,
    "value": [
        {
            "id": "893fc648-73fc-482b-b964-ddd1cabf0db4",
            "condition": null,
            "displayName": "Assign Contoso_App_Admin to School Admin",
            "description": "test",
            "roleDefinitionId": "2f9f4f7e-2d13-427b-adf2-361a1eef7ae8",
            "principalIds": [
                "564ae70c-73d9-476b-820b-fb61eb7384b9"
            ],
            "directoryScopeIds": [],
            "appScopeIds": [
                "0",
                "AllLicensedUsers"
            ]
        }
    ]
}
```

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="7d1f6-156">Пример 3. Получить роль с областью каталогаAssignmentMultiple с `$expand`</span><span class="sxs-lookup"><span data-stu-id="7d1f6-156">Example 3: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="7d1f6-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d1f6-157">Request</span></span>

<span data-ttu-id="7d1f6-158">Ниже приводится пример запроса с `$expand` параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-158">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="7d1f6-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d1f6-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="7d1f6-160">C#</span><span class="sxs-lookup"><span data-stu-id="7d1f6-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d1f6-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d1f6-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d1f6-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d1f6-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d1f6-163">Java</span><span class="sxs-lookup"><span data-stu-id="7d1f6-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d1f6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d1f6-164">Response</span></span>

<span data-ttu-id="7d1f6-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-165">The following is an example of the response.</span></span>
> <span data-ttu-id="7d1f6-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d1f6-166">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
  "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
  "roleDefinition": {
    "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "displayName": "Application Manager",
    "description": "Manages mobile and managed applications",
    "rolePermissions": [
      {
        "allowedResourceActions": [],
        "excludedResourceActions": [],
    }],
    "isEnabled": true,
    "isBuiltIn": true,
  },
  "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
  "principals": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Global IT"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "c1518aa9-4da5-4c84-a902-a31404023890",
      "displayName": "Americas IT"
    }
],
  "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
  "directoryScopes": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Washington Sales Region"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "8152656a-cf9a-4928-a457-1512d4cae295",
      "displayName": "Oregon Sales Region"
    }
  ]
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


