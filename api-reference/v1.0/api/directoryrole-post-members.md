---
title: Добавление участника роли каталога
description: С помощью этого API можно создать участника роли каталога.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ae03863fd35d7438a5fa3b9ff2ae0bfa90e41dce
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854168"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="65f8f-103">Добавление участника роли каталога</span><span class="sxs-lookup"><span data-stu-id="65f8f-103">Add directory role member</span></span>

<span data-ttu-id="65f8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f8f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65f8f-105">Создание нового участника роли каталога.</span><span class="sxs-lookup"><span data-stu-id="65f8f-105">Create a new directory role member.</span></span>

<span data-ttu-id="65f8f-106">С помощью этого API можно использовать ИД объекта и ИД шаблона **каталогаRole.**</span><span class="sxs-lookup"><span data-stu-id="65f8f-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="65f8f-107">ID шаблона встроенной роли неменяем и его можно увидеть в описании роли на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="65f8f-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="65f8f-108">Подробные сведения см. [в материале Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="65f8f-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="65f8f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65f8f-109">Permissions</span></span>
<span data-ttu-id="65f8f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f8f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65f8f-112">Permission type</span></span>      | <span data-ttu-id="65f8f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65f8f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65f8f-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65f8f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="65f8f-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65f8f-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65f8f-116">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65f8f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65f8f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f8f-117">Not supported.</span></span>    |
|<span data-ttu-id="65f8f-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="65f8f-118">Application</span></span> | <span data-ttu-id="65f8f-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="65f8f-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="65f8f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65f8f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{role-objectId}/members/$ref
POST /directoryRoles/roleTemplateId={role-templateId}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="65f8f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65f8f-121">Request headers</span></span>
| <span data-ttu-id="65f8f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="65f8f-122">Name</span></span>       | <span data-ttu-id="65f8f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="65f8f-123">Type</span></span> | <span data-ttu-id="65f8f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="65f8f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="65f8f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="65f8f-125">Authorization</span></span>  | <span data-ttu-id="65f8f-126">string</span><span class="sxs-lookup"><span data-stu-id="65f8f-126">string</span></span>  | <span data-ttu-id="65f8f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65f8f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65f8f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65f8f-129">Content-Type</span></span>  | <span data-ttu-id="65f8f-130">string</span><span class="sxs-lookup"><span data-stu-id="65f8f-130">string</span></span>  | <span data-ttu-id="65f8f-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65f8f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65f8f-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65f8f-133">Request body</span></span>
<span data-ttu-id="65f8f-134">Предоставьте в тексте запроса описание добавляемого объекта [directoryObject](../resources/directoryobject.md) или [user](../resources/user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65f8f-134">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="65f8f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f8f-135">Response</span></span>

<span data-ttu-id="65f8f-136">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="65f8f-136">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="65f8f-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="65f8f-137">Examples</span></span>

### <a name="example-1-add-a-new-member-to-a-directory-role-using-role-objectid"></a><span data-ttu-id="65f8f-138">Пример 1. Добавление нового участника в роль каталога с помощью объекта roleId</span><span class="sxs-lookup"><span data-stu-id="65f8f-138">Example 1: Add a new member to a directory role using role objectId</span></span>

<span data-ttu-id="65f8f-139">В этом запросе замените значение id для роли каталога, которую вы хотите назначить пользователю `fe8f10bf-c9c2-47eb-95cb-c26cc85f1830` или объекту  каталога.</span><span class="sxs-lookup"><span data-stu-id="65f8f-139">In this request, replace `fe8f10bf-c9c2-47eb-95cb-c26cc85f1830` with the **id** value for the directory role you wish to assign to the user or directory object.</span></span> <span data-ttu-id="65f8f-140">`15c1a2d5-9101-44b2-83ab-885db8a647ca`Замените **значение id** объекта пользователя или каталога.</span><span class="sxs-lookup"><span data-stu-id="65f8f-140">Replace `15c1a2d5-9101-44b2-83ab-885db8a647ca` with the **id** value of your user or directory object.</span></span> 

##### <a name="request"></a><span data-ttu-id="65f8f-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="65f8f-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="65f8f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="65f8f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_objectId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/15c1a2d5-9101-44b2-83ab-885db8a647ca"
}
```
# <a name="javascript"></a>[<span data-ttu-id="65f8f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65f8f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65f8f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65f8f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="65f8f-145">C#</span><span class="sxs-lookup"><span data-stu-id="65f8f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65f8f-146">Java</span><span class="sxs-lookup"><span data-stu-id="65f8f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65f8f-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f8f-147">Response</span></span>
><span data-ttu-id="65f8f-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="65f8f-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

### <a name="example-2-add-a-new-member-to-a-directory-role-using-role-templateid"></a><span data-ttu-id="65f8f-149">Пример 2. Добавление нового участника в роль каталога с помощью шаблона ролейId</span><span class="sxs-lookup"><span data-stu-id="65f8f-149">Example 2: Add a new member to a directory role using role templateId</span></span>

<span data-ttu-id="65f8f-150">В этом запросе замените значение `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` **roleTemplateId** для роли каталога, которую вы хотите назначить объекту пользователя или каталога.</span><span class="sxs-lookup"><span data-stu-id="65f8f-150">In this request, replace `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` with the value of the **roleTemplateId** for the directory role you wish to assign to the user or directory object.</span></span> <span data-ttu-id="65f8f-151">`bb165b45-151c-4cf6-9911-cd7188912848`Замените **значение id** объекта пользователя или каталога.</span><span class="sxs-lookup"><span data-stu-id="65f8f-151">Replace `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user or directory object.</span></span> 

##### <a name="request"></a><span data-ttu-id="65f8f-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="65f8f-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="65f8f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="65f8f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_templateId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/bb165b45-151c-4cf6-9911-cd7188912848"
}
```
# <a name="javascript"></a>[<span data-ttu-id="65f8f-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65f8f-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65f8f-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65f8f-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="65f8f-156">C#</span><span class="sxs-lookup"><span data-stu-id="65f8f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65f8f-157">Java</span><span class="sxs-lookup"><span data-stu-id="65f8f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="65f8f-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f8f-158">Response</span></span>
><span data-ttu-id="65f8f-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="65f8f-159">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response"
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

