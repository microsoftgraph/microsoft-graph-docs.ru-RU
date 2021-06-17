---
title: Получение directoryRole
description: Получение свойств объекта directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 997882a9385d9fa3c9f474b9d4fa6efc930af21f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991773"
---
# <a name="get-directoryrole"></a><span data-ttu-id="e007a-103">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="e007a-103">Get directoryRole</span></span>

<span data-ttu-id="e007a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e007a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e007a-105">Получение свойств объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="e007a-105">Retrieve the properties of a directoryRole object.</span></span>

<span data-ttu-id="e007a-106">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="e007a-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="e007a-107">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e007a-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="e007a-108">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="e007a-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="e007a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e007a-109">Permissions</span></span>
<span data-ttu-id="e007a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e007a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e007a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e007a-112">Permission type</span></span>      | <span data-ttu-id="e007a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e007a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e007a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e007a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e007a-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e007a-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e007a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e007a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e007a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e007a-117">Not supported.</span></span>    |
|<span data-ttu-id="e007a-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="e007a-118">Application</span></span> | <span data-ttu-id="e007a-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e007a-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e007a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e007a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-objectId}
GET /directoryRoles/roleTemplateId={role-templateId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e007a-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e007a-121">Optional query parameters</span></span>
<span data-ttu-id="e007a-122">Этот метод **не поддерживает** параметры [запроса OData](/graph/query-parameters) для настройки ответа (например, `$filter` здесь не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="e007a-122">This method does **not** support any [OData Query Parameters](/graph/query-parameters) to help customize the response (for example, `$filter` is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e007a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e007a-123">Request headers</span></span>
| <span data-ttu-id="e007a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="e007a-124">Name</span></span>       | <span data-ttu-id="e007a-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e007a-125">Type</span></span> | <span data-ttu-id="e007a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e007a-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e007a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e007a-127">Authorization</span></span>  | <span data-ttu-id="e007a-128">string</span><span class="sxs-lookup"><span data-stu-id="e007a-128">string</span></span>  | <span data-ttu-id="e007a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e007a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e007a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e007a-131">Request body</span></span>
<span data-ttu-id="e007a-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e007a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e007a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e007a-133">Response</span></span>

<span data-ttu-id="e007a-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e007a-134">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e007a-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="e007a-135">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-role-objectid"></a><span data-ttu-id="e007a-136">Пример 1. Определение роли каталога с помощью объекта role ObjectId</span><span class="sxs-lookup"><span data-stu-id="e007a-136">Example 1: Get the definition of a directory role using role objectId</span></span>
#### <a name="request"></a><span data-ttu-id="e007a-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e007a-137">Request</span></span>
<span data-ttu-id="e007a-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e007a-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e007a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e007a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830
```
# <a name="c"></a>[<span data-ttu-id="e007a-140">C#</span><span class="sxs-lookup"><span data-stu-id="e007a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e007a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e007a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e007a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e007a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e007a-143">Java</span><span class="sxs-lookup"><span data-stu-id="e007a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e007a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e007a-144">Response</span></span>
><span data-ttu-id="e007a-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e007a-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```


### <a name="example-2-get-the-definition-of-a-directory-role-using-role-templateid"></a><span data-ttu-id="e007a-146">Пример 2. Определение роли каталога с помощью шаблона roleId</span><span class="sxs-lookup"><span data-stu-id="e007a-146">Example 2: Get the definition of a directory role using role templateId</span></span>
#### <a name="request"></a><span data-ttu-id="e007a-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="e007a-147">Request</span></span>
<span data-ttu-id="e007a-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e007a-148">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="e007a-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="e007a-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b
```
# <a name="c"></a>[<span data-ttu-id="e007a-150">C#</span><span class="sxs-lookup"><span data-stu-id="e007a-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e007a-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e007a-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e007a-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e007a-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e007a-153">Java</span><span class="sxs-lookup"><span data-stu-id="e007a-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e007a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e007a-154">Response</span></span>
><span data-ttu-id="e007a-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e007a-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
