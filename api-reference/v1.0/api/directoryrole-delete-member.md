---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2c6c8dba462c4514907c4d167810abe1ccfe3cd7
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377073"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="64ed9-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="64ed9-103">Remove directory role member</span></span>

<span data-ttu-id="64ed9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64ed9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64ed9-105">Удаление члена из [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="64ed9-105">Remove a member from a [directoryRole](../resources/directoryrole.md).</span></span>

> [!Note]
> <span data-ttu-id="64ed9-106">С этим API можно использовать как идентификатор объекта, так и идентификатор шаблона **directoryRole** .</span><span class="sxs-lookup"><span data-stu-id="64ed9-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="64ed9-107">Неизменяемый идентификатор шаблона встроенной роли, который можно просмотреть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="64ed9-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="64ed9-108">Дополнительные сведения: [идентификаторы шаблонов ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="64ed9-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="64ed9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64ed9-109">Permissions</span></span>

<span data-ttu-id="64ed9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64ed9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64ed9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64ed9-112">Permission type</span></span>      | <span data-ttu-id="64ed9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64ed9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64ed9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64ed9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="64ed9-115">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="64ed9-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64ed9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64ed9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64ed9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64ed9-117">Not supported.</span></span>    |
|<span data-ttu-id="64ed9-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="64ed9-118">Application</span></span> | <span data-ttu-id="64ed9-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="64ed9-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="64ed9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64ed9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="64ed9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64ed9-121">Request headers</span></span>

| <span data-ttu-id="64ed9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="64ed9-122">Name</span></span>       | <span data-ttu-id="64ed9-123">Тип</span><span class="sxs-lookup"><span data-stu-id="64ed9-123">Type</span></span> | <span data-ttu-id="64ed9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="64ed9-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64ed9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="64ed9-125">Authorization</span></span>  | <span data-ttu-id="64ed9-126">string</span><span class="sxs-lookup"><span data-stu-id="64ed9-126">string</span></span>  | <span data-ttu-id="64ed9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64ed9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64ed9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64ed9-129">Request body</span></span>

<span data-ttu-id="64ed9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64ed9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64ed9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="64ed9-131">Response</span></span>

<span data-ttu-id="64ed9-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="64ed9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64ed9-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="64ed9-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="64ed9-135">Пример 1: Удаление члена роли каталога с помощью ИД роли</span><span class="sxs-lookup"><span data-stu-id="64ed9-135">Example 1: Remove directory role member using role objectId</span></span>

##### <a name="request"></a><span data-ttu-id="64ed9-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="64ed9-136">Request</span></span>

<span data-ttu-id="64ed9-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64ed9-137">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64ed9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="64ed9-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_objectId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{role-objectId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="64ed9-139">C#</span><span class="sxs-lookup"><span data-stu-id="64ed9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64ed9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64ed9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64ed9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64ed9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64ed9-142">Java</span><span class="sxs-lookup"><span data-stu-id="64ed9-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64ed9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="64ed9-143">Response</span></span>

<span data-ttu-id="64ed9-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64ed9-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-role-templateid"></a><span data-ttu-id="64ed9-145">Пример 2: Удаление члена роли каталога с помощью templateId ролей</span><span class="sxs-lookup"><span data-stu-id="64ed9-145">Example 2: Remove directory role member using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="64ed9-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="64ed9-146">Request</span></span>

<span data-ttu-id="64ed9-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64ed9-147">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64ed9-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="64ed9-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId={role-templateId}/members/{user-id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="64ed9-149">C#</span><span class="sxs-lookup"><span data-stu-id="64ed9-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64ed9-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64ed9-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64ed9-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64ed9-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64ed9-152">Java</span><span class="sxs-lookup"><span data-stu-id="64ed9-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64ed9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="64ed9-153">Response</span></span>

<span data-ttu-id="64ed9-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64ed9-154">Here is an example of the response.</span></span> 
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

