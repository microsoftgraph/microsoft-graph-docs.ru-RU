---
title: Получение unifiedRoleAssignmentMultiple
description: Извлечение свойств и связей объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6b1aeecdae5b36e4c10768ee37b1505aba25687b
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334502"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="e5cef-103">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="e5cef-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="e5cef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5cef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5cef-105">Получите свойства и связи объекта [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="e5cef-105">Get the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="e5cef-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="e5cef-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="e5cef-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="e5cef-107">cloud PC</span></span> 
- <span data-ttu-id="e5cef-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="e5cef-108">device management (Intune)</span></span>

<span data-ttu-id="e5cef-109">Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e5cef-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="e5cef-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5cef-110">Permissions</span></span>

<span data-ttu-id="e5cef-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e5cef-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="e5cef-112">Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="e5cef-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="e5cef-113">Поставщик облачных ПК</span><span class="sxs-lookup"><span data-stu-id="e5cef-113">For Cloud PC provider</span></span>

|<span data-ttu-id="e5cef-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5cef-114">Permission type</span></span>      | <span data-ttu-id="e5cef-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5cef-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5cef-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5cef-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5cef-117">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cef-117">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="e5cef-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5cef-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5cef-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5cef-119">Not supported.</span></span>    |
|<span data-ttu-id="e5cef-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5cef-120">Application</span></span> | <span data-ttu-id="e5cef-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cef-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="e5cef-122">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="e5cef-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="e5cef-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5cef-123">Permission type</span></span>      | <span data-ttu-id="e5cef-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5cef-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5cef-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5cef-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5cef-126">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cef-126">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="e5cef-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5cef-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5cef-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5cef-128">Not supported.</span></span>    |
|<span data-ttu-id="e5cef-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5cef-129">Application</span></span> | <span data-ttu-id="e5cef-130">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5cef-130">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |



## <a name="http-request"></a><span data-ttu-id="e5cef-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5cef-131">HTTP request</span></span>

<span data-ttu-id="e5cef-132">Чтобы получить свойства и связи единого поставщика облачных КОМПЬЮТЕРов, службу единойRoleAssignmentMultiple:</span><span class="sxs-lookup"><span data-stu-id="e5cef-132">To get the properties and relationships of a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="e5cef-133">Для получения свойств и связей единого поставщика Intune Для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="e5cef-133">To get the properties and relationships of a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5cef-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5cef-134">Optional query parameters</span></span>

<span data-ttu-id="e5cef-135">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5cef-135">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="e5cef-136">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e5cef-136">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5cef-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5cef-137">Request headers</span></span>

| <span data-ttu-id="e5cef-138">Имя</span><span class="sxs-lookup"><span data-stu-id="e5cef-138">Name</span></span>  | <span data-ttu-id="e5cef-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e5cef-139">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="e5cef-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5cef-140">Authorization</span></span> | <span data-ttu-id="e5cef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5cef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5cef-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5cef-143">Request body</span></span>

<span data-ttu-id="e5cef-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5cef-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5cef-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5cef-145">Response</span></span>

<span data-ttu-id="e5cef-146">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e5cef-146">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e5cef-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="e5cef-147">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="e5cef-148">Пример 1. Получить роль с областью каталоговAssignmentMultiple в поставщике Intune</span><span class="sxs-lookup"><span data-stu-id="e5cef-148">Example 1: Get a directory-scoped roleAssignmentMultiple in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="e5cef-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5cef-149">Request</span></span>

<span data-ttu-id="e5cef-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5cef-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5cef-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5cef-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="e5cef-152">C#</span><span class="sxs-lookup"><span data-stu-id="e5cef-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5cef-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5cef-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5cef-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5cef-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5cef-155">Java</span><span class="sxs-lookup"><span data-stu-id="e5cef-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5cef-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5cef-156">Response</span></span>

<span data-ttu-id="e5cef-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5cef-157">The following is an example of the response.</span></span>
> <span data-ttu-id="e5cef-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5cef-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-roleassignmentmultiple-assigned-to-a-group-in-an-intune-provider"></a><span data-ttu-id="e5cef-159">Пример 2. Получить рольAssignmentMultiple, назначенную группе в поставщике Intune</span><span class="sxs-lookup"><span data-stu-id="e5cef-159">Example 2: Get a roleAssignmentMultiple assigned to a group in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="e5cef-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5cef-160">Request</span></span>

<span data-ttu-id="e5cef-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5cef-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5cef-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5cef-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="e5cef-163">C#</span><span class="sxs-lookup"><span data-stu-id="e5cef-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5cef-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5cef-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5cef-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5cef-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5cef-166">Java</span><span class="sxs-lookup"><span data-stu-id="e5cef-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5cef-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5cef-167">Response</span></span>

<span data-ttu-id="e5cef-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5cef-168">The following is an example of the response.</span></span>
> <span data-ttu-id="e5cef-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5cef-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider-with-expand"></a><span data-ttu-id="e5cef-170">Пример 3. Получить роль с областью каталоговAssignmentMultiple в поставщике Intune с `$expand`</span><span class="sxs-lookup"><span data-stu-id="e5cef-170">Example 3: Get a directory-scoped roleAssignmentMultiple in an Intune provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="e5cef-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5cef-171">Request</span></span>

<span data-ttu-id="e5cef-172">Ниже приводится пример запроса с `$expand` параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="e5cef-172">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5cef-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5cef-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="e5cef-174">C#</span><span class="sxs-lookup"><span data-stu-id="e5cef-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5cef-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5cef-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5cef-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5cef-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5cef-177">Java</span><span class="sxs-lookup"><span data-stu-id="e5cef-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5cef-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5cef-178">Response</span></span>

<span data-ttu-id="e5cef-179">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5cef-179">The following is an example of the response.</span></span>
> <span data-ttu-id="e5cef-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5cef-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-4-get-a-roleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="e5cef-181">Пример 4. Получить рольAssignmentMultiple в поставщике облачных ПК</span><span class="sxs-lookup"><span data-stu-id="e5cef-181">Example 4: Get a roleAssignmentMultiple in a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="e5cef-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5cef-182">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e5cef-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5cef-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
```
# <a name="c"></a>[<span data-ttu-id="e5cef-184">C#</span><span class="sxs-lookup"><span data-stu-id="e5cef-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5cef-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5cef-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5cef-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5cef-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5cef-187">Java</span><span class="sxs-lookup"><span data-stu-id="e5cef-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5cef-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5cef-188">Response</span></span>
> <span data-ttu-id="e5cef-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5cef-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "description": null,
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "8e811502-ebda-4782-8f81-071d17f0f892",
        "30e3492f-964c-4d73-88c6-986a53c6e2a0"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```

### <a name="example-5-get-a-roleassignmentmultiple-in-a-cloud-pc-provider-with-expand"></a><span data-ttu-id="e5cef-191">Пример 5. Получить рольAssignmentMultiple в поставщике облачных ПК с `$expand`</span><span class="sxs-lookup"><span data-stu-id="e5cef-191">Example 5: Get a roleAssignmentMultiple in a cloud PC provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="e5cef-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5cef-192">Request</span></span>

<span data-ttu-id="e5cef-193">Ниже приводится пример запроса с `$expand` параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="e5cef-193">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5cef-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5cef-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096?$expand=roleDefinition
```
# <a name="c"></a>[<span data-ttu-id="e5cef-195">C#</span><span class="sxs-lookup"><span data-stu-id="e5cef-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5cef-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5cef-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5cef-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5cef-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5cef-198">Java</span><span class="sxs-lookup"><span data-stu-id="e5cef-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5cef-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5cef-199">Response</span></span>
> <span data-ttu-id="e5cef-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5cef-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": ["8e811502-ebda-4782-8f81-071d17f0f892", "30e3492f-964c-4d73-88c6-986a53c6e2a0"],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": [],
    "roleDefinitions": {
        "id": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "description": "Have read and write access to all Cloud PC features.",
        "displayName": "Cloud PC Administrator",
        "isBuiltIn": true,
        "isEnabled": true,
        "resourceScopes": [
            "/"
        ],
        "templateId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "version": null,
        "rolePermissions": [
            {
                "allowedResourceActions": [
                    "Microsoft.CloudPC/CloudPCs/Read",
                    "Microsoft.CloudPC/CloudPCs/Reprovision",
                    "Microsoft.CloudPC/DeviceImages/Create",
                    "Microsoft.CloudPC/DeviceImages/Delete",
                    "Microsoft.CloudPC/DeviceImages/Read",
                    "Microsoft.CloudPC/OnPremisesConnections/Create",
                    "Microsoft.CloudPC/OnPremisesConnections/Delete",
                    "Microsoft.CloudPC/OnPremisesConnections/Read",
                    "Microsoft.CloudPC/OnPremisesConnections/Update",
                    "Microsoft.CloudPC/OnPremisesConnections/RunHealthChecks",
                    "Microsoft.CloudPC/OnPremisesConnections/UpdateAdDomainPassword",
                    "Microsoft.CloudPC/ProvisioningPolicies/Assign",
                    "Microsoft.CloudPC/ProvisioningPolicies/Create",
                    "Microsoft.CloudPC/ProvisioningPolicies/Delete",
                    "Microsoft.CloudPC/ProvisioningPolicies/Read",
                    "Microsoft.CloudPC/ProvisioningPolicies/Update",
                    "Microsoft.CloudPC/RoleAssignments/Create",
                    "Microsoft.CloudPC/RoleAssignments/Update",
                    "Microsoft.CloudPC/RoleAssignments/Delete",
                    "Microsoft.CloudPC/Roles/Read",
                    "Microsoft.CloudPC/SelfServiceSettings/Read",
                    "Microsoft.CloudPC/SelfServiceSettings/Update"
                ],
                "condition": null
            }
        ]
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


