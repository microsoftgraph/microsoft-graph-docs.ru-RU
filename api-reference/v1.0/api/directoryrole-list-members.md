---
title: Список участников роли каталога
description: Извлечение списка директоров, которые назначены роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 878c99489b2faf1c4c079958491b64366945a67c
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854245"
---
# <a name="list-members-of-a-directory-role"></a><span data-ttu-id="7f92d-103">Список участников роли каталога</span><span class="sxs-lookup"><span data-stu-id="7f92d-103">List members of a directory role</span></span>

<span data-ttu-id="7f92d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f92d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7f92d-105">Извлечение списка директоров, которые назначены роли каталога.</span><span class="sxs-lookup"><span data-stu-id="7f92d-105">Retrieve the list of principals that are assigned to the directory role.</span></span> 

<span data-ttu-id="7f92d-106">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="7f92d-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="7f92d-107">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7f92d-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="7f92d-108">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="7f92d-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f92d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f92d-109">Permissions</span></span>
<span data-ttu-id="7f92d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f92d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7f92d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f92d-112">Permission type</span></span>      | <span data-ttu-id="7f92d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f92d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f92d-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f92d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7f92d-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7f92d-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7f92d-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f92d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f92d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f92d-117">Not supported.</span></span>    |
|<span data-ttu-id="7f92d-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f92d-118">Application</span></span> | <span data-ttu-id="7f92d-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f92d-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="7f92d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f92d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-objectId}/members
GET /directoryRoles/roleTemplateId={role-templateId}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f92d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7f92d-121">Optional query parameters</span></span>
<span data-ttu-id="7f92d-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7f92d-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7f92d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f92d-123">Request headers</span></span>
| <span data-ttu-id="7f92d-124">Имя</span><span class="sxs-lookup"><span data-stu-id="7f92d-124">Name</span></span>       | <span data-ttu-id="7f92d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="7f92d-125">Type</span></span> | <span data-ttu-id="7f92d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="7f92d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f92d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f92d-127">Authorization</span></span>  | <span data-ttu-id="7f92d-128">string</span><span class="sxs-lookup"><span data-stu-id="7f92d-128">string</span></span>  | <span data-ttu-id="7f92d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f92d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f92d-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f92d-131">Request body</span></span>
<span data-ttu-id="7f92d-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f92d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f92d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f92d-133">Response</span></span>

<span data-ttu-id="7f92d-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f92d-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7f92d-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="7f92d-135">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-role-objectid"></a><span data-ttu-id="7f92d-136">Пример 1. Получить членов роли каталога с помощью объекта role ObjectId</span><span class="sxs-lookup"><span data-stu-id="7f92d-136">Example 1: Get the members of a directory role using role objectId</span></span>

#### <a name="request"></a><span data-ttu-id="7f92d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f92d-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f92d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f92d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_objectid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="7f92d-139">C#</span><span class="sxs-lookup"><span data-stu-id="7f92d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f92d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f92d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f92d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f92d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f92d-142">Java</span><span class="sxs-lookup"><span data-stu-id="7f92d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7f92d-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f92d-143">Response</span></span>
> <span data-ttu-id="7f92d-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7f92d-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2-get-the-members-of-a-directory-role-using-role-templateid"></a><span data-ttu-id="7f92d-145">Пример 2. Получить членов роли каталога с помощью шаблона ролейId</span><span class="sxs-lookup"><span data-stu-id="7f92d-145">Example 2: Get the members of a directory role using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="7f92d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f92d-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f92d-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f92d-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="7f92d-148">C#</span><span class="sxs-lookup"><span data-stu-id="7f92d-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f92d-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f92d-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f92d-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f92d-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f92d-151">Java</span><span class="sxs-lookup"><span data-stu-id="7f92d-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7f92d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f92d-152">Response</span></span>
><span data-ttu-id="7f92d-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7f92d-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
