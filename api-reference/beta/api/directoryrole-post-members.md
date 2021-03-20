---
title: Добавление участника роли каталога
description: Создание нового участника роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 843eb3d27e8765d0d95fb8ee86c11b0f1deae5bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946614"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="81e02-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="81e02-103">Add directory role member</span></span>

<span data-ttu-id="81e02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81e02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81e02-105">Создание нового участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="81e02-105">Create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="81e02-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81e02-106">Permissions</span></span>
<span data-ttu-id="81e02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81e02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81e02-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81e02-109">Permission type</span></span>      | <span data-ttu-id="81e02-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81e02-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81e02-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81e02-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81e02-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81e02-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81e02-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81e02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81e02-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81e02-114">Not supported.</span></span>    |
|<span data-ttu-id="81e02-115">Application</span><span class="sxs-lookup"><span data-stu-id="81e02-115">Application</span></span> | <span data-ttu-id="81e02-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="81e02-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="81e02-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81e02-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="81e02-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81e02-118">Request headers</span></span>
| <span data-ttu-id="81e02-119">Имя</span><span class="sxs-lookup"><span data-stu-id="81e02-119">Name</span></span>       | <span data-ttu-id="81e02-120">Тип</span><span class="sxs-lookup"><span data-stu-id="81e02-120">Type</span></span> | <span data-ttu-id="81e02-121">Описание</span><span class="sxs-lookup"><span data-stu-id="81e02-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81e02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81e02-122">Authorization</span></span>  | <span data-ttu-id="81e02-123">string</span><span class="sxs-lookup"><span data-stu-id="81e02-123">string</span></span>  | <span data-ttu-id="81e02-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81e02-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81e02-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81e02-126">Content-type</span></span> | <span data-ttu-id="81e02-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81e02-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81e02-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81e02-129">Request body</span></span>
<span data-ttu-id="81e02-130">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="81e02-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="81e02-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="81e02-131">Response</span></span>

<span data-ttu-id="81e02-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81e02-132">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81e02-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="81e02-133">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="81e02-134">Пример 1. Назначение встроенной роли пользователю</span><span class="sxs-lookup"><span data-stu-id="81e02-134">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="81e02-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="81e02-135">Request</span></span>
<span data-ttu-id="81e02-136">В следующем примере пользователю назначается встроенная роль.</span><span class="sxs-lookup"><span data-stu-id="81e02-136">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="81e02-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="81e02-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_1"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
}
```
# <a name="javascript"></a>[<span data-ttu-id="81e02-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81e02-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="81e02-139">C#</span><span class="sxs-lookup"><span data-stu-id="81e02-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81e02-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81e02-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81e02-141">Java</span><span class="sxs-lookup"><span data-stu-id="81e02-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="81e02-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="81e02-142">Response</span></span>
<span data-ttu-id="81e02-143">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81e02-143">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="81e02-144">Пример 2. Назначение встроенной роли группе</span><span class="sxs-lookup"><span data-stu-id="81e02-144">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="81e02-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="81e02-145">Request</span></span>
<span data-ttu-id="81e02-146">Вы можете использовать определенный набор ресурсов, например пользователей или групп в теле запроса, или общие **каталогиОбъектов.**</span><span class="sxs-lookup"><span data-stu-id="81e02-146">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="81e02-147">В этом примере показано, как можно использовать **directoryObjects.**</span><span class="sxs-lookup"><span data-stu-id="81e02-147">This example shows how you can use **directoryObjects**.</span></span>


# <a name="http"></a>[<span data-ttu-id="81e02-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="81e02-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_2"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
}
```
# <a name="c"></a>[<span data-ttu-id="81e02-149">C#</span><span class="sxs-lookup"><span data-stu-id="81e02-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81e02-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81e02-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81e02-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81e02-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81e02-152">Java</span><span class="sxs-lookup"><span data-stu-id="81e02-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81e02-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="81e02-153">Response</span></span>
<span data-ttu-id="81e02-154">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81e02-154">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


