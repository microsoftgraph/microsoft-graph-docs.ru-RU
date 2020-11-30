---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e14e80c6330b864d4d90496eb24094bac6a27d5
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377084"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="72350-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="72350-103">Add directory role member</span></span>

<span data-ttu-id="72350-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72350-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72350-105">С помощью этого API можно создать участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="72350-105">Use this API to create a new directory role member.</span></span>

> [!Note]
> <span data-ttu-id="72350-106">С этим API можно использовать как идентификатор объекта, так и идентификатор шаблона **directoryRole** .</span><span class="sxs-lookup"><span data-stu-id="72350-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="72350-107">Неизменяемый идентификатор шаблона встроенной роли, который можно просмотреть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="72350-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="72350-108">Дополнительные сведения: [идентификаторы шаблонов ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="72350-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="72350-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72350-109">Permissions</span></span>
<span data-ttu-id="72350-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72350-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72350-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72350-112">Permission type</span></span>      | <span data-ttu-id="72350-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72350-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72350-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72350-114">Delegated (work or school account)</span></span> | <span data-ttu-id="72350-115">Ролеманажемент. ReadWrite. Directory, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="72350-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="72350-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72350-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72350-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72350-117">Not supported.</span></span>    |
|<span data-ttu-id="72350-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="72350-118">Application</span></span> | <span data-ttu-id="72350-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="72350-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="72350-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72350-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="72350-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72350-121">Request headers</span></span>
| <span data-ttu-id="72350-122">Имя</span><span class="sxs-lookup"><span data-stu-id="72350-122">Name</span></span>       | <span data-ttu-id="72350-123">Тип</span><span class="sxs-lookup"><span data-stu-id="72350-123">Type</span></span> | <span data-ttu-id="72350-124">Описание</span><span class="sxs-lookup"><span data-stu-id="72350-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="72350-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="72350-125">Authorization</span></span>  | <span data-ttu-id="72350-126">string</span><span class="sxs-lookup"><span data-stu-id="72350-126">string</span></span>  | <span data-ttu-id="72350-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72350-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="72350-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72350-129">Content-Type</span></span>  | <span data-ttu-id="72350-130">string</span><span class="sxs-lookup"><span data-stu-id="72350-130">string</span></span>  | <span data-ttu-id="72350-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72350-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72350-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72350-133">Request body</span></span>
<span data-ttu-id="72350-134">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72350-134">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="72350-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="72350-135">Response</span></span>

<span data-ttu-id="72350-136">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="72350-136">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="72350-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="72350-137">Examples</span></span>

### <a name="example-1-add-a-new-member-to-a-directory-role-using-role-objectid"></a><span data-ttu-id="72350-138">Пример 1: Добавление нового члена к роли каталога с помощью ИД объекта Role</span><span class="sxs-lookup"><span data-stu-id="72350-138">Example 1: Add a new member to a directory role using role objectId</span></span>

##### <a name="request"></a><span data-ttu-id="72350-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="72350-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="72350-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="72350-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_objectId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{role-objectId}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{user-id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="72350-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72350-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72350-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72350-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="72350-143">C#</span><span class="sxs-lookup"><span data-stu-id="72350-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72350-144">Java</span><span class="sxs-lookup"><span data-stu-id="72350-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72350-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="72350-145">Response</span></span>
><span data-ttu-id="72350-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72350-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

### <a name="example-2-add-a-new-member-to-a-directory-role-using-role-templateid"></a><span data-ttu-id="72350-147">Пример 2: Добавление нового члена к роли каталога с помощью роли templateId</span><span class="sxs-lookup"><span data-stu-id="72350-147">Example 2: Add a new member to a directory role using role templateId</span></span>

##### <a name="request"></a><span data-ttu-id="72350-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="72350-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="72350-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="72350-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_templateId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId={role-templateId}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{user-id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="72350-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72350-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72350-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72350-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="72350-152">C#</span><span class="sxs-lookup"><span data-stu-id="72350-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72350-153">Java</span><span class="sxs-lookup"><span data-stu-id="72350-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="72350-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="72350-154">Response</span></span>
><span data-ttu-id="72350-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="72350-155">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

