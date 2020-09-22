---
title: Добавление участника роли каталога
description: Создайте новый член роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff6569531dd264223e0352b659531a02aaab4a05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008738"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="9bee2-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="9bee2-103">Add directory role member</span></span>

<span data-ttu-id="9bee2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bee2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bee2-105">Создайте новый член роли каталога.</span><span class="sxs-lookup"><span data-stu-id="9bee2-105">Create a new directory role member.</span></span>
## <a name="permissions"></a><span data-ttu-id="9bee2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bee2-106">Permissions</span></span>
<span data-ttu-id="9bee2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bee2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bee2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bee2-109">Permission type</span></span>      | <span data-ttu-id="9bee2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bee2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bee2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bee2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9bee2-112">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="9bee2-112">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9bee2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bee2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bee2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bee2-114">Not supported.</span></span>    |
|<span data-ttu-id="9bee2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bee2-115">Application</span></span> | <span data-ttu-id="9bee2-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9bee2-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="9bee2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bee2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9bee2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bee2-118">Request headers</span></span>
| <span data-ttu-id="9bee2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9bee2-119">Name</span></span>       | <span data-ttu-id="9bee2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9bee2-120">Type</span></span> | <span data-ttu-id="9bee2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9bee2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9bee2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bee2-122">Authorization</span></span>  | <span data-ttu-id="9bee2-123">string</span><span class="sxs-lookup"><span data-stu-id="9bee2-123">string</span></span>  | <span data-ttu-id="9bee2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bee2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9bee2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bee2-126">Content-type</span></span> | <span data-ttu-id="9bee2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bee2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9bee2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bee2-129">Request body</span></span>
<span data-ttu-id="9bee2-130">В тексте запроса добавьте представление объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bee2-130">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9bee2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bee2-131">Response</span></span>

<span data-ttu-id="9bee2-132">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9bee2-132">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9bee2-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="9bee2-133">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="9bee2-134">Пример 1: назначение встроенной роли пользователю</span><span class="sxs-lookup"><span data-stu-id="9bee2-134">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="9bee2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bee2-135">Request</span></span>
<span data-ttu-id="9bee2-136">В следующем примере для пользователя назначается встроенная роль.</span><span class="sxs-lookup"><span data-stu-id="9bee2-136">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bee2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bee2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2"
}
```
# <a name="javascript"></a>[<span data-ttu-id="9bee2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bee2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9bee2-139">C#</span><span class="sxs-lookup"><span data-stu-id="9bee2-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bee2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bee2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="9bee2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bee2-141">Response</span></span>
<span data-ttu-id="9bee2-142">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bee2-142">The following example shows the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="9bee2-143">Пример 2: назначение встроенной роли группе</span><span class="sxs-lookup"><span data-stu-id="9bee2-143">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="9bee2-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bee2-144">Request</span></span>
<span data-ttu-id="9bee2-145">Вы можете использовать определенный набор ресурсов, такой как пользователи или группы, в теле запроса, или можно использовать универсальный **директорйобжектс**.</span><span class="sxs-lookup"><span data-stu-id="9bee2-145">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="9bee2-146">В этом примере показано, как можно использовать **директорйобжектс**.</span><span class="sxs-lookup"><span data-stu-id="9bee2-146">This example shows how you can use **directoryObjects**.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id":"https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
}
```

#### <a name="response"></a><span data-ttu-id="9bee2-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bee2-147">Response</span></span>
<span data-ttu-id="9bee2-148">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bee2-148">The following example shows the response.</span></span> 

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


