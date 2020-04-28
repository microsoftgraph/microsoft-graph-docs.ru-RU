---
title: Получение unifiedRoleAssignmentMultiple
description: Получение свойств и связей объекта Унифиедролеассигнментмултипле.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 01f59e08a298fd5bf3e630de1cb562bc6de810a4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215835"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="31919-103">Получение unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="31919-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="31919-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31919-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31919-105">Получение свойств и связей объекта [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="31919-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="31919-106">Используйте этот объект для получения назначений ролей в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="31919-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="31919-107">Для других приложений Микрсофт 365 (например, Azure AD) используйте [унифиедролеассигнмент](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31919-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="31919-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31919-108">Permissions</span></span>

<span data-ttu-id="31919-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31919-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="31919-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31919-111">Permission type</span></span> | <span data-ttu-id="31919-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31919-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="31919-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31919-113">Delegated (work or school account)</span></span> | <span data-ttu-id="31919-114">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="31919-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="31919-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31919-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31919-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31919-116">Not supported.</span></span> |
| <span data-ttu-id="31919-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31919-117">Application</span></span> | <span data-ttu-id="31919-118">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="31919-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31919-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31919-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="31919-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="31919-120">Optional query parameters</span></span>

<span data-ttu-id="31919-121">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="31919-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="31919-122">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="31919-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="31919-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31919-123">Request headers</span></span>

| <span data-ttu-id="31919-124">Имя</span><span class="sxs-lookup"><span data-stu-id="31919-124">Name</span></span>  | <span data-ttu-id="31919-125">Описание</span><span class="sxs-lookup"><span data-stu-id="31919-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="31919-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31919-126">Authorization</span></span> | <span data-ttu-id="31919-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31919-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31919-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="31919-129">Request body</span></span>

<span data-ttu-id="31919-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="31919-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31919-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="31919-131">Response</span></span>

<span data-ttu-id="31919-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [унифиедролеассигнментмултипле](../resources/unifiedroleassignmentmultiple.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31919-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31919-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="31919-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="31919-134">Пример 1: получение Ролеассигнментмултипле с областью действия каталога в Intune</span><span class="sxs-lookup"><span data-stu-id="31919-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="31919-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="31919-135">Request</span></span>

<span data-ttu-id="31919-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31919-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="31919-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="31919-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="31919-138">C#</span><span class="sxs-lookup"><span data-stu-id="31919-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31919-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31919-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31919-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31919-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="31919-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="31919-141">Response</span></span>

<span data-ttu-id="31919-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31919-142">The following is an example of the response.</span></span>
> <span data-ttu-id="31919-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31919-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="31919-145">Пример 2: получение Ролеассигнментмултипле с областью действия в каталоге с`$expand`</span><span class="sxs-lookup"><span data-stu-id="31919-145">Example 2: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="31919-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="31919-146">Request</span></span>

<span data-ttu-id="31919-147">Ниже приведен пример запроса с параметром `$expand` Query.</span><span class="sxs-lookup"><span data-stu-id="31919-147">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="31919-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="31919-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="31919-149">C#</span><span class="sxs-lookup"><span data-stu-id="31919-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31919-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31919-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31919-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31919-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="31919-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="31919-152">Response</span></span>

<span data-ttu-id="31919-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="31919-153">The following is an example of the response.</span></span>
> <span data-ttu-id="31919-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31919-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
