---
title: Создание unifiedRoleDefinition
description: Создайте новый объект unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 92d02320b102cedf1cef95f6966d97d78ad341d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051006"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="57900-103">Создание unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="57900-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="57900-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57900-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57900-105">Создайте новый [объект unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="57900-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57900-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57900-106">Permissions</span></span>

<span data-ttu-id="57900-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57900-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57900-109">Permission type</span></span>                        | <span data-ttu-id="57900-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57900-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57900-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57900-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57900-112">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="57900-112">RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="57900-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57900-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57900-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57900-114">Not supported.</span></span> |
| <span data-ttu-id="57900-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="57900-115">Application</span></span>                            | <span data-ttu-id="57900-116">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="57900-116">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="57900-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57900-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="57900-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57900-118">Request headers</span></span>

| <span data-ttu-id="57900-119">Имя</span><span class="sxs-lookup"><span data-stu-id="57900-119">Name</span></span>          | <span data-ttu-id="57900-120">Описание</span><span class="sxs-lookup"><span data-stu-id="57900-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="57900-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57900-121">Authorization</span></span> | <span data-ttu-id="57900-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="57900-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="57900-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57900-123">Request body</span></span>

<span data-ttu-id="57900-124">В теле запроса поставляем представление JSON объекта [unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="57900-124">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="57900-125">В следующей таблице показаны свойства, необходимые при создании roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="57900-125">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="57900-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="57900-126">Parameter</span></span> | <span data-ttu-id="57900-127">Тип</span><span class="sxs-lookup"><span data-stu-id="57900-127">Type</span></span> | <span data-ttu-id="57900-128">Описание</span><span class="sxs-lookup"><span data-stu-id="57900-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57900-129">displayName</span><span class="sxs-lookup"><span data-stu-id="57900-129">displayName</span></span> |<span data-ttu-id="57900-130">string</span><span class="sxs-lookup"><span data-stu-id="57900-130">string</span></span> |<span data-ttu-id="57900-131">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="57900-131">The display name for the role definition.</span></span>|
|<span data-ttu-id="57900-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="57900-132">isEnabled</span></span> |<span data-ttu-id="57900-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="57900-133">Boolean</span></span> |<span data-ttu-id="57900-134">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="57900-134">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="57900-135">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="57900-135">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="57900-136">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="57900-136">rolePermissions</span></span> |<span data-ttu-id="57900-137">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="57900-137">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="57900-138">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="57900-138">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="57900-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="57900-139">Response</span></span>

<span data-ttu-id="57900-140">В случае успеха этот метод возвращает код отклика и новый `201 Created` [объект unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="57900-140">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57900-141">Пример</span><span class="sxs-lookup"><span data-stu-id="57900-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="57900-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="57900-142">Request</span></span>

<span data-ttu-id="57900-143">Ниже приводится пример создания настраиваемой роли.</span><span class="sxs-lookup"><span data-stu-id="57900-143">The following is an example of creating a custom role.</span></span>


# <a name="http"></a>[<span data-ttu-id="57900-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="57900-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroledefinition_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
Content-type: application/json

{
  "description": "Update basic properties of application registrations",
  "displayName": "Application Registration Support Administrator",
  "rolePermissions":
    [
        {
            "allowedResourceActions": 
            [
                "microsoft.directory/applications/basic/read"
            ]
        }
    ],
    "isEnabled" : "true"
}
```
# <a name="c"></a>[<span data-ttu-id="57900-145">C#</span><span class="sxs-lookup"><span data-stu-id="57900-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57900-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57900-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57900-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57900-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57900-148">Java</span><span class="sxs-lookup"><span data-stu-id="57900-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57900-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="57900-149">Response</span></span>

<span data-ttu-id="57900-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="57900-150">The following is an example of the response.</span></span>
> <span data-ttu-id="57900-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57900-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "d5eec5e0-6992-4c6b-b430-0f833f1a815a",
    "description": "Update basic properties of application registrations",
    "displayName": "Application Registration Support Administrator",
    "isBuiltIn": false,
    "isEnabled": true,
    "templateId": "c2cb59a3-2d01-4176-a458-95b0e674966f",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/standard/read",
                "microsoft.directory/applications/basic/update"
            ],
            "condition": null
        }
    ],
    "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('c2cb59a3-2d01-4176-a458-95b0e674966f')/inheritsPermissionsFrom",
    "inheritsPermissionsFrom": []
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


