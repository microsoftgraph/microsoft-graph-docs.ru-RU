---
title: Список участников роли каталога
description: Извлечение списка директоров, которые назначены роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2860e1c0d6293f13fa07df26e7b9493501ac8185
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448557"
---
# <a name="list-members-of-a-directory-role"></a><span data-ttu-id="cc2c3-103">Список участников роли каталога</span><span class="sxs-lookup"><span data-stu-id="cc2c3-103">List members of a directory role</span></span>

<span data-ttu-id="cc2c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc2c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc2c3-105">Извлечение списка директоров, которые назначены роли каталога.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-105">Retrieve the list of principals that are assigned to the directory role.</span></span> 

> [!Note]
> <span data-ttu-id="cc2c3-106">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="cc2c3-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="cc2c3-107">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="cc2c3-108">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="cc2c3-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc2c3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc2c3-109">Permissions</span></span>
<span data-ttu-id="cc2c3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc2c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cc2c3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc2c3-112">Permission type</span></span>      | <span data-ttu-id="cc2c3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc2c3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc2c3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc2c3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cc2c3-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc2c3-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc2c3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc2c3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc2c3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-117">Not supported.</span></span>    |
|<span data-ttu-id="cc2c3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc2c3-118">Application</span></span> | <span data-ttu-id="cc2c3-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc2c3-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="cc2c3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc2c3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cc2c3-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc2c3-121">Optional query parameters</span></span>
<span data-ttu-id="cc2c3-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cc2c3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc2c3-123">Request headers</span></span>
| <span data-ttu-id="cc2c3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cc2c3-124">Name</span></span>       | <span data-ttu-id="cc2c3-125">Тип</span><span class="sxs-lookup"><span data-stu-id="cc2c3-125">Type</span></span> | <span data-ttu-id="cc2c3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cc2c3-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cc2c3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc2c3-127">Authorization</span></span>  | <span data-ttu-id="cc2c3-128">string</span><span class="sxs-lookup"><span data-stu-id="cc2c3-128">string</span></span>  | <span data-ttu-id="cc2c3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc2c3-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc2c3-131">Request body</span></span>
<span data-ttu-id="cc2c3-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc2c3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc2c3-133">Response</span></span>

<span data-ttu-id="cc2c3-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="cc2c3-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc2c3-135">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-objectid"></a><span data-ttu-id="cc2c3-136">Пример 1. Получить членов роли каталога с помощью objectId</span><span class="sxs-lookup"><span data-stu-id="cc2c3-136">Example 1: Get the members of a directory role using objectId</span></span>

##### <a name="request"></a><span data-ttu-id="cc2c3-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc2c3-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cc2c3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc2c3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_objectid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="cc2c3-139">C#</span><span class="sxs-lookup"><span data-stu-id="cc2c3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc2c3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc2c3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc2c3-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc2c3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc2c3-142">Java</span><span class="sxs-lookup"><span data-stu-id="cc2c3-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc2c3-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc2c3-143">Response</span></span>
> <span data-ttu-id="cc2c3-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```
### <a name="example-2-get-the-members-of-a-directory-role-using-templateid"></a><span data-ttu-id="cc2c3-145">Пример 2. Получить членов роли каталога с помощью templateId</span><span class="sxs-lookup"><span data-stu-id="cc2c3-145">Example 2: Get the members of a directory role using templateId</span></span>

##### <a name="request"></a><span data-ttu-id="cc2c3-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc2c3-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cc2c3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc2c3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="cc2c3-148">C#</span><span class="sxs-lookup"><span data-stu-id="cc2c3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc2c3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc2c3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc2c3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc2c3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc2c3-151">Java</span><span class="sxs-lookup"><span data-stu-id="cc2c3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cc2c3-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc2c3-152">Response</span></span>
><span data-ttu-id="cc2c3-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cc2c3-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
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
