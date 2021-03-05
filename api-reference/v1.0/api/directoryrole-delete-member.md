---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c5f074b99260154db0d5e9f725a2082c4980af91
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448565"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="33acf-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="33acf-103">Remove directory role member</span></span>

<span data-ttu-id="33acf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33acf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33acf-105">Удаление члена из [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="33acf-105">Remove a member from a [directoryRole](../resources/directoryrole.md).</span></span>

> [!Note]
> <span data-ttu-id="33acf-106">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="33acf-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="33acf-107">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="33acf-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="33acf-108">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="33acf-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="33acf-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33acf-109">Permissions</span></span>

<span data-ttu-id="33acf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33acf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="33acf-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33acf-112">Permission type</span></span>      | <span data-ttu-id="33acf-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33acf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33acf-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33acf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="33acf-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33acf-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33acf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33acf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33acf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33acf-117">Not supported.</span></span>    |
|<span data-ttu-id="33acf-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33acf-118">Application</span></span> | <span data-ttu-id="33acf-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="33acf-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="33acf-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33acf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="33acf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33acf-121">Request headers</span></span>

| <span data-ttu-id="33acf-122">Имя</span><span class="sxs-lookup"><span data-stu-id="33acf-122">Name</span></span>       | <span data-ttu-id="33acf-123">Тип</span><span class="sxs-lookup"><span data-stu-id="33acf-123">Type</span></span> | <span data-ttu-id="33acf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="33acf-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33acf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="33acf-125">Authorization</span></span>  | <span data-ttu-id="33acf-126">string</span><span class="sxs-lookup"><span data-stu-id="33acf-126">string</span></span>  | <span data-ttu-id="33acf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33acf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33acf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="33acf-129">Request body</span></span>

<span data-ttu-id="33acf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33acf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33acf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="33acf-131">Response</span></span>

<span data-ttu-id="33acf-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="33acf-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="33acf-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="33acf-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="33acf-135">Пример 1. Удаление члена роли каталога с помощью объекта role objectId</span><span class="sxs-lookup"><span data-stu-id="33acf-135">Example 1: Remove directory role member using role objectId</span></span>

##### <a name="request"></a><span data-ttu-id="33acf-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="33acf-136">Request</span></span>

<span data-ttu-id="33acf-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33acf-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33acf-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="33acf-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_objectId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{role-objectId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="33acf-139">C#</span><span class="sxs-lookup"><span data-stu-id="33acf-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33acf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33acf-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33acf-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33acf-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33acf-142">Java</span><span class="sxs-lookup"><span data-stu-id="33acf-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33acf-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="33acf-143">Response</span></span>

<span data-ttu-id="33acf-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33acf-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-role-templateid"></a><span data-ttu-id="33acf-145">Пример 2. Удаление члена роли каталога с помощью шаблона roleId</span><span class="sxs-lookup"><span data-stu-id="33acf-145">Example 2: Remove directory role member using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="33acf-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="33acf-146">Request</span></span>

<span data-ttu-id="33acf-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="33acf-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="33acf-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="33acf-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId={role-templateId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="33acf-149">C#</span><span class="sxs-lookup"><span data-stu-id="33acf-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33acf-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33acf-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33acf-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33acf-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33acf-152">Java</span><span class="sxs-lookup"><span data-stu-id="33acf-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33acf-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="33acf-153">Response</span></span>

<span data-ttu-id="33acf-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="33acf-154">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

