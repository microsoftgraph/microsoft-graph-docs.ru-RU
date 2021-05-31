---
title: Создание unifiedRoleDefinition
description: Создайте новый объект unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: e5512205b346d1005b8ce51f3ab11afa4f95a9a2
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709509"
---
# <a name="create-unifiedroledefinition"></a><span data-ttu-id="14350-103">Создание unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="14350-103">Create unifiedRoleDefinition</span></span>

<span data-ttu-id="14350-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14350-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14350-105">Создание нового [единого объектаRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="14350-105">Create a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="14350-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="14350-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="14350-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="14350-107">device management (Intune)</span></span>
- <span data-ttu-id="14350-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="14350-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="14350-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="14350-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="14350-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14350-110">Permissions</span></span>

<span data-ttu-id="14350-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="14350-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="14350-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14350-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="14350-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="14350-113">Supported provider</span></span>      | <span data-ttu-id="14350-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14350-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="14350-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14350-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14350-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14350-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="14350-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="14350-117">Device management</span></span> | <span data-ttu-id="14350-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14350-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="14350-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14350-119">Not supported.</span></span> | <span data-ttu-id="14350-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14350-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="14350-121">Каталог</span><span class="sxs-lookup"><span data-stu-id="14350-121">Directory</span></span> | <span data-ttu-id="14350-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="14350-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="14350-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14350-123">Not supported.</span></span>| <span data-ttu-id="14350-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14350-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14350-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14350-125">HTTP request</span></span>

<span data-ttu-id="14350-126">Чтобы создать определение роли для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="14350-126">To create a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/deviceManagement/roleDefinitions
```

<span data-ttu-id="14350-127">Чтобы создать определение роли для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="14350-127">To create a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /roleManagement/directory/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="14350-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14350-128">Request headers</span></span>

| <span data-ttu-id="14350-129">Имя</span><span class="sxs-lookup"><span data-stu-id="14350-129">Name</span></span>          | <span data-ttu-id="14350-130">Описание</span><span class="sxs-lookup"><span data-stu-id="14350-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="14350-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14350-131">Authorization</span></span> | <span data-ttu-id="14350-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="14350-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="14350-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14350-133">Request body</span></span>

<span data-ttu-id="14350-134">В теле запроса поставляем представление JSON объекта [unifiedRoleDefinition.](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="14350-134">In the request body, supply a JSON representation of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.</span></span>

<span data-ttu-id="14350-135">В следующей таблице показаны свойства, необходимые при создании roleDefinition.</span><span class="sxs-lookup"><span data-stu-id="14350-135">The following table shows the properties that are required when you create a roleDefinition.</span></span>

| <span data-ttu-id="14350-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="14350-136">Parameter</span></span> | <span data-ttu-id="14350-137">Тип</span><span class="sxs-lookup"><span data-stu-id="14350-137">Type</span></span> | <span data-ttu-id="14350-138">Описание</span><span class="sxs-lookup"><span data-stu-id="14350-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14350-139">displayName</span><span class="sxs-lookup"><span data-stu-id="14350-139">displayName</span></span> |<span data-ttu-id="14350-140">string</span><span class="sxs-lookup"><span data-stu-id="14350-140">string</span></span> |<span data-ttu-id="14350-141">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="14350-141">The display name for the role definition.</span></span>|
|<span data-ttu-id="14350-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="14350-142">isEnabled</span></span> |<span data-ttu-id="14350-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="14350-143">Boolean</span></span> |<span data-ttu-id="14350-144">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="14350-144">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="14350-145">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="14350-145">If false the role is not available for assignment.</span></span>|
|<span data-ttu-id="14350-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="14350-146">rolePermissions</span></span> |<span data-ttu-id="14350-147">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="14350-147">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span> |<span data-ttu-id="14350-148">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="14350-148">List of permissions included in the role.</span></span>|

## <a name="response"></a><span data-ttu-id="14350-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="14350-149">Response</span></span>

<span data-ttu-id="14350-150">В случае успеха этот метод возвращает код отклика и новый `201 Created` [объект unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="14350-150">If successful, this method returns `201 Created` response code and a new [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14350-151">Пример</span><span class="sxs-lookup"><span data-stu-id="14350-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="14350-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="14350-152">Request</span></span>

<span data-ttu-id="14350-153">Ниже приводится пример создания настраиваемой роли поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="14350-153">The following is an example of creating a custom role for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="14350-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="14350-154">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="14350-155">C#</span><span class="sxs-lookup"><span data-stu-id="14350-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroledefinition-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14350-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14350-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroledefinition-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14350-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14350-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroledefinition-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14350-158">Java</span><span class="sxs-lookup"><span data-stu-id="14350-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-unifiedroledefinition-from-rbacapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14350-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="14350-159">Response</span></span>

<span data-ttu-id="14350-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="14350-160">The following is an example of the response.</span></span>
> <span data-ttu-id="14350-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="14350-161">**Note:** The response object shown here might be shortened for readability.</span></span>

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


