---
title: Получение unifiedRoleAssignmentMultiple
description: Извлечение свойств и связей объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9e9867d2c314534115f7c620d52329805d8b890e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960622"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="44db7-103">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="44db7-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="44db7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44db7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44db7-105">Извлечение свойств и связей объекта [unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="44db7-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="44db7-106">Используйте этот объект для получения назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="44db7-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="44db7-107">Для других приложений Microsoft 365 (например, Azure AD) используйте [унифицированныеRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="44db7-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="44db7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44db7-108">Permissions</span></span>

<span data-ttu-id="44db7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44db7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44db7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44db7-111">Permission type</span></span> | <span data-ttu-id="44db7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44db7-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="44db7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44db7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="44db7-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44db7-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="44db7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44db7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44db7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44db7-116">Not supported.</span></span> |
| <span data-ttu-id="44db7-117">Application</span><span class="sxs-lookup"><span data-stu-id="44db7-117">Application</span></span> | <span data-ttu-id="44db7-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44db7-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44db7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44db7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44db7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="44db7-120">Optional query parameters</span></span>

<span data-ttu-id="44db7-121">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="44db7-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="44db7-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="44db7-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="44db7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44db7-123">Request headers</span></span>

| <span data-ttu-id="44db7-124">Имя</span><span class="sxs-lookup"><span data-stu-id="44db7-124">Name</span></span>  | <span data-ttu-id="44db7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="44db7-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="44db7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44db7-126">Authorization</span></span> | <span data-ttu-id="44db7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44db7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44db7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44db7-129">Request body</span></span>

<span data-ttu-id="44db7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44db7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44db7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="44db7-131">Response</span></span>

<span data-ttu-id="44db7-132">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="44db7-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44db7-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="44db7-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="44db7-134">Пример 1. Получить роль в каталогеAssignmentMultiple в Intune</span><span class="sxs-lookup"><span data-stu-id="44db7-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="44db7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="44db7-135">Request</span></span>

<span data-ttu-id="44db7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44db7-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="44db7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="44db7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="44db7-138">C#</span><span class="sxs-lookup"><span data-stu-id="44db7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44db7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44db7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44db7-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44db7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44db7-141">Java</span><span class="sxs-lookup"><span data-stu-id="44db7-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44db7-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="44db7-142">Response</span></span>

<span data-ttu-id="44db7-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44db7-143">The following is an example of the response.</span></span>
> <span data-ttu-id="44db7-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44db7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-roleassignmentmultiple-in-intune-assigned-to-a-group"></a><span data-ttu-id="44db7-146">Пример 2. Получить рольAssignmentMultiple в Intune, назначенной группе</span><span class="sxs-lookup"><span data-stu-id="44db7-146">Example 2: Get a roleAssignmentMultiple in Intune assigned to a group</span></span>

#### <a name="request"></a><span data-ttu-id="44db7-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="44db7-147">Request</span></span>

<span data-ttu-id="44db7-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44db7-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="44db7-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="44db7-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="44db7-150">C#</span><span class="sxs-lookup"><span data-stu-id="44db7-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44db7-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44db7-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44db7-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44db7-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44db7-153">Java</span><span class="sxs-lookup"><span data-stu-id="44db7-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44db7-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="44db7-154">Response</span></span>

<span data-ttu-id="44db7-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44db7-155">The following is an example of the response.</span></span>
> <span data-ttu-id="44db7-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44db7-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="44db7-158">Пример 3. Получить роль с областью каталогаAssignmentMultiple с `$expand`</span><span class="sxs-lookup"><span data-stu-id="44db7-158">Example 3: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="44db7-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="44db7-159">Request</span></span>

<span data-ttu-id="44db7-160">Ниже приводится пример запроса с `$expand` параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="44db7-160">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="44db7-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="44db7-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="44db7-162">C#</span><span class="sxs-lookup"><span data-stu-id="44db7-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44db7-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44db7-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44db7-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44db7-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="44db7-165">Java</span><span class="sxs-lookup"><span data-stu-id="44db7-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44db7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="44db7-166">Response</span></span>

<span data-ttu-id="44db7-167">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44db7-167">The following is an example of the response.</span></span>
> <span data-ttu-id="44db7-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44db7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


