---
title: Добавление участника роли каталога
description: Создание нового участника роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 135640887f43952a83f93b1b4267645a228383c4
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118499"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="0792b-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="0792b-103">Add directory role member</span></span>

<span data-ttu-id="0792b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0792b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0792b-105">Создание нового участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="0792b-105">Create a new directory role member.</span></span>

<span data-ttu-id="0792b-106">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="0792b-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="0792b-107">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0792b-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="0792b-108">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="0792b-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="0792b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0792b-109">Permissions</span></span>
<span data-ttu-id="0792b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0792b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0792b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0792b-112">Permission type</span></span>      | <span data-ttu-id="0792b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0792b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0792b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0792b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0792b-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0792b-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0792b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0792b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0792b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0792b-117">Not supported.</span></span>    |
|<span data-ttu-id="0792b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0792b-118">Application</span></span> | <span data-ttu-id="0792b-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="0792b-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="0792b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0792b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{role-id}/members/$ref
POST /directoryRoles/roleTemplateId={roleTemplateId}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="0792b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0792b-121">Request headers</span></span>
| <span data-ttu-id="0792b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0792b-122">Name</span></span>       | <span data-ttu-id="0792b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0792b-123">Type</span></span> | <span data-ttu-id="0792b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0792b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0792b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0792b-125">Authorization</span></span>  | <span data-ttu-id="0792b-126">string</span><span class="sxs-lookup"><span data-stu-id="0792b-126">string</span></span>  | <span data-ttu-id="0792b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0792b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0792b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0792b-129">Content-type</span></span> | <span data-ttu-id="0792b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0792b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0792b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0792b-132">Request body</span></span>
<span data-ttu-id="0792b-133">Укажите представление JSON объекта [directoryObject](../resources/directoryobject.md) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="0792b-133">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0792b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0792b-134">Response</span></span>

<span data-ttu-id="0792b-135">В случае успеха этот метод возвращает код отклика `201 Created` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0792b-135">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0792b-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="0792b-136">Examples</span></span>

### <a name="example-1-assign-a-built-in-role-to-a-user"></a><span data-ttu-id="0792b-137">Пример 1. Назначение встроенной роли пользователю</span><span class="sxs-lookup"><span data-stu-id="0792b-137">Example 1: Assign a built-in role to a user</span></span>
#### <a name="request"></a><span data-ttu-id="0792b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="0792b-138">Request</span></span>
<span data-ttu-id="0792b-139">В следующем примере пользователю назначается встроенная роль.</span><span class="sxs-lookup"><span data-stu-id="0792b-139">The following example assigns a built-in role to a user.</span></span>

# <a name="http"></a>[<span data-ttu-id="0792b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0792b-140">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="0792b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0792b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0792b-142">C#</span><span class="sxs-lookup"><span data-stu-id="0792b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0792b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0792b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0792b-144">Java</span><span class="sxs-lookup"><span data-stu-id="0792b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="0792b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="0792b-145">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-2-assign-a-built-in-role-to-a-group"></a><span data-ttu-id="0792b-146">Пример 2. Назначение встроенной роли группе</span><span class="sxs-lookup"><span data-stu-id="0792b-146">Example 2: Assign a built-in role to a group</span></span>
#### <a name="request"></a><span data-ttu-id="0792b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0792b-147">Request</span></span>
<span data-ttu-id="0792b-148">Вы можете использовать определенный набор ресурсов, например пользователей или групп в теле запроса, или общие **каталогиОбъектов.**</span><span class="sxs-lookup"><span data-stu-id="0792b-148">You can use a specific resource set like users or groups in the request body, or you can use generic **directoryObjects**.</span></span> <span data-ttu-id="0792b-149">В этом примере показано, как можно использовать **directoryObjects.**</span><span class="sxs-lookup"><span data-stu-id="0792b-149">This example shows how you can use **directoryObjects**.</span></span>


# <a name="http"></a>[<span data-ttu-id="0792b-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="0792b-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0792b-151">C#</span><span class="sxs-lookup"><span data-stu-id="0792b-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0792b-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0792b-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0792b-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0792b-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0792b-154">Java</span><span class="sxs-lookup"><span data-stu-id="0792b-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0792b-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="0792b-155">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No content
```

### <a name="example-3-add-a-new-member-to-a-directory-role-using-roletemplateid"></a><span data-ttu-id="0792b-156">Пример 3. Добавление нового участника в роль каталога с помощью roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="0792b-156">Example 3: Add a new member to a directory role using roleTemplateId</span></span>
#### <a name="request"></a><span data-ttu-id="0792b-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="0792b-157">Request</span></span>
<span data-ttu-id="0792b-158">В этом запросе замените значение `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` **roleTemplateId** для роли каталога, которую вы хотите назначить объекту пользователя или каталога.</span><span class="sxs-lookup"><span data-stu-id="0792b-158">In this request, replace `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` with the value of the **roleTemplateId** for the directory role you wish to assign to the user or directory object.</span></span> <span data-ttu-id="0792b-159">`bb165b45-151c-4cf6-9911-cd7188912848`Замените **значение id** объекта пользователя или каталога.</span><span class="sxs-lookup"><span data-stu-id="0792b-159">Replace `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user or directory object.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0792b-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="0792b-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_2_templateId"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b/members/$ref
Content-type: application/json
Content-length: 30

{
    "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/bb165b45-151c-4cf6-9911-cd7188912848"
}
```
# <a name="c"></a>[<span data-ttu-id="0792b-161">C#</span><span class="sxs-lookup"><span data-stu-id="0792b-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-2-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0792b-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0792b-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-2-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0792b-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0792b-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-2-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0792b-164">Java</span><span class="sxs-lookup"><span data-stu-id="0792b-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-2-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0792b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="0792b-165">Response</span></span>

<!-- {
  "blockType": "response"
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


