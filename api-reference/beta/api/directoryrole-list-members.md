---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9ae55125cf14c5636346afcd447d417f577d6c84
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118527"
---
# <a name="list-members"></a><span data-ttu-id="6283f-104">Список участников</span><span class="sxs-lookup"><span data-stu-id="6283f-104">List members</span></span>

<span data-ttu-id="6283f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6283f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6283f-p102">Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="6283f-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>

<span data-ttu-id="6283f-108">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="6283f-108">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="6283f-109">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6283f-109">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="6283f-110">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="6283f-110">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="6283f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6283f-111">Permissions</span></span>
<span data-ttu-id="6283f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6283f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6283f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6283f-114">Permission type</span></span>      | <span data-ttu-id="6283f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6283f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6283f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6283f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6283f-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6283f-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6283f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6283f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6283f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6283f-119">Not supported.</span></span>    |
|<span data-ttu-id="6283f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6283f-120">Application</span></span> | <span data-ttu-id="6283f-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6283f-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6283f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6283f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}/members
GET /directoryRoles/roleTemplateId={roleTemplateId}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6283f-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6283f-123">Optional query parameters</span></span>
<span data-ttu-id="6283f-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6283f-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6283f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6283f-125">Request headers</span></span>
| <span data-ttu-id="6283f-126">Имя</span><span class="sxs-lookup"><span data-stu-id="6283f-126">Name</span></span>       | <span data-ttu-id="6283f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6283f-127">Type</span></span> | <span data-ttu-id="6283f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6283f-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6283f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6283f-129">Authorization</span></span>  | <span data-ttu-id="6283f-130">string</span><span class="sxs-lookup"><span data-stu-id="6283f-130">string</span></span>  | <span data-ttu-id="6283f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6283f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6283f-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6283f-133">Request body</span></span>
<span data-ttu-id="6283f-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6283f-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6283f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6283f-135">Response</span></span>

<span data-ttu-id="6283f-136">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6283f-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="6283f-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="6283f-137">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-role-id"></a><span data-ttu-id="6283f-138">Пример 1. Получить членов роли каталога с помощью id роли</span><span class="sxs-lookup"><span data-stu-id="6283f-138">Example 1: Get the members of a directory role using role id</span></span>

#### <a name="request"></a><span data-ttu-id="6283f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6283f-139">Request</span></span>
<span data-ttu-id="6283f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6283f-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6283f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6283f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="6283f-142">C#</span><span class="sxs-lookup"><span data-stu-id="6283f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6283f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6283f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6283f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6283f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6283f-145">Java</span><span class="sxs-lookup"><span data-stu-id="6283f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6283f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6283f-146">Response</span></span>
> <span data-ttu-id="6283f-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6283f-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-the-members-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="6283f-148">Пример 2. Получить членов роли каталога с помощью roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="6283f-148">Example 2: Get the members of a directory role using roleTemplateId</span></span>

#### <a name="request"></a><span data-ttu-id="6283f-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="6283f-149">Request</span></span>
<span data-ttu-id="6283f-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6283f-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6283f-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="6283f-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="6283f-152">C#</span><span class="sxs-lookup"><span data-stu-id="6283f-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6283f-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6283f-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6283f-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6283f-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6283f-155">Java</span><span class="sxs-lookup"><span data-stu-id="6283f-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6283f-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="6283f-156">Response</span></span>
><span data-ttu-id="6283f-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6283f-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
