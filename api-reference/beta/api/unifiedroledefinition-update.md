---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4102ece8a559161e5813e175d81a62a4c7ce9843
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787417"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="67282-103">Обновление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="67282-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="67282-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67282-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67282-105">Обновление свойств объекта [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="67282-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="67282-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="67282-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="67282-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="67282-107">device management (Intune)</span></span>
- <span data-ttu-id="67282-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="67282-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="67282-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="67282-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="67282-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67282-110">Permissions</span></span>

<span data-ttu-id="67282-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="67282-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="67282-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67282-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="67282-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="67282-113">Supported provider</span></span>      | <span data-ttu-id="67282-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67282-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="67282-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67282-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67282-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="67282-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="67282-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="67282-117">Device management</span></span> | <span data-ttu-id="67282-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67282-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="67282-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67282-119">Not supported.</span></span> | <span data-ttu-id="67282-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67282-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="67282-121">Каталог</span><span class="sxs-lookup"><span data-stu-id="67282-121">Directory</span></span> | <span data-ttu-id="67282-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="67282-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="67282-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67282-123">Not supported.</span></span>| <span data-ttu-id="67282-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67282-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67282-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67282-125">HTTP request</span></span>

<span data-ttu-id="67282-126">Обновление определения ролей для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="67282-126">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="67282-127">Обновление определения ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="67282-127">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="67282-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67282-128">Request headers</span></span>

| <span data-ttu-id="67282-129">Имя</span><span class="sxs-lookup"><span data-stu-id="67282-129">Name</span></span>       | <span data-ttu-id="67282-130">Описание</span><span class="sxs-lookup"><span data-stu-id="67282-130">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="67282-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67282-131">Authorization</span></span> | <span data-ttu-id="67282-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="67282-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="67282-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67282-133">Request body</span></span>

<span data-ttu-id="67282-134">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="67282-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="67282-135">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="67282-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="67282-136">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="67282-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="67282-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="67282-137">Property</span></span>     | <span data-ttu-id="67282-138">Тип</span><span class="sxs-lookup"><span data-stu-id="67282-138">Type</span></span>        | <span data-ttu-id="67282-139">Описание</span><span class="sxs-lookup"><span data-stu-id="67282-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="67282-140">description</span><span class="sxs-lookup"><span data-stu-id="67282-140">description</span></span>|<span data-ttu-id="67282-141">String</span><span class="sxs-lookup"><span data-stu-id="67282-141">String</span></span>| <span data-ttu-id="67282-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="67282-142">The description for the role definition.</span></span> <span data-ttu-id="67282-143">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="67282-143">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="67282-144">displayName</span><span class="sxs-lookup"><span data-stu-id="67282-144">displayName</span></span>|<span data-ttu-id="67282-145">String</span><span class="sxs-lookup"><span data-stu-id="67282-145">String</span></span>| <span data-ttu-id="67282-146">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="67282-146">The display name for the role definition.</span></span> <span data-ttu-id="67282-147">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="67282-147">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="67282-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67282-148">Required.</span></span>|
|<span data-ttu-id="67282-149">id</span><span class="sxs-lookup"><span data-stu-id="67282-149">id</span></span>|<span data-ttu-id="67282-150">String</span><span class="sxs-lookup"><span data-stu-id="67282-150">String</span></span>| <span data-ttu-id="67282-151">Уникальный идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="67282-151">The unique identifier for the role definition.</span></span> <span data-ttu-id="67282-152">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="67282-152">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="67282-153">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="67282-153">isBuiltIn</span></span>|<span data-ttu-id="67282-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="67282-154">Boolean</span></span>| <span data-ttu-id="67282-155">Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в продукт или настраиваемый.</span><span class="sxs-lookup"><span data-stu-id="67282-155">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="67282-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67282-156">Read-only.</span></span> |
|<span data-ttu-id="67282-157">isEnabled</span><span class="sxs-lookup"><span data-stu-id="67282-157">isEnabled</span></span>|<span data-ttu-id="67282-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="67282-158">Boolean</span></span>| <span data-ttu-id="67282-159">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="67282-159">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="67282-160">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="67282-160">If false the role is not available for assignment.</span></span> <span data-ttu-id="67282-161">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="67282-161">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="67282-162">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="67282-162">resourceScopes</span></span>|<span data-ttu-id="67282-163">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="67282-163">String collection</span></span>| <span data-ttu-id="67282-164">К списку областей применяются разрешения, предоставленные определением ролей.</span><span class="sxs-lookup"><span data-stu-id="67282-164">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="67282-165">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="67282-165">Currently only "/" is supported.</span></span> <span data-ttu-id="67282-166">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="67282-166">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="67282-167">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**</span><span class="sxs-lookup"><span data-stu-id="67282-167">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="67282-168">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="67282-168">rolePermissions</span></span>|<span data-ttu-id="67282-169">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="67282-169">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="67282-170">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="67282-170">List of permissions included in the role.</span></span> <span data-ttu-id="67282-171">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="67282-171">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="67282-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67282-172">Required.</span></span> |
|<span data-ttu-id="67282-173">templateId</span><span class="sxs-lookup"><span data-stu-id="67282-173">templateId</span></span>|<span data-ttu-id="67282-174">String</span><span class="sxs-lookup"><span data-stu-id="67282-174">String</span></span>| <span data-ttu-id="67282-175">Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным.</span><span class="sxs-lookup"><span data-stu-id="67282-175">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="67282-176">Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах.</span><span class="sxs-lookup"><span data-stu-id="67282-176">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="67282-177">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="67282-177">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="67282-178">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="67282-178">inheritsPermissionsFrom</span></span>| <span data-ttu-id="67282-179">[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="67282-179">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="67282-180">Только для чтения набор определений ролей, которые наследует заданное определение роли.</span><span class="sxs-lookup"><span data-stu-id="67282-180">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="67282-181">Только встроенные роли Azure AD поддерживают этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="67282-181">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="67282-182">version</span><span class="sxs-lookup"><span data-stu-id="67282-182">version</span></span>|<span data-ttu-id="67282-183">String</span><span class="sxs-lookup"><span data-stu-id="67282-183">String</span></span>| <span data-ttu-id="67282-184">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="67282-184">Indicates version of the role definition.</span></span> <span data-ttu-id="67282-185">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="67282-185">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="67282-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="67282-186">Response</span></span>

<span data-ttu-id="67282-187">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="67282-187">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67282-188">Пример</span><span class="sxs-lookup"><span data-stu-id="67282-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="67282-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="67282-189">Request</span></span>

<span data-ttu-id="67282-190">В следующем примере **обновляется единоеroleDefinition** для поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="67282-190">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="67282-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="67282-191">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedroledefinition"
}-->

```http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/0d55728d-3e24-4309-9b1b-5ac09921475a
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
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="67282-192">C#</span><span class="sxs-lookup"><span data-stu-id="67282-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67282-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67282-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67282-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67282-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67282-195">Java</span><span class="sxs-lookup"><span data-stu-id="67282-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="67282-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="67282-196">Response</span></span>

<span data-ttu-id="67282-197">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="67282-197">The following is an example of the response.</span></span>
> <span data-ttu-id="67282-198">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="67282-198">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 OK
Content-type: application/json

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update unifiedroledefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


