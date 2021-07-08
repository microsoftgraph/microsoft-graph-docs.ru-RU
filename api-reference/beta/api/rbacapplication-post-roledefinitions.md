---
title: Создание unifiedRoleDefinition
description: Создайте новый объект unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8b5fb362456b306b8f7887ad84fe80677e3262b1
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334614"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="60ad6-103">Создание unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="60ad6-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="60ad6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60ad6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60ad6-105">Создание нового [единого объектаRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="60ad6-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="60ad6-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="60ad6-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="60ad6-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="60ad6-107">device management (Intune)</span></span>
- <span data-ttu-id="60ad6-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="60ad6-108">directory (Azure AD)</span></span>

> [!NOTE]
> <span data-ttu-id="60ad6-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="60ad6-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="60ad6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60ad6-110">Permissions</span></span>

<span data-ttu-id="60ad6-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="60ad6-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="60ad6-112">Дополнительные новости, в том числе осторожность [перед](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) выбором более привилегированных разрешений, см. [в см. в руб. Permissions.](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="60ad6-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="60ad6-113">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="60ad6-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="60ad6-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60ad6-114">Permission type</span></span>      | <span data-ttu-id="60ad6-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60ad6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60ad6-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60ad6-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="60ad6-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ad6-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="60ad6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60ad6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ad6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60ad6-119">Not supported.</span></span>    |
|<span data-ttu-id="60ad6-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="60ad6-120">Application</span></span> | <span data-ttu-id="60ad6-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ad6-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="60ad6-122">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="60ad6-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="60ad6-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60ad6-123">Permission type</span></span>      | <span data-ttu-id="60ad6-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60ad6-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60ad6-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60ad6-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="60ad6-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60ad6-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="60ad6-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60ad6-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60ad6-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60ad6-128">Not supported.</span></span>    |
|<span data-ttu-id="60ad6-129">Приложение</span><span class="sxs-lookup"><span data-stu-id="60ad6-129">Application</span></span> | <span data-ttu-id="60ad6-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ad6-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60ad6-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60ad6-131">HTTP request</span></span>

<span data-ttu-id="60ad6-132">Чтобы создать определение роли для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="60ad6-132">To create a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="60ad6-133">Чтобы создать определение роли для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="60ad6-133">To create a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="60ad6-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60ad6-134">Request headers</span></span>

| <span data-ttu-id="60ad6-135">Имя</span><span class="sxs-lookup"><span data-stu-id="60ad6-135">Name</span></span>          | <span data-ttu-id="60ad6-136">Описание</span><span class="sxs-lookup"><span data-stu-id="60ad6-136">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60ad6-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="60ad6-137">Authorization</span></span> | <span data-ttu-id="60ad6-138">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="60ad6-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="60ad6-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="60ad6-139">Request body</span></span>

<span data-ttu-id="60ad6-140">В теле запроса поставляем представление JSON объекта [unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="60ad6-140">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="60ad6-141">В следующей таблице показаны свойства, необходимые при создании roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="60ad6-141">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="60ad6-142">Параметр</span><span class="sxs-lookup"><span data-stu-id="60ad6-142">Parameter</span></span> | <span data-ttu-id="60ad6-143">Тип</span><span class="sxs-lookup"><span data-stu-id="60ad6-143">Type</span></span> | <span data-ttu-id="60ad6-144">Описание</span><span class="sxs-lookup"><span data-stu-id="60ad6-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60ad6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="60ad6-145">displayName</span></span> |<span data-ttu-id="60ad6-146">string</span><span class="sxs-lookup"><span data-stu-id="60ad6-146">string</span></span> |<span data-ttu-id="60ad6-147">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="60ad6-147">The display name for the role definition.</span></span>|
|<span data-ttu-id="60ad6-148">isEnabled</span><span class="sxs-lookup"><span data-stu-id="60ad6-148">isEnabled</span></span> |<span data-ttu-id="60ad6-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="60ad6-149">Boolean</span></span> |<span data-ttu-id="60ad6-150">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="60ad6-150">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="60ad6-151">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="60ad6-151">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="60ad6-152">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="60ad6-152">rolePermissions</span></span> |<span data-ttu-id="60ad6-153">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="60ad6-153">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="60ad6-154">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="60ad6-154">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="60ad6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="60ad6-155">Response</span></span>

<span data-ttu-id="60ad6-156">В случае успеха этот метод возвращает код отклика и новый `201 Created` [объект unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="60ad6-156">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60ad6-157">Пример</span><span class="sxs-lookup"><span data-stu-id="60ad6-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="60ad6-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="60ad6-158">Request</span></span>

<span data-ttu-id="60ad6-159">Ниже приводится пример создания настраиваемой роли поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="60ad6-159">The following is an example of creating a custom role for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="60ad6-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="60ad6-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="60ad6-161">C#</span><span class="sxs-lookup"><span data-stu-id="60ad6-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60ad6-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60ad6-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60ad6-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60ad6-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60ad6-164">Java</span><span class="sxs-lookup"><span data-stu-id="60ad6-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60ad6-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="60ad6-165">Response</span></span>

<span data-ttu-id="60ad6-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="60ad6-166">The following is an example of the response.</span></span>
> <span data-ttu-id="60ad6-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="60ad6-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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


