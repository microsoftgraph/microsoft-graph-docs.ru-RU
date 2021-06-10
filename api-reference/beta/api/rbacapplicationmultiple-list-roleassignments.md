---
title: Перечисление объектов unifiedRoleAssignmentMultiple
description: Извлечение свойств и связей объекта unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0a70bfab57b398e0ac904cee02411a7b7c665bf9
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869045"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="98357-103">Перечисление объектов unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="98357-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="98357-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98357-105">Получите список объектов [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="98357-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects for an RBAC provider.</span></span>

<span data-ttu-id="98357-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="98357-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="98357-107">облачный КОМПЬЮТЕР</span><span class="sxs-lookup"><span data-stu-id="98357-107">cloud PC</span></span> 
- <span data-ttu-id="98357-108">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="98357-108">device management (Intune)</span></span>

<span data-ttu-id="98357-109">Для других Microsoft 365 приложений (например, Azure AD) используйте [унифицированную системуRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="98357-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="98357-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98357-110">Permissions</span></span>

<span data-ttu-id="98357-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="98357-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="98357-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98357-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="98357-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="98357-113">Supported provider</span></span>      | <span data-ttu-id="98357-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98357-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="98357-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98357-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98357-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="98357-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="98357-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="98357-117">Cloud PC</span></span> | <span data-ttu-id="98357-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98357-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="98357-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98357-119">Not supported.</span></span> | <span data-ttu-id="98357-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98357-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="98357-121">Intune</span><span class="sxs-lookup"><span data-stu-id="98357-121">Intune</span></span> | <span data-ttu-id="98357-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98357-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="98357-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98357-123">Not supported.</span></span>| <span data-ttu-id="98357-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98357-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98357-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98357-125">HTTP request</span></span>

<span data-ttu-id="98357-126">Список назначений ролей для поставщика облачных ПК:</span><span class="sxs-lookup"><span data-stu-id="98357-126">To list role assignments for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/cloudPc/roleAssignments
```

<span data-ttu-id="98357-127">Список назначений ролей для поставщика Intune:</span><span class="sxs-lookup"><span data-stu-id="98357-127">To list role assignments for an Intune provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98357-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98357-128">Optional query parameters</span></span>
<span data-ttu-id="98357-129">Вы можете фильтровать свойства `roleDefinitionId` или `principalId` свойства.</span><span class="sxs-lookup"><span data-stu-id="98357-129">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="98357-130">Свойство `roleDefinitionId` может быть как ИД объекта роли, так и объектом шаблона ролей.</span><span class="sxs-lookup"><span data-stu-id="98357-130">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="98357-131">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="98357-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="98357-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98357-132">Request headers</span></span>

| <span data-ttu-id="98357-133">Имя</span><span class="sxs-lookup"><span data-stu-id="98357-133">Name</span></span> | <span data-ttu-id="98357-134">Описание</span><span class="sxs-lookup"><span data-stu-id="98357-134">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="98357-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98357-135">Authorization</span></span> | <span data-ttu-id="98357-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98357-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98357-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98357-138">Request body</span></span>

<span data-ttu-id="98357-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98357-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98357-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="98357-140">Response</span></span>

<span data-ttu-id="98357-141">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98357-141">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98357-142">Пример</span><span class="sxs-lookup"><span data-stu-id="98357-142">Example</span></span>

### <a name="example-1-list-the-role-assignments-for-a-specific-principal-for-an-intune-provider"></a><span data-ttu-id="98357-143">Пример 1. Список назначений ролей для определенного основного поставщика Intune</span><span class="sxs-lookup"><span data-stu-id="98357-143">Example 1: List the role assignments for a specific principal for an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="98357-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="98357-144">Request</span></span>

<span data-ttu-id="98357-145">Ниже приводится пример запроса:</span><span class="sxs-lookup"><span data-stu-id="98357-145">The following is an example of the request:</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="98357-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="98357-146">Response</span></span>

<span data-ttu-id="98357-147">Ниже приводится пример ответа:</span><span class="sxs-lookup"><span data-stu-id="98357-147">The following is an example of the response:</span></span>
> <span data-ttu-id="98357-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="98357-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```
### <a name="example-2-list-role-assignments-for-a-cloud-pc-provider"></a><span data-ttu-id="98357-149">Пример 2. Список назначений ролей для поставщика облачных ПК</span><span class="sxs-lookup"><span data-stu-id="98357-149">Example 2: List role assignments for a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="98357-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="98357-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="98357-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="98357-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
```
# <a name="c"></a>[<span data-ttu-id="98357-152">C#</span><span class="sxs-lookup"><span data-stu-id="98357-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98357-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98357-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98357-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98357-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98357-155">Java</span><span class="sxs-lookup"><span data-stu-id="98357-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98357-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="98357-156">Response</span></span>

> <span data-ttu-id="98357-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98357-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "value": [
        {
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
        },
        {
            "id": "fad74173-3fe3-4e64-9a80-297bdad2b36e",
            "description": null,
            "displayName": "My test role assignment 2",
            "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "principalIds": [
                "8e811502-ebda-4782-8f81-071d17f0f892",
            ],
            "directoryScopeIds": [
                "/"
            ],
            "appScopeIds": []
        }
    ]
}
```

### <a name="example-3-list-role-assignments-for-specific-role-of-a-cloud-pc-provider"></a><span data-ttu-id="98357-159">Пример 3. Список назначений ролей для определенной роли поставщика облачных ПК</span><span class="sxs-lookup"><span data-stu-id="98357-159">Example 3: List role assignments for specific role of a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="98357-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="98357-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="98357-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="98357-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments?$filter=roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'
```
# <a name="c"></a>[<span data-ttu-id="98357-162">C#</span><span class="sxs-lookup"><span data-stu-id="98357-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98357-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98357-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98357-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98357-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98357-165">Java</span><span class="sxs-lookup"><span data-stu-id="98357-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98357-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="98357-166">Response</span></span>

> <span data-ttu-id="98357-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98357-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments",
    "value": [{
        "id": "ed9e247f-f23b-4d72-9e8c-97fa6f385246",
        "description": "",
        "displayName": "test",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["689c9051-77ff-4f14-9b39-3d22de07321a"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "3d8e564b-761a-4b32-8f50-63d555f7bc00",
        "description": "test1",
        "displayName": "AssignmentTest",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["0ec7855b-4057-4b7c-9217-09ee9bf4dfd7"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "f36a3269-d03d-4d33-81e7-190bded40ad2",
        "description": "",
        "displayName": "test3",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["e4ea53cf-cdd6-46b5-bf38-570033a0fba3"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }]
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


