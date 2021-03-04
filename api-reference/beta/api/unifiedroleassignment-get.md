---
title: Get unifiedRoleAssignment
description: Извлечение свойств и связей объекта unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d3900e716926ca200a82ae56eee19819b8c2e80b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444877"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="6f399-103">Get unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6f399-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="6f399-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f399-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f399-105">Извлечение свойств и связей объекта [unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6f399-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f399-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f399-106">Permissions</span></span>

<span data-ttu-id="6f399-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f399-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f399-109">Permission type</span></span>      | <span data-ttu-id="6f399-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f399-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f399-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f399-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6f399-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6f399-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f399-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f399-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f399-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f399-114">Not supported.</span></span>    |
|<span data-ttu-id="6f399-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6f399-115">Application</span></span> | <span data-ttu-id="6f399-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f399-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f399-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f399-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f399-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6f399-118">Optional query parameters</span></span>

<span data-ttu-id="6f399-119">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6f399-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="6f399-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6f399-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f399-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f399-121">Request headers</span></span>

| <span data-ttu-id="6f399-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6f399-122">Name</span></span>      |<span data-ttu-id="6f399-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6f399-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6f399-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f399-124">Authorization</span></span> | <span data-ttu-id="6f399-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6f399-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f399-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f399-126">Request body</span></span>

<span data-ttu-id="6f399-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f399-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f399-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f399-128">Response</span></span>

<span data-ttu-id="6f399-129">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [unifiedRoleAssignment](../resources/unifiedroleassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6f399-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f399-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="6f399-130">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="6f399-131">Пример 1. Сведения о назначении ролей</span><span class="sxs-lookup"><span data-stu-id="6f399-131">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="6f399-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f399-132">Request</span></span>

<span data-ttu-id="6f399-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f399-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f399-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f399-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="6f399-135">C#</span><span class="sxs-lookup"><span data-stu-id="6f399-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f399-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f399-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f399-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f399-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f399-138">Java</span><span class="sxs-lookup"><span data-stu-id="6f399-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f399-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f399-139">Response</span></span>

<span data-ttu-id="6f399-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f399-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6f399-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f399-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="6f399-143">Пример 2. Сведения о назначении ролей с помощью `$expand`</span><span class="sxs-lookup"><span data-stu-id="6f399-143">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="6f399-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f399-144">Request</span></span>

<span data-ttu-id="6f399-145">Ниже приводится пример запроса с `$expand` параметром запроса.</span><span class="sxs-lookup"><span data-stu-id="6f399-145">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f399-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f399-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="6f399-147">C#</span><span class="sxs-lookup"><span data-stu-id="6f399-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f399-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f399-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f399-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f399-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f399-150">Java</span><span class="sxs-lookup"><span data-stu-id="6f399-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f399-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f399-151">Response</span></span>

<span data-ttu-id="6f399-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f399-152">The following is an example of the response.</span></span>
> <span data-ttu-id="6f399-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f399-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


