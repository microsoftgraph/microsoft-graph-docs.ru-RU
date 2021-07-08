---
title: Обновление unifiedRoleDefinition
description: Обновление свойств объекта unifiedRoleDefinition.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9e5315a58adc5c6b4447b725ee7315d390d18904
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334719"
---
# <a name="update-unifiedroledefinition"></a><span data-ttu-id="91aaa-103">Обновление unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="91aaa-103">Update unifiedRoleDefinition</span></span>

<span data-ttu-id="91aaa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91aaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91aaa-105">Обновление свойств объекта [unifiedRoleDefinition](../resources/unifiedroledefinition.md) для поставщика RBAC.</span><span class="sxs-lookup"><span data-stu-id="91aaa-105">Update the properties of a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object for an RBAC provider.</span></span>

<span data-ttu-id="91aaa-106">В настоящее время поддерживаются следующие поставщики RBAC:</span><span class="sxs-lookup"><span data-stu-id="91aaa-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="91aaa-107">управление устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="91aaa-107">device management (Intune)</span></span>
- <span data-ttu-id="91aaa-108">каталог (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="91aaa-108">directory (Azure AD)</span></span> 

> [!NOTE]
> <span data-ttu-id="91aaa-109">Поставщик облачных ПК RBAC в настоящее время поддерживает только [список и](rbacapplication-list-roledefinitions.md) [получать](unifiedroledefinition-get.md) операции.</span><span class="sxs-lookup"><span data-stu-id="91aaa-109">The cloud PC RBAC provider currently supports only the [list](rbacapplication-list-roledefinitions.md) and [get](unifiedroledefinition-get.md) operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="91aaa-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91aaa-110">Permissions</span></span>

<span data-ttu-id="91aaa-111">В зависимости от поставщика RBAC и необходимого типа разрешений (делегирования или приложения) выберите из следующей таблицы наименее привилегированное разрешение, необходимое для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="91aaa-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="91aaa-112">Дополнительные данные, [](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) в том числе осторожность перед выбором более привилегированных разрешений, поиск следующих разрешений в ссылке [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91aaa-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in the [Permissions reference](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="91aaa-113">Поддерживаемый поставщик</span><span class="sxs-lookup"><span data-stu-id="91aaa-113">Supported provider</span></span>      | <span data-ttu-id="91aaa-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91aaa-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="91aaa-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91aaa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91aaa-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="91aaa-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="91aaa-117">Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="91aaa-117">Device management</span></span> | <span data-ttu-id="91aaa-118">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-118">DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="91aaa-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91aaa-119">Not supported.</span></span> | <span data-ttu-id="91aaa-120">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-120">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="91aaa-121">Каталог</span><span class="sxs-lookup"><span data-stu-id="91aaa-121">Directory</span></span> | <span data-ttu-id="91aaa-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-122">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> | <span data-ttu-id="91aaa-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91aaa-123">Not supported.</span></span>| <span data-ttu-id="91aaa-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-124">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="91aaa-125">Для поставщика управления устройствами (Intune)</span><span class="sxs-lookup"><span data-stu-id="91aaa-125">For Device management (Intune) provider</span></span>

|<span data-ttu-id="91aaa-126">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91aaa-126">Permission type</span></span>      | <span data-ttu-id="91aaa-127">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91aaa-127">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91aaa-128">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91aaa-128">Delegated (work or school account)</span></span> |  <span data-ttu-id="91aaa-129">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-129">DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="91aaa-130">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91aaa-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91aaa-131">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91aaa-131">Not supported.</span></span>    |
|<span data-ttu-id="91aaa-132">Приложение</span><span class="sxs-lookup"><span data-stu-id="91aaa-132">Application</span></span> | <span data-ttu-id="91aaa-133">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-133">DeviceManagementRBAC.ReadWrite.All</span></span> |

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="91aaa-134">Поставщик каталогов (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="91aaa-134">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="91aaa-135">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91aaa-135">Permission type</span></span>      | <span data-ttu-id="91aaa-136">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91aaa-136">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91aaa-137">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91aaa-137">Delegated (work or school account)</span></span> |  <span data-ttu-id="91aaa-138">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-138">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="91aaa-139">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91aaa-139">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91aaa-140">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91aaa-140">Not supported.</span></span>    |
|<span data-ttu-id="91aaa-141">Приложение</span><span class="sxs-lookup"><span data-stu-id="91aaa-141">Application</span></span> | <span data-ttu-id="91aaa-142">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91aaa-142">RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91aaa-143">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91aaa-143">HTTP request</span></span>

<span data-ttu-id="91aaa-144">Обновление определения ролей для поставщика управления устройствами:</span><span class="sxs-lookup"><span data-stu-id="91aaa-144">To update a role definition for a device management provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/deviceManagement/roleDefinitions/{id}
```

<span data-ttu-id="91aaa-145">Обновление определения ролей для поставщика каталогов:</span><span class="sxs-lookup"><span data-stu-id="91aaa-145">To update a role definition for a directory provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /roleManagement/directory/roleDefinitions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91aaa-146">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91aaa-146">Request headers</span></span>

| <span data-ttu-id="91aaa-147">Имя</span><span class="sxs-lookup"><span data-stu-id="91aaa-147">Name</span></span>       | <span data-ttu-id="91aaa-148">Описание</span><span class="sxs-lookup"><span data-stu-id="91aaa-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="91aaa-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="91aaa-149">Authorization</span></span> | <span data-ttu-id="91aaa-150">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="91aaa-150">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="91aaa-151">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91aaa-151">Request body</span></span>

<span data-ttu-id="91aaa-152">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="91aaa-152">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="91aaa-153">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="91aaa-153">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="91aaa-154">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="91aaa-154">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="91aaa-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="91aaa-155">Property</span></span>     | <span data-ttu-id="91aaa-156">Тип</span><span class="sxs-lookup"><span data-stu-id="91aaa-156">Type</span></span>        | <span data-ttu-id="91aaa-157">Описание</span><span class="sxs-lookup"><span data-stu-id="91aaa-157">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="91aaa-158">description</span><span class="sxs-lookup"><span data-stu-id="91aaa-158">description</span></span>|<span data-ttu-id="91aaa-159">String</span><span class="sxs-lookup"><span data-stu-id="91aaa-159">String</span></span>| <span data-ttu-id="91aaa-160">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="91aaa-160">The description for the role definition.</span></span> <span data-ttu-id="91aaa-161">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="91aaa-161">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="91aaa-162">displayName</span><span class="sxs-lookup"><span data-stu-id="91aaa-162">displayName</span></span>|<span data-ttu-id="91aaa-163">String</span><span class="sxs-lookup"><span data-stu-id="91aaa-163">String</span></span>| <span data-ttu-id="91aaa-164">Имя отображения для определения роли.</span><span class="sxs-lookup"><span data-stu-id="91aaa-164">The display name for the role definition.</span></span> <span data-ttu-id="91aaa-165">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="91aaa-165">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="91aaa-166">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91aaa-166">Required.</span></span>|
|<span data-ttu-id="91aaa-167">id</span><span class="sxs-lookup"><span data-stu-id="91aaa-167">id</span></span>|<span data-ttu-id="91aaa-168">String</span><span class="sxs-lookup"><span data-stu-id="91aaa-168">String</span></span>| <span data-ttu-id="91aaa-169">Уникальный идентификатор определения роли.</span><span class="sxs-lookup"><span data-stu-id="91aaa-169">The unique identifier for the role definition.</span></span> <span data-ttu-id="91aaa-170">Key, not nullable, Read-only.</span><span class="sxs-lookup"><span data-stu-id="91aaa-170">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="91aaa-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="91aaa-171">isBuiltIn</span></span>|<span data-ttu-id="91aaa-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="91aaa-172">Boolean</span></span>| <span data-ttu-id="91aaa-173">Флаг, указывающий, является ли определение роли частью набора по умолчанию, включенного в продукт или настраиваемый.</span><span class="sxs-lookup"><span data-stu-id="91aaa-173">Flag indicating if the role definition is part of the default set included with the product or custom.</span></span> <span data-ttu-id="91aaa-174">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91aaa-174">Read-only.</span></span> |
|<span data-ttu-id="91aaa-175">isEnabled</span><span class="sxs-lookup"><span data-stu-id="91aaa-175">isEnabled</span></span>|<span data-ttu-id="91aaa-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="91aaa-176">Boolean</span></span>| <span data-ttu-id="91aaa-177">Флаг, указывающий, включена ли роль для назначения.</span><span class="sxs-lookup"><span data-stu-id="91aaa-177">Flag indicating if the role is enabled for assignment.</span></span> <span data-ttu-id="91aaa-178">Если значение false, роль недоступна для назначения.</span><span class="sxs-lookup"><span data-stu-id="91aaa-178">If false the role is not available for assignment.</span></span> <span data-ttu-id="91aaa-179">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="91aaa-179">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="91aaa-180">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="91aaa-180">resourceScopes</span></span>|<span data-ttu-id="91aaa-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91aaa-181">String collection</span></span>| <span data-ttu-id="91aaa-182">К списку областей применяются разрешения, предоставленные определением ролей.</span><span class="sxs-lookup"><span data-stu-id="91aaa-182">List of scopes permissions granted by the role definition apply to.</span></span> <span data-ttu-id="91aaa-183">В настоящее время поддерживается только "/".</span><span class="sxs-lookup"><span data-stu-id="91aaa-183">Currently only "/" is supported.</span></span> <span data-ttu-id="91aaa-184">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="91aaa-184">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="91aaa-185">**НЕ ИСПОЛЬЗУЙТЕ. В ближайшее время это свойство будет обесценилось. Прикрепить область к назначению ролей.**</span><span class="sxs-lookup"><span data-stu-id="91aaa-185">**DO NOT USE. This property will be deprecated soon. Attach scope to role assignment.**</span></span>|
|<span data-ttu-id="91aaa-186">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="91aaa-186">rolePermissions</span></span>|<span data-ttu-id="91aaa-187">[коллекция unifiedRolePermission](../resources/unifiedrolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="91aaa-187">[unifiedRolePermission](../resources/unifiedrolepermission.md) collection</span></span>| <span data-ttu-id="91aaa-188">Список разрешений, включенных в роль.</span><span class="sxs-lookup"><span data-stu-id="91aaa-188">List of permissions included in the role.</span></span> <span data-ttu-id="91aaa-189">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="91aaa-189">Read-only when isBuiltIn is true.</span></span> <span data-ttu-id="91aaa-190">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91aaa-190">Required.</span></span> |
|<span data-ttu-id="91aaa-191">templateId</span><span class="sxs-lookup"><span data-stu-id="91aaa-191">templateId</span></span>|<span data-ttu-id="91aaa-192">String</span><span class="sxs-lookup"><span data-stu-id="91aaa-192">String</span></span>| <span data-ttu-id="91aaa-193">Настраиваемый идентификатор шаблона, который можно установить, когда isBuiltIn является ложным.</span><span class="sxs-lookup"><span data-stu-id="91aaa-193">Custom template identifier that can be set when isBuiltIn is false.</span></span> <span data-ttu-id="91aaa-194">Этот идентификатор обычно используется, если требуется, чтобы идентификатор был одинаковым в разных каталогах.</span><span class="sxs-lookup"><span data-stu-id="91aaa-194">This identifier is typically used if one needs an identifier to be the same across different directories.</span></span> <span data-ttu-id="91aaa-195">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="91aaa-195">Read-only when isBuiltIn is true.</span></span> |
|<span data-ttu-id="91aaa-196">inheritsPermissionsFrom</span><span class="sxs-lookup"><span data-stu-id="91aaa-196">inheritsPermissionsFrom</span></span>| <span data-ttu-id="91aaa-197">[коллекция unifiedRoleDefinition](../resources/unifiedroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="91aaa-197">[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection</span></span>| <span data-ttu-id="91aaa-198">Только для чтения набор определений ролей, которые наследует заданное определение роли.</span><span class="sxs-lookup"><span data-stu-id="91aaa-198">Read-only collection of role definitions that the given role definition inherits from.</span></span> <span data-ttu-id="91aaa-199">Только встроенные роли Azure AD поддерживают этот атрибут.</span><span class="sxs-lookup"><span data-stu-id="91aaa-199">Only Azure AD built-in roles support this attribute.</span></span> |
|<span data-ttu-id="91aaa-200">version</span><span class="sxs-lookup"><span data-stu-id="91aaa-200">version</span></span>|<span data-ttu-id="91aaa-201">String</span><span class="sxs-lookup"><span data-stu-id="91aaa-201">String</span></span>| <span data-ttu-id="91aaa-202">Указывает версию определения роли.</span><span class="sxs-lookup"><span data-stu-id="91aaa-202">Indicates version of the role definition.</span></span> <span data-ttu-id="91aaa-203">Только для чтения, когда isBuiltIn является правдой.</span><span class="sxs-lookup"><span data-stu-id="91aaa-203">Read-only when isBuiltIn is true.</span></span>|

## <a name="response"></a><span data-ttu-id="91aaa-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="91aaa-204">Response</span></span>

<span data-ttu-id="91aaa-205">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [unifiedRoleDefinition](../resources/unifiedroledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="91aaa-205">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91aaa-206">Пример</span><span class="sxs-lookup"><span data-stu-id="91aaa-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="91aaa-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="91aaa-207">Request</span></span>

<span data-ttu-id="91aaa-208">В следующем примере **обновляется единоеroleDefinition** для поставщика каталогов.</span><span class="sxs-lookup"><span data-stu-id="91aaa-208">The following example updates a **unifiedRoleDefinition** for a directory provider.</span></span>


# <a name="http"></a>[<span data-ttu-id="91aaa-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="91aaa-209">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="91aaa-210">C#</span><span class="sxs-lookup"><span data-stu-id="91aaa-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedroledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91aaa-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91aaa-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedroledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91aaa-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91aaa-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedroledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91aaa-213">Java</span><span class="sxs-lookup"><span data-stu-id="91aaa-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedroledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91aaa-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="91aaa-214">Response</span></span>

<span data-ttu-id="91aaa-215">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91aaa-215">The following is an example of the response.</span></span>
> <span data-ttu-id="91aaa-216">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91aaa-216">**Note:** The response object shown here might be shortened for readability.</span></span>

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


