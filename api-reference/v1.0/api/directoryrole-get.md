---
title: Получение directoryRole
description: Получение свойств объекта directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 368503c10b809571dcef4cef5265a86a37044031
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522761"
---
# <a name="get-directoryrole"></a><span data-ttu-id="36208-103">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="36208-103">Get directoryRole</span></span>

<span data-ttu-id="36208-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36208-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36208-105">Получение свойств объекта [directoryRole](../resources/directoryrole.md) .</span><span class="sxs-lookup"><span data-stu-id="36208-105">Retrieve the properties of a [directoryRole](../resources/directoryrole.md) object.</span></span> <span data-ttu-id="36208-106">Для успешного ответа роль должна быть активирована в клиенте.</span><span class="sxs-lookup"><span data-stu-id="36208-106">The role must be activated in tenant for a successful response.</span></span>

> [!Note]
> <span data-ttu-id="36208-107">С этим API можно использовать как идентификатор объекта, так и идентификатор шаблона **directoryRole** .</span><span class="sxs-lookup"><span data-stu-id="36208-107">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="36208-108">Неизменяемый идентификатор шаблона встроенной роли, который можно просмотреть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="36208-108">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="36208-109">Дополнительные сведения: [идентификаторы шаблонов ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="36208-109">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="36208-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36208-110">Permissions</span></span>
<span data-ttu-id="36208-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36208-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36208-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36208-113">Permission type</span></span>      | <span data-ttu-id="36208-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36208-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36208-115">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36208-115">Delegated (work or school account)</span></span> | <span data-ttu-id="36208-116">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="36208-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36208-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36208-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36208-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36208-118">Not supported.</span></span>    |
|<span data-ttu-id="36208-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="36208-119">Application</span></span> | <span data-ttu-id="36208-120">Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="36208-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36208-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36208-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36208-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="36208-122">Optional query parameters</span></span>
<span data-ttu-id="36208-123">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="36208-123">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="36208-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36208-124">Request headers</span></span>
| <span data-ttu-id="36208-125">Имя</span><span class="sxs-lookup"><span data-stu-id="36208-125">Name</span></span>       | <span data-ttu-id="36208-126">Тип</span><span class="sxs-lookup"><span data-stu-id="36208-126">Type</span></span> | <span data-ttu-id="36208-127">Описание</span><span class="sxs-lookup"><span data-stu-id="36208-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="36208-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="36208-128">Authorization</span></span>  | <span data-ttu-id="36208-129">string</span><span class="sxs-lookup"><span data-stu-id="36208-129">string</span></span>  | <span data-ttu-id="36208-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36208-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36208-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36208-132">Request body</span></span>
<span data-ttu-id="36208-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36208-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36208-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="36208-134">Response</span></span>

<span data-ttu-id="36208-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryRole](../resources/directoryrole.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36208-135">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="36208-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="36208-136">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-objectid"></a><span data-ttu-id="36208-137">Пример 1: получение определения роли каталога с помощью objectId</span><span class="sxs-lookup"><span data-stu-id="36208-137">Example 1: Get the definition of a directory role using objectId</span></span>
##### <a name="request"></a><span data-ttu-id="36208-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="36208-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36208-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="36208-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_objectId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda
```
# <a name="c"></a>[<span data-ttu-id="36208-140">C#</span><span class="sxs-lookup"><span data-stu-id="36208-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36208-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36208-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36208-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36208-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36208-143">Java</span><span class="sxs-lookup"><span data-stu-id="36208-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36208-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="36208-144">Response</span></span>
><span data-ttu-id="36208-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36208-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
    "id": "23f3b4b4-8a29-4420-8052-e4950273bbda",
    "deletedDateTime": null,
    "description": "Can read sign-in and audit reports.",
    "displayName": "Reports Reader",
    "roleTemplateId": "4a5d8f65-41da-4de4-8968-e035b65339cf"
}
```

### <a name="example-2-get-the-definition-of-a-directory-role-using-templateid"></a><span data-ttu-id="36208-146">Пример 2: получение определения роли каталога с помощью templateId</span><span class="sxs-lookup"><span data-stu-id="36208-146">Example 2: Get the definition of a directory role using templateId</span></span>
##### <a name="request"></a><span data-ttu-id="36208-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="36208-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36208-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="36208-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf
```
# <a name="c"></a>[<span data-ttu-id="36208-149">C#</span><span class="sxs-lookup"><span data-stu-id="36208-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36208-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36208-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36208-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36208-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36208-152">Java</span><span class="sxs-lookup"><span data-stu-id="36208-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36208-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="36208-153">Response</span></span>
><span data-ttu-id="36208-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36208-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
    "id": "23f3b4b4-8a29-4420-8052-e4950273bbda",
    "deletedDateTime": null,
    "description": "Allows ability to read usage reports.",
    "displayName": "Reports Reader",
    "roleTemplateId": "4a5d8f65-41da-4de4-8968-e035b65339cf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
