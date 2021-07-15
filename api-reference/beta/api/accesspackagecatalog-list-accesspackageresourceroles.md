---
title: Список accessPackageResourceRoles
description: Извлечение списка объектов accessPackageResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 45e8f2364997518bbc47d61906a9e3f4986e64e6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439272"
---
# <a name="list-accesspackageresourceroles"></a><span data-ttu-id="055d0-103">Список accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="055d0-103">List accessPackageResourceRoles</span></span>

<span data-ttu-id="055d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="055d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="055d0-105">Извлечение списка [объектов accessPackageResourceRole](../resources/accesspackageresourcerole.md) [accessPackageResource](../resources/accesspackageresource.md) в [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="055d0-105">Retrieve a list of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects of an [accessPackageResource](../resources/accesspackageresource.md) in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span> <span data-ttu-id="055d0-106">Ресурс должен был быть добавлен в каталог путем [создания accessPackageResourceRequest.](accesspackageresourcerequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="055d0-106">The resource should have been added to the catalog by [creating an accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span> <span data-ttu-id="055d0-107">Этот список ролей может быть использован звонивцом для выбора роли, которая необходима при создании [accessPackageResourceRoleScope.](accesspackage-post-accesspackageresourcerolescopes.md)</span><span class="sxs-lookup"><span data-stu-id="055d0-107">This list of roles can then be used by the caller to select a role, which is needed when subsequently [creating an accessPackageResourceRoleScope](accesspackage-post-accesspackageresourcerolescopes.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="055d0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="055d0-108">Permissions</span></span>

<span data-ttu-id="055d0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="055d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="055d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="055d0-111">Permission type</span></span>                        | <span data-ttu-id="055d0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="055d0-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="055d0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="055d0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="055d0-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="055d0-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="055d0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="055d0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="055d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="055d0-116">Not supported.</span></span> |
| <span data-ttu-id="055d0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="055d0-117">Application</span></span>                            | <span data-ttu-id="055d0-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="055d0-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="055d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="055d0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/accessPackageResourceRoles?$filter=(originSystem+eq+%27{originSystemType}%27+and+accessPackageResource/id+eq+%27{resourceId}%27)&$expand=accessPackageResource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="055d0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="055d0-120">Optional query parameters</span></span>

<span data-ttu-id="055d0-121">Этот метод использует параметры запроса OData для построения ответа.</span><span class="sxs-lookup"><span data-stu-id="055d0-121">This method uses OData query parameters to construct the response.</span></span> <span data-ttu-id="055d0-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="055d0-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="055d0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="055d0-123">Request headers</span></span>

| <span data-ttu-id="055d0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="055d0-124">Name</span></span>      |<span data-ttu-id="055d0-125">Описание</span><span class="sxs-lookup"><span data-stu-id="055d0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="055d0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="055d0-126">Authorization</span></span> | <span data-ttu-id="055d0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="055d0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="055d0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="055d0-129">Request body</span></span>

<span data-ttu-id="055d0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="055d0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="055d0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="055d0-131">Response</span></span>

<span data-ttu-id="055d0-132">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResourceRole](../resources/accesspackageresourcerole.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="055d0-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceRole](../resources/accesspackageresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="055d0-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="055d0-133">Examples</span></span>

### <a name="example-1-retrieving-the-roles-of-a-resource-for-a-group"></a><span data-ttu-id="055d0-134">Пример 1. Ирисовка ролей ресурса для группы</span><span class="sxs-lookup"><span data-stu-id="055d0-134">Example 1: Retrieving the roles of a resource for a group</span></span>

#### <a name="request"></a><span data-ttu-id="055d0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="055d0-135">Request</span></span>

<span data-ttu-id="055d0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="055d0-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="055d0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="055d0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)&$expand=accessPackageResource
```
# <a name="c"></a>[<span data-ttu-id="055d0-138">C#</span><span class="sxs-lookup"><span data-stu-id="055d0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="055d0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="055d0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="055d0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="055d0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="055d0-141">Java</span><span class="sxs-lookup"><span data-stu-id="055d0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="055d0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="055d0-142">Response</span></span>

<span data-ttu-id="055d0-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="055d0-143">The following is an example of the response.</span></span>

> <span data-ttu-id="055d0-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="055d0-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "displayName": "Member",
      "description": "description-value",
      "originId": "originId-value",
      "originSystem": "originSystem-value"
    }
  ]
}
```

### <a name="example-2-retrieve-the-roles-of-a-resource-for-a-sharepoint-online-site"></a><span data-ttu-id="055d0-145">Пример 2. Извлечение ролей ресурса для сайта SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="055d0-145">Example 2: Retrieve the roles of a resource for a SharePoint Online site</span></span>

<span data-ttu-id="055d0-146">Это пример получения ролей ресурса для получения **originId** каждой роли.</span><span class="sxs-lookup"><span data-stu-id="055d0-146">This is an example of retrieving the roles of a resource, to obtain the **originId** of each role.</span></span>  <span data-ttu-id="055d0-147">Это будет использоваться после того, как SharePoint сайт Online был добавлен в каталог в качестве ресурса, так как **originId** роли необходим для добавления роли в пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="055d0-147">This would be used after a SharePoint Online site has been added as a resource to the catalog, as the **originId** of a role is needed to add the role to an access package.</span></span>

#### <a name="request"></a><span data-ttu-id="055d0-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="055d0-148">Request</span></span>

<span data-ttu-id="055d0-149">Ниже приводится пример запроса для получения ролей определенного ресурса **53c71803-a0a8-4777-aecc-075de8ee3991,** который имеет **происхождениеSystem** of **SharePointOnline** и расположен в каталоге **beedadfe-01d5-4025-910b-84abb936997**.</span><span class="sxs-lookup"><span data-stu-id="055d0-149">The following is an example of the request, to retrieve the roles of a particular resource **53c71803-a0a8-4777-aecc-075de8ee3991** which has an **originSystem** of **SharePointOnline** and is located in catalog **beedadfe-01d5-4025-910b-84abb9369997**.</span></span>



# <a name="http"></a>[<span data-ttu-id="055d0-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="055d0-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourceroles2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/beedadfe-01d5-4025-910b-84abb9369997/accessPackageResourceRoles?$filter=(originSystem+eq+%27SharePointOnline%27+and+accessPackageResource/id+eq+%2753c71803-a0a8-4777-aecc-075de8ee3991%27)&$select=displayName,originId
```
# <a name="c"></a>[<span data-ttu-id="055d0-151">C#</span><span class="sxs-lookup"><span data-stu-id="055d0-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourceroles2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="055d0-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="055d0-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourceroles2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="055d0-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="055d0-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourceroles2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="055d0-154">Java</span><span class="sxs-lookup"><span data-stu-id="055d0-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourceroles2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="055d0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="055d0-155">Response</span></span>

<span data-ttu-id="055d0-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="055d0-156">The following is an example of the response.</span></span>  <span data-ttu-id="055d0-157">**DisplayName** является таким же, как показано в представлении SharePoint Online сайта, и **originId** — это идентификатор, установленный SharePoint Online для роли.</span><span class="sxs-lookup"><span data-stu-id="055d0-157">The **displayName** is the same as shown in the SharePoint Online view of a site, and the **originId** is the underlying identifier established by SharePoint Online for the role.</span></span>

> <span data-ttu-id="055d0-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="055d0-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "displayName": "Contributors",
        "originId": "4"
    },
    {
        "displayName": "Creators",
        "originId": "3"
    },
    {
        "displayName": "Viewers",
        "originId": "5"
    }
  ]
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
