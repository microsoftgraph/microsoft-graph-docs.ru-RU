---
title: Перечисление объектов directoryRole
description: Перечисление ролей каталога, активированных в клиенте.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b34011e1ed208405f40e4a5a5be6af20e1f217fe
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334425"
---
# <a name="list-directoryroles"></a><span data-ttu-id="599e1-103">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="599e1-103">List directoryRoles</span></span>

<span data-ttu-id="599e1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="599e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="599e1-105">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="599e1-105">List the directory roles that are activated in the tenant.</span></span>

<span data-ttu-id="599e1-106">Эта операция возвращает только роли, которые были активированы.</span><span class="sxs-lookup"><span data-stu-id="599e1-106">This operation only returns roles that have been activated.</span></span> <span data-ttu-id="599e1-107">Роль активируется, когда администратор активирует роль с помощью API [Activat directoryRole.](directoryrole-post-directoryroles.md)</span><span class="sxs-lookup"><span data-stu-id="599e1-107">A role becomes activated when an admin activates the role using the [Activate directoryRole](directoryrole-post-directoryroles.md) API.</span></span> <span data-ttu-id="599e1-108">Не все встроенные роли изначально активируются.</span><span class="sxs-lookup"><span data-stu-id="599e1-108">Not all built-in roles are initially activated.</span></span> 

<span data-ttu-id="599e1-109">При назначении роли с помощью портала Azure шаг активации роли неявно делается от имени администратора.</span><span class="sxs-lookup"><span data-stu-id="599e1-109">When assigning a role using the Azure portal, the role activation step is implicitly done on the admin's behalf.</span></span> <span data-ttu-id="599e1-110">Чтобы получить полный список ролей, доступных в Azure AD, используйте [list directoryRoleTemplates.](directoryroletemplate-list.md)</span><span class="sxs-lookup"><span data-stu-id="599e1-110">To get the full list of roles that are available in Azure AD, use [List directoryRoleTemplates](directoryroletemplate-list.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="599e1-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="599e1-111">Permissions</span></span>
<span data-ttu-id="599e1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="599e1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="599e1-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="599e1-114">Permission type</span></span>      | <span data-ttu-id="599e1-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="599e1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="599e1-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="599e1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="599e1-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="599e1-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="599e1-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="599e1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="599e1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="599e1-119">Not supported.</span></span>    |
|<span data-ttu-id="599e1-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="599e1-120">Application</span></span> | <span data-ttu-id="599e1-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599e1-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="599e1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="599e1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="599e1-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="599e1-123">Optional query parameters</span></span>
<span data-ttu-id="599e1-124">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="599e1-124">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="599e1-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="599e1-125">Request headers</span></span>
| <span data-ttu-id="599e1-126">Имя</span><span class="sxs-lookup"><span data-stu-id="599e1-126">Name</span></span>       | <span data-ttu-id="599e1-127">Тип</span><span class="sxs-lookup"><span data-stu-id="599e1-127">Type</span></span> | <span data-ttu-id="599e1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="599e1-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="599e1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="599e1-129">Authorization</span></span>  | <span data-ttu-id="599e1-130">string</span><span class="sxs-lookup"><span data-stu-id="599e1-130">string</span></span>  | <span data-ttu-id="599e1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="599e1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="599e1-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="599e1-133">Request body</span></span>
<span data-ttu-id="599e1-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="599e1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="599e1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="599e1-135">Response</span></span>

<span data-ttu-id="599e1-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="599e1-136">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="599e1-137">Пример</span><span class="sxs-lookup"><span data-stu-id="599e1-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="599e1-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="599e1-138">Request</span></span>
<span data-ttu-id="599e1-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="599e1-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="599e1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="599e1-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles
```
# <a name="c"></a>[<span data-ttu-id="599e1-141">C#</span><span class="sxs-lookup"><span data-stu-id="599e1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="599e1-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="599e1-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="599e1-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="599e1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="599e1-144">Java</span><span class="sxs-lookup"><span data-stu-id="599e1-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="599e1-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="599e1-145">Response</span></span>
<span data-ttu-id="599e1-p105">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="599e1-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles",
  "value": [
    {
      "id": "9ed3a0c4-53e1-498c-ab4d-2473476fde14",
      "deletedDateTime": null,
      "description": "Can manage all aspects of Azure AD and Microsoft services that use Azure AD identities.",
      "displayName": "Global Administrator",
      "roleTemplateId": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "id": "f8e85ed8-f66f-4058-b170-3efae8b9c6e5",
      "deletedDateTime": null,
      "description": "Device Administrators",
      "displayName": "Azure AD Joined Device Local Administrator",
      "roleTemplateId": "9f06204d-73c1-4d4c-880a-6edb90606fd8"
    },
    {
      "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
      "deletedDateTime": null,
      "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
      "displayName": "Directory Readers",
      "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
