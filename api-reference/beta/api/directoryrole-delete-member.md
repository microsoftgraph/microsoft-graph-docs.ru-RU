---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: aec2f698c947a74f2814c4e91f350b612fa0600c
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118597"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="05abc-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="05abc-103">Remove directory role member</span></span>

<span data-ttu-id="05abc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05abc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05abc-105">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="05abc-105">Remove a member from a directoryRole.</span></span>

<span data-ttu-id="05abc-106">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="05abc-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="05abc-107">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="05abc-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="05abc-108">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="05abc-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="05abc-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05abc-109">Permissions</span></span>

<span data-ttu-id="05abc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05abc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05abc-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05abc-112">Permission type</span></span>      | <span data-ttu-id="05abc-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05abc-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05abc-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05abc-114">Delegated (work or school account)</span></span> | <span data-ttu-id="05abc-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05abc-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05abc-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05abc-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05abc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05abc-117">Not supported.</span></span>    |
|<span data-ttu-id="05abc-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05abc-118">Application</span></span> | <span data-ttu-id="05abc-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="05abc-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="05abc-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05abc-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{role-id}/members/{id}/$ref
DELETE /directoryRoles/roleTemplateId={roleTemplateId}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="05abc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05abc-121">Request headers</span></span>

| <span data-ttu-id="05abc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="05abc-122">Name</span></span>       | <span data-ttu-id="05abc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="05abc-123">Type</span></span> | <span data-ttu-id="05abc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="05abc-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05abc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="05abc-125">Authorization</span></span>  | <span data-ttu-id="05abc-126">string</span><span class="sxs-lookup"><span data-stu-id="05abc-126">string</span></span>  | <span data-ttu-id="05abc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05abc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="05abc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05abc-129">Request body</span></span>

<span data-ttu-id="05abc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05abc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05abc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="05abc-131">Response</span></span>

<span data-ttu-id="05abc-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05abc-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05abc-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="05abc-134">Examples</span></span>

### <a name="example-1-remove-directory-role-member-using-role-objectid"></a><span data-ttu-id="05abc-135">Пример 1. Удаление члена роли каталога с помощью объекта role objectId</span><span class="sxs-lookup"><span data-stu-id="05abc-135">Example 1: Remove directory role member using role objectId</span></span>

#### <a name="request"></a><span data-ttu-id="05abc-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="05abc-136">Request</span></span>

<span data-ttu-id="05abc-137">В этом примере замените значение id роли каталога и id-значение объекта пользователя или каталога, которое требуется отменить из роли `f8e85ed8-f66f-4058-b170-3efae8b9c6e5`  `bb165b45-151c-4cf6-9911-cd7188912848` каталога. </span><span class="sxs-lookup"><span data-stu-id="05abc-137">In this example, replace `f8e85ed8-f66f-4058-b170-3efae8b9c6e5` with the **id** value of the directory role and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of the user or directory object that you wish to unassign from the directory role.</span></span>

# <a name="http"></a>[<span data-ttu-id="05abc-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="05abc-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryRoles/f8e85ed8-f66f-4058-b170-3efae8b9c6e5/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="05abc-139">C#</span><span class="sxs-lookup"><span data-stu-id="05abc-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05abc-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05abc-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05abc-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05abc-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05abc-142">Java</span><span class="sxs-lookup"><span data-stu-id="05abc-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="05abc-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="05abc-143">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-directory-role-member-using-roletemplateid"></a><span data-ttu-id="05abc-144">Пример 2. Удаление члена роли каталога с помощью roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="05abc-144">Example 2: Remove directory role member using roleTemplateId</span></span>

#### <a name="request"></a><span data-ttu-id="05abc-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="05abc-145">Request</span></span>

<span data-ttu-id="05abc-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05abc-146">The following is an example of the request.</span></span> <span data-ttu-id="05abc-147">Замените `9f06204d-73c1-4d4c-880a-6edb90606fd8` значение roleTemplateId и `bb165b45-151c-4cf6-9911-cd7188912848` **id-значением** пользователя объекта каталога.</span><span class="sxs-lookup"><span data-stu-id="05abc-147">Replace `9f06204d-73c1-4d4c-880a-6edb90606fd8` with the value of your roleTemplateId and `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user of directory object.</span></span>


# <a name="http"></a>[<span data-ttu-id="05abc-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="05abc-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole_templateId"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=9f06204d-73c1-4d4c-880a-6edb90606fd8/members/bb165b45-151c-4cf6-9911-cd7188912848/$ref
```
# <a name="c"></a>[<span data-ttu-id="05abc-149">C#</span><span class="sxs-lookup"><span data-stu-id="05abc-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05abc-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05abc-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05abc-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05abc-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05abc-152">Java</span><span class="sxs-lookup"><span data-stu-id="05abc-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="05abc-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="05abc-153">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


