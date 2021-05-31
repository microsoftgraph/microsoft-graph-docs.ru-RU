---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 47ff9ff4c40360ddb28d5d6d344ca1d7375cc119
ms.sourcegitcommit: 30903b12daf4cf2841524c57743889e23d11f85a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2021
ms.locfileid: "52709495"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="74a71-103">Обновление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="74a71-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="74a71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74a71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74a71-105">Обновление свойств объекта [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="74a71-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="74a71-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="74a71-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="74a71-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="74a71-107">device management (Intune)</span></span>
- <span data-ttu-id="74a71-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="74a71-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="74a71-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="74a71-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="74a71-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74a71-110">Permissions</span></span>

<span data-ttu-id="74a71-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="74a71-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="74a71-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74a71-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="74a71-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="74a71-113">Supported provider</span></span>      | <span data-ttu-id="74a71-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74a71-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="74a71-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74a71-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74a71-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74a71-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="74a71-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="74a71-117">Device management</span></span> | <span data-ttu-id="74a71-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74a71-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="74a71-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74a71-119">Not supported.</span></span> | <span data-ttu-id="74a71-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74a71-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="74a71-121">Каталог</span><span class="sxs-lookup"><span data-stu-id="74a71-121">Directory</span></span> | <span data-ttu-id="74a71-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="74a71-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="74a71-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74a71-123">Not supported.</span></span>| <span data-ttu-id="74a71-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74a71-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74a71-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74a71-125">HTTP request</span></span>

<span data-ttu-id="74a71-126">Обновление определения ролей для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="74a71-126">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="74a71-127">Обновление определения ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="74a71-127">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="74a71-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74a71-128">Request headers</span></span>

| <span data-ttu-id="74a71-129">Имя</span><span class="sxs-lookup"><span data-stu-id="74a71-129">Name</span></span>       | <span data-ttu-id="74a71-130">Описание</span><span class="sxs-lookup"><span data-stu-id="74a71-130">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="74a71-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74a71-131">Authorization</span></span> | <span data-ttu-id="74a71-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="74a71-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="74a71-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="74a71-133">Request body</span></span>

<span data-ttu-id="74a71-134">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="74a71-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="74a71-135">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="74a71-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="74a71-136">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="74a71-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="74a71-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="74a71-137">Property</span></span>     | <span data-ttu-id="74a71-138">Тип</span><span class="sxs-lookup"><span data-stu-id="74a71-138">Type</span></span>        | <span data-ttu-id="74a71-139">Описание</span><span class="sxs-lookup"><span data-stu-id="74a71-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74a71-140">description</span><span class="sxs-lookup"><span data-stu-id="74a71-140">description</span></span>|<span data-ttu-id="74a71-141">String</span><span class="sxs-lookup"><span data-stu-id="74a71-141">String</span></span>| <span data-ttu-id="74a71-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="74a71-142">The description for the role definition.</span></span> <span data-ttu-id="74a71-143">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="74a71-143">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="74a71-144">displayName</span><span class="sxs-lookup"><span data-stu-id="74a71-144">displayName</span></span>|<span data-ttu-id="74a71-145">String</span><span class="sxs-lookup"><span data-stu-id="74a71-145">String</span></span>| <span data-ttu-id="74a71-146">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="74a71-146">The display name for the role definition.</span></span> <span data-ttu-id="74a71-147">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="74a71-147">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="74a71-148">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74a71-148">Required.</span></span>|
|<span data-ttu-id="74a71-149">id</span><span class="sxs-lookup"><span data-stu-id="74a71-149">id</span></span>|<span data-ttu-id="74a71-150">String</span><span class="sxs-lookup"><span data-stu-id="74a71-150">String</span></span>| <span data-ttu-id="74a71-151">Уникальный идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="74a71-151">The unique identifier for the role definition.</span></span> <span data-ttu-id="74a71-152">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="74a71-152">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="74a71-153">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="74a71-153">isBuiltIn</span></span>|<span data-ttu-id="74a71-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="74a71-154">Boolean</span></span>| <span data-ttu-id="74a71-155">Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в продукт или настраиваемый.</span><span class="sxs-lookup"><span data-stu-id="74a71-155">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="74a71-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74a71-156">Read-only.</span></span> |
|<span data-ttu-id="74a71-157">isEnabled</span><span class="sxs-lookup"><span data-stu-id="74a71-157">isEnabled</span></span>|<span data-ttu-id="74a71-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="74a71-158">Boolean</span></span>| <span data-ttu-id="74a71-159">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="74a71-159">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="74a71-160">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="74a71-160">If false the role is not available for assignment.</span></span> <span data-ttu-id="74a71-161">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="74a71-161">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="74a71-162">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="74a71-162">resourceScopes</span></span>|<span data-ttu-id="74a71-163">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="74a71-163">String collection</span></span>| <span data-ttu-id="74a71-164">К списку областей применяются разрешения, предоставленные определением ролей.</span><span class="sxs-lookup"><span data-stu-id="74a71-164">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="74a71-165">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="74a71-165">Currently only "/" is supported.</span></span> <span data-ttu-id="74a71-166">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="74a71-166">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="74a71-167">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**</span><span class="sxs-lookup"><span data-stu-id="74a71-167">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="74a71-168">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="74a71-168">rolePermissions</span></span>|<span data-ttu-id="74a71-169">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="74a71-169">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="74a71-170">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="74a71-170">List of permissions included in the role.</span></span> <span data-ttu-id="74a71-171">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="74a71-171">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="74a71-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74a71-172">Required.</span></span> |
|<span data-ttu-id="74a71-173">templateId</span><span class="sxs-lookup"><span data-stu-id="74a71-173">templateId</span></span>|<span data-ttu-id="74a71-174">String</span><span class="sxs-lookup"><span data-stu-id="74a71-174">String</span></span>| <span data-ttu-id="74a71-175">Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным.</span><span class="sxs-lookup"><span data-stu-id="74a71-175">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="74a71-176">Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах.</span><span class="sxs-lookup"><span data-stu-id="74a71-176">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="74a71-177">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="74a71-177">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="74a71-178">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="74a71-178">inheritsPermissionsFrom</span></span>| <span data-ttu-id="74a71-179">[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="74a71-179">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="74a71-180">Только для чтения набор определений ролей, которые наследует заданное определение роли.</span><span class="sxs-lookup"><span data-stu-id="74a71-180">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="74a71-181">Только встроенные роли Azure AD поддерживают этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="74a71-181">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="74a71-182">version</span><span class="sxs-lookup"><span data-stu-id="74a71-182">version</span></span>|<span data-ttu-id="74a71-183">String</span><span class="sxs-lookup"><span data-stu-id="74a71-183">String</span></span>| <span data-ttu-id="74a71-184">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="74a71-184">Indicates version of the role definition.</span></span> <span data-ttu-id="74a71-185">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="74a71-185">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="74a71-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="74a71-186">Response</span></span>

<span data-ttu-id="74a71-187">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="74a71-187">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74a71-188">Пример</span><span class="sxs-lookup"><span data-stu-id="74a71-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="74a71-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="74a71-189">Request</span></span>

<span data-ttu-id="74a71-190">В следующем примере **обновляется единоеroleDefinition** для поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="74a71-190">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="74a71-191">HTTP</span><span class="sxs-lookup"><span data-stu-id="74a71-191">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="74a71-192">C#</span><span class="sxs-lookup"><span data-stu-id="74a71-192">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74a71-193">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74a71-193">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74a71-194">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74a71-194">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74a71-195">Java</span><span class="sxs-lookup"><span data-stu-id="74a71-195">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74a71-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="74a71-196">Response</span></span>

<span data-ttu-id="74a71-197">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="74a71-197">The following is an example of the response.</span></span>
> <span data-ttu-id="74a71-198">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="74a71-198">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
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


