---
title: Создание accessPackageResourceRoleScope
description: Создайте новый accessPackageResourceRoleScope для добавления роли ресурса в пакет доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6b4abe2f9c2c0060e97560a26c22d19ed53e01b7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466966"
---
# <a name="create-accesspackageresourcerolescope"></a><span data-ttu-id="3bcb7-103">Создание accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="3bcb7-103">Create accessPackageResourceRoleScope</span></span>

<span data-ttu-id="3bcb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bcb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bcb7-105">Создайте [новый accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) для добавления роли ресурса в пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-105">Create a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) for adding a resource role to an access package.</span></span> <span data-ttu-id="3bcb7-106">Ресурс пакета доступа для группы, приложения или сайта SharePoint Online уже должен существовать в каталоге пакетов доступа и **originId** для роли ресурса, извлеченной из списка ролей [ресурса.](accesspackagecatalog-list-accesspackageresourceroles.md)</span><span class="sxs-lookup"><span data-stu-id="3bcb7-106">The access package resource, for a group, an app, or a SharePoint Online site, must already exist in the access package catalog, and the **originId** for the resource role retrieved from the [list of the resource roles](accesspackagecatalog-list-accesspackageresourceroles.md).</span></span> <span data-ttu-id="3bcb7-107">После добавления области роли ресурсов в пакет доступа пользователь получит эту роль ресурса с помощью любых назначений пакета текущих и будущих пакетов доступа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-107">Once you add the resource role scope to the access package, the user will receive this resource role through any current and future access package assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bcb7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bcb7-108">Permissions</span></span>

<span data-ttu-id="3bcb7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bcb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bcb7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bcb7-111">Permission type</span></span>                        | <span data-ttu-id="3bcb7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bcb7-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3bcb7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bcb7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bcb7-114">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bcb7-114">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3bcb7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bcb7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bcb7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-116">Not supported.</span></span> |
| <span data-ttu-id="3bcb7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3bcb7-117">Application</span></span>                            | <span data-ttu-id="3bcb7-118">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bcb7-118">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bcb7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bcb7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
```

## <a name="request-headers"></a><span data-ttu-id="3bcb7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bcb7-120">Request headers</span></span>

| <span data-ttu-id="3bcb7-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3bcb7-121">Name</span></span>          | <span data-ttu-id="3bcb7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3bcb7-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3bcb7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bcb7-123">Authorization</span></span> | <span data-ttu-id="3bcb7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3bcb7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3bcb7-126">Content-Type</span></span>  | <span data-ttu-id="3bcb7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3bcb7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bcb7-129">Request body</span></span>

<span data-ttu-id="3bcb7-130">В теле запроса устройте представление JSON объекта [accessPackageResourceRoleScope.](../resources/accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="3bcb7-130">In the request body, supply a JSON representation of an [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object.</span></span>  <span data-ttu-id="3bcb7-131">Включайте в объект связи с объектом [accessPackageResourceRole,](../resources/accesspackageresourcerole.md) который можно получить из запроса на список ролей ресурсов пакета доступа ресурса ресурса в каталоге, [](accesspackagecatalog-list-accesspackageresources.md) и [объект accessPackageResourceScope,](../resources/accesspackageresourcescope.md) который можно получить из запроса на список ресурсов пакета доступа с [](accesspackagecatalog-list-accesspackageresourceroles.md) `$expand=accessPackageResourceScopes` .</span><span class="sxs-lookup"><span data-stu-id="3bcb7-131">Include in the object the relationships to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) object, which can be obtained from a request to [list access package resource roles of a resource in a catalog](accesspackagecatalog-list-accesspackageresourceroles.md), and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md) object, which can be obtained from a request to [list access package resources](accesspackagecatalog-list-accesspackageresources.md) with `$expand=accessPackageResourceScopes`.</span></span>

## <a name="response"></a><span data-ttu-id="3bcb7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bcb7-132">Response</span></span>

<span data-ttu-id="3bcb7-133">В случае успешной работы этот метод возвращает код ответа из 200 серий и новый [объект accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-133">If successful, this method returns a 200-series response code and a new [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3bcb7-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="3bcb7-134">Examples</span></span>

### <a name="example-1-add-group-membership-as-a-resource-role-to-an-access-package"></a><span data-ttu-id="3bcb7-135">Пример 1. Добавление членства в группе в качестве роли ресурса в пакет доступа</span><span class="sxs-lookup"><span data-stu-id="3bcb7-135">Example 1: Add group membership as a resource role to an access package</span></span>

#### <a name="request"></a><span data-ttu-id="3bcb7-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bcb7-136">Request</span></span>

<span data-ttu-id="3bcb7-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-137">The following is an example of the request.</span></span>  <span data-ttu-id="3bcb7-138">До этого запроса ресурс пакета доступа для группы уже должен быть добавлен в каталог пакета доступа, содержащий `1d08498d-72a1-403f-8511-6b1f875746a0` `b31fe1f1-3651-488f-bd9a-1711887fd4ca` этот пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-138">Prior to this request, the access package resource `1d08498d-72a1-403f-8511-6b1f875746a0` for the group `b31fe1f1-3651-488f-bd9a-1711887fd4ca` must already have been added to the access package catalog containing this access package.</span></span>  <span data-ttu-id="3bcb7-139">Этот ресурс можно было бы добавить в каталог, [создав запрос ресурса](accesspackageresourcerequest-post.md)пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-139">The resource could have been added to the catalog by [creating an access package resource request](accesspackageresourcerequest-post.md).</span></span>

# <a name="http"></a>[<span data-ttu-id="3bcb7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bcb7-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackage"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole":{
    "originId":"Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource":{"id":"1d08498d-72a1-403f-8511-6b1f875746a0","resourceType":"O365 Group","originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"}
  },
 "accessPackageResourceScope":{
   "originId":"b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem":"AadGroup"
 }
}
```
# <a name="c"></a>[<span data-ttu-id="3bcb7-141">C#</span><span class="sxs-lookup"><span data-stu-id="3bcb7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bcb7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bcb7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bcb7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bcb7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bcb7-144">Java</span><span class="sxs-lookup"><span data-stu-id="3bcb7-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3bcb7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bcb7-145">Response</span></span>

<span data-ttu-id="3bcb7-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-146">The following is an example of the response.</span></span>

> <span data-ttu-id="3bcb7-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-147">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResourceRoleScopes/$entity",
    "id": "ad5c7636-e481-4528-991f-198e3b38dd56_ffd4004a-f4a9-4b22-b027-759e55c0d1db",
    "createdBy": "admin@example.com",
    "createdDateTime": "2019-12-11T01:35:26.4754081Z",
    "modifiedBy": "admin@example.com",
    "modifiedDateTime": "2019-12-11T01:35:26.4754081Z"
}
```

### <a name="example-2-add-a-sharepoint-online-site-role-to-an-access-package"></a><span data-ttu-id="3bcb7-148">Пример 2. Добавление роли SharePoint веб-сайта в пакет доступа</span><span class="sxs-lookup"><span data-stu-id="3bcb7-148">Example 2: Add a SharePoint Online site role to an access package</span></span>

#### <a name="request"></a><span data-ttu-id="3bcb7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bcb7-149">Request</span></span>

<span data-ttu-id="3bcb7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-150">The following is an example of the request.</span></span>  <span data-ttu-id="3bcb7-151">Ресурс пакета доступа для сайта уже должен быть добавлен в каталог пакетов доступа, содержащий этот пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-151">The access package resource for the site must already have been added to the access package catalog containing this access package.</span></span>


# <a name="http"></a>[<span data-ttu-id="3bcb7-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bcb7-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerolescope_from_accesspackage2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes
Content-type: application/json

{
    "accessPackageResourceRole": {
        "originId": "4",
        "originSystem": "SharePointOnline",
        "accessPackageResource": {
            "id": "53c71803-a0a8-4777-aecc-075de8ee3991"
        }
    },
    "accessPackageResourceScope": {
        "id": "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33",
        "originId": "https://microsoft.sharepoint.com/portals/Community",
        "originSystem": "SharePointOnline"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="3bcb7-153">C#</span><span class="sxs-lookup"><span data-stu-id="3bcb7-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageresourcerolescope-from-accesspackage2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bcb7-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bcb7-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageresourcerolescope-from-accesspackage2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bcb7-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bcb7-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageresourcerolescope-from-accesspackage2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bcb7-156">Java</span><span class="sxs-lookup"><span data-stu-id="3bcb7-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageresourcerolescope-from-accesspackage2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3bcb7-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bcb7-157">Response</span></span>

<span data-ttu-id="3bcb7-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-158">The following is an example of the response.</span></span>

> <span data-ttu-id="3bcb7-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3bcb7-159">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "id": "6646a29e-da03-49f6-bcd9-dec124492de3_5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRoleScope",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
