---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: af8e75ca0364a269168c2c3b072c8c7ec6c087ae
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351078"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="f5e26-103">Обновление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f5e26-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="f5e26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5e26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5e26-105">Обновление свойств объекта [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="f5e26-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="f5e26-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="f5e26-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="f5e26-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="f5e26-107">device management (Intune)</span></span>
- <span data-ttu-id="f5e26-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="f5e26-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="f5e26-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="f5e26-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5e26-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5e26-110">Permissions</span></span>

<span data-ttu-id="f5e26-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f5e26-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="f5e26-112">Дополнительные данные, [](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) в том числе осторожность перед выбором более привилегированных разрешений, поиск следующих разрешений в ссылке [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5e26-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in the [Permissions reference](/graph/permissions-reference).</span></span> 

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="f5e26-113">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="f5e26-113">For Device management (Intune) provider</span></span>

|<span data-ttu-id="f5e26-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5e26-114">Permission type</span></span>      | <span data-ttu-id="f5e26-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5e26-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5e26-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5e26-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="f5e26-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5e26-117">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="f5e26-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5e26-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5e26-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5e26-119">Not supported.</span></span>    |
|<span data-ttu-id="f5e26-120">Application</span><span class="sxs-lookup"><span data-stu-id="f5e26-120">Application</span></span> | <span data-ttu-id="f5e26-121">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5e26-121">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="f5e26-122">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="f5e26-122">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="f5e26-123">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5e26-123">Permission type</span></span>      | <span data-ttu-id="f5e26-124">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5e26-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5e26-125">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5e26-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="f5e26-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5e26-126">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="f5e26-127">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5e26-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5e26-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5e26-128">Not supported.</span></span>    |
|<span data-ttu-id="f5e26-129">Application</span><span class="sxs-lookup"><span data-stu-id="f5e26-129">Application</span></span> | <span data-ttu-id="f5e26-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5e26-130">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5e26-131">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5e26-131">HTTP request</span></span>

<span data-ttu-id="f5e26-132">Обновление определения ролей для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="f5e26-132">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="f5e26-133">Обновление определения ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="f5e26-133">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f5e26-134">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5e26-134">Request headers</span></span>

| <span data-ttu-id="f5e26-135">Имя</span><span class="sxs-lookup"><span data-stu-id="f5e26-135">Name</span></span>       | <span data-ttu-id="f5e26-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f5e26-136">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f5e26-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5e26-137">Authorization</span></span> | <span data-ttu-id="f5e26-138">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f5e26-138">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5e26-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5e26-139">Request body</span></span>

<span data-ttu-id="f5e26-140">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f5e26-140">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f5e26-141">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f5e26-141">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f5e26-142">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f5e26-142">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f5e26-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5e26-143">Property</span></span>     | <span data-ttu-id="f5e26-144">Тип</span><span class="sxs-lookup"><span data-stu-id="f5e26-144">Type</span></span>        | <span data-ttu-id="f5e26-145">Описание</span><span class="sxs-lookup"><span data-stu-id="f5e26-145">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5e26-146">description</span><span class="sxs-lookup"><span data-stu-id="f5e26-146">description</span></span>|<span data-ttu-id="f5e26-147">Строка</span><span class="sxs-lookup"><span data-stu-id="f5e26-147">String</span></span>| <span data-ttu-id="f5e26-148">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="f5e26-148">The description for the role definition.</span></span> <span data-ttu-id="f5e26-149">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="f5e26-149">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="f5e26-150">displayName</span><span class="sxs-lookup"><span data-stu-id="f5e26-150">displayName</span></span>|<span data-ttu-id="f5e26-151">Строка</span><span class="sxs-lookup"><span data-stu-id="f5e26-151">String</span></span>| <span data-ttu-id="f5e26-152">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="f5e26-152">The display name for the role definition.</span></span> <span data-ttu-id="f5e26-153">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="f5e26-153">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="f5e26-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5e26-154">Required.</span></span>|
|<span data-ttu-id="f5e26-155">id</span><span class="sxs-lookup"><span data-stu-id="f5e26-155">id</span></span>|<span data-ttu-id="f5e26-156">Строка</span><span class="sxs-lookup"><span data-stu-id="f5e26-156">String</span></span>| <span data-ttu-id="f5e26-157">Уникальный идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="f5e26-157">The unique identifier for the role definition.</span></span> <span data-ttu-id="f5e26-158">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="f5e26-158">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="f5e26-159">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="f5e26-159">isBuiltIn</span></span>|<span data-ttu-id="f5e26-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5e26-160">Boolean</span></span>| <span data-ttu-id="f5e26-161">Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в продукт или настраиваемый.</span><span class="sxs-lookup"><span data-stu-id="f5e26-161">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="f5e26-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f5e26-162">Read-only.</span></span> |
|<span data-ttu-id="f5e26-163">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f5e26-163">isEnabled</span></span>|<span data-ttu-id="f5e26-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5e26-164">Boolean</span></span>| <span data-ttu-id="f5e26-165">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="f5e26-165">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="f5e26-166">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="f5e26-166">If false the role is not available for assignment.</span></span> <span data-ttu-id="f5e26-167">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="f5e26-167">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="f5e26-168">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="f5e26-168">resourceScopes</span></span>|<span data-ttu-id="f5e26-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f5e26-169">String collection</span></span>| <span data-ttu-id="f5e26-170">К списку областей применяются разрешения, предоставленные определением ролей.</span><span class="sxs-lookup"><span data-stu-id="f5e26-170">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="f5e26-171">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="f5e26-171">Currently only "/" is supported.</span></span> <span data-ttu-id="f5e26-172">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="f5e26-172">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="f5e26-173">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**</span><span class="sxs-lookup"><span data-stu-id="f5e26-173">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="f5e26-174">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="f5e26-174">rolePermissions</span></span>|<span data-ttu-id="f5e26-175">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="f5e26-175">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="f5e26-176">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="f5e26-176">List of permissions included in the role.</span></span> <span data-ttu-id="f5e26-177">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="f5e26-177">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="f5e26-178">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f5e26-178">Required.</span></span> |
|<span data-ttu-id="f5e26-179">templateId</span><span class="sxs-lookup"><span data-stu-id="f5e26-179">templateId</span></span>|<span data-ttu-id="f5e26-180">Строка</span><span class="sxs-lookup"><span data-stu-id="f5e26-180">String</span></span>| <span data-ttu-id="f5e26-181">Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным.</span><span class="sxs-lookup"><span data-stu-id="f5e26-181">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="f5e26-182">Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах.</span><span class="sxs-lookup"><span data-stu-id="f5e26-182">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="f5e26-183">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="f5e26-183">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="f5e26-184">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="f5e26-184">inheritsPermissionsFrom</span></span>| <span data-ttu-id="f5e26-185">[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f5e26-185">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="f5e26-186">Только для чтения набор определений ролей, которые наследует заданное определение роли.</span><span class="sxs-lookup"><span data-stu-id="f5e26-186">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="f5e26-187">Только встроенные роли Azure AD поддерживают этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="f5e26-187">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="f5e26-188">version</span><span class="sxs-lookup"><span data-stu-id="f5e26-188">version</span></span>|<span data-ttu-id="f5e26-189">String</span><span class="sxs-lookup"><span data-stu-id="f5e26-189">String</span></span>| <span data-ttu-id="f5e26-190">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="f5e26-190">Indicates version of the role definition.</span></span> <span data-ttu-id="f5e26-191">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="f5e26-191">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="f5e26-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="f5e26-192">Response</span></span>

<span data-ttu-id="f5e26-193">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f5e26-193">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5e26-194">Пример</span><span class="sxs-lookup"><span data-stu-id="f5e26-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5e26-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5e26-195">Request</span></span>

<span data-ttu-id="f5e26-196">В следующем примере **обновляется единоеroleDefinition** для поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="f5e26-196">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="f5e26-197">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5e26-197">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f5e26-198">C#</span><span class="sxs-lookup"><span data-stu-id="f5e26-198">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5e26-199">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5e26-199">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5e26-200">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5e26-200">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5e26-201">Java</span><span class="sxs-lookup"><span data-stu-id="f5e26-201">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5e26-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5e26-202">Response</span></span>

<span data-ttu-id="f5e26-203">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5e26-203">The following is an example of the response.</span></span>
> <span data-ttu-id="f5e26-204">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f5e26-204">**Note:** The response object shown here might be shortened for readability.</span></span>

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


