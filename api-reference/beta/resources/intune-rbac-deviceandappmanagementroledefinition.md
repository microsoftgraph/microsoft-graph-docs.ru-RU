---
title: Тип ресурса deviceAndAppManagementRoleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3de415e6f0ef0ce7efa23c69a6692ecabd054130
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940535"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="11240-109">Тип ресурса deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11240-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="11240-110">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11240-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11240-111">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11240-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11240-112">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="11240-112">The Role Definition resource.</span></span> <span data-ttu-id="11240-113">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="11240-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="11240-114">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="11240-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="11240-115">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="11240-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="11240-116">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="11240-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="11240-117">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="11240-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="11240-118">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="11240-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="11240-119">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="11240-120">Методы</span><span class="sxs-lookup"><span data-stu-id="11240-120">Methods</span></span>
|<span data-ttu-id="11240-121">Метод</span><span class="sxs-lookup"><span data-stu-id="11240-121">Method</span></span>|<span data-ttu-id="11240-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11240-122">Return Type</span></span>|<span data-ttu-id="11240-123">Описание</span><span class="sxs-lookup"><span data-stu-id="11240-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11240-124">Перечисление deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="11240-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="11240-125">Коллекция [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="11240-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="11240-126">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="11240-127">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11240-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|<span data-ttu-id="11240-128">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="11240-128">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span></span>|<span data-ttu-id="11240-129">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="11240-130">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11240-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|<span data-ttu-id="11240-131">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="11240-131">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span></span>|<span data-ttu-id="11240-132">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="11240-133">Удаление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11240-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="11240-134">None</span><span class="sxs-lookup"><span data-stu-id="11240-134">None</span></span>|<span data-ttu-id="11240-135">Удаление экземпляра [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="11240-136">Обновление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11240-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="11240-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="11240-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="11240-138">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11240-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="11240-139">Properties</span></span>
|<span data-ttu-id="11240-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="11240-140">Property</span></span>|<span data-ttu-id="11240-141">Тип</span><span class="sxs-lookup"><span data-stu-id="11240-141">Type</span></span>|<span data-ttu-id="11240-142">Описание</span><span class="sxs-lookup"><span data-stu-id="11240-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11240-143">id</span><span class="sxs-lookup"><span data-stu-id="11240-143">id</span></span>|<span data-ttu-id="11240-144">String</span><span class="sxs-lookup"><span data-stu-id="11240-144">String</span></span>|<span data-ttu-id="11240-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11240-145">Key of the entity.</span></span> <span data-ttu-id="11240-146">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="11240-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="11240-147">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="11240-148">displayName</span><span class="sxs-lookup"><span data-stu-id="11240-148">displayName</span></span>|<span data-ttu-id="11240-149">Строка</span><span class="sxs-lookup"><span data-stu-id="11240-149">String</span></span>|<span data-ttu-id="11240-150">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="11240-150">Display Name of the Role definition.</span></span> <span data-ttu-id="11240-151">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="11240-152">description</span><span class="sxs-lookup"><span data-stu-id="11240-152">description</span></span>|<span data-ttu-id="11240-153">String</span><span class="sxs-lookup"><span data-stu-id="11240-153">String</span></span>|<span data-ttu-id="11240-154">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="11240-154">Description of the Role definition.</span></span> <span data-ttu-id="11240-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="11240-156">permissions</span><span class="sxs-lookup"><span data-stu-id="11240-156">permissions</span></span>|<span data-ttu-id="11240-157">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="11240-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="11240-158">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="11240-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="11240-159">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="11240-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="11240-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="11240-161">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="11240-161">rolePermissions</span></span>|<span data-ttu-id="11240-162">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="11240-162">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="11240-163">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="11240-163">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="11240-164">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="11240-164">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="11240-165">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="11240-166">Исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="11240-166">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="11240-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="11240-167">Boolean</span></span>|<span data-ttu-id="11240-168">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="11240-168">Type of Role.</span></span> <span data-ttu-id="11240-169">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="11240-169">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="11240-170">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-170">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="11240-171">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="11240-171">isBuiltIn</span></span>|<span data-ttu-id="11240-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="11240-172">Boolean</span></span>|<span data-ttu-id="11240-173">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="11240-173">Type of Role.</span></span> <span data-ttu-id="11240-174">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="11240-174">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="11240-175">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-175">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="11240-176">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11240-176">roleScopeTagIds</span></span>|<span data-ttu-id="11240-177">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="11240-177">String collection</span></span>|<span data-ttu-id="11240-178">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="11240-178">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="11240-179">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-179">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="11240-180">Связи</span><span class="sxs-lookup"><span data-stu-id="11240-180">Relationships</span></span>
|<span data-ttu-id="11240-181">Отношение</span><span class="sxs-lookup"><span data-stu-id="11240-181">Relationship</span></span>|<span data-ttu-id="11240-182">Тип</span><span class="sxs-lookup"><span data-stu-id="11240-182">Type</span></span>|<span data-ttu-id="11240-183">Описание</span><span class="sxs-lookup"><span data-stu-id="11240-183">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11240-184">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="11240-184">roleAssignments</span></span>|<span data-ttu-id="11240-185">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="11240-185">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="11240-186">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="11240-186">List of Role assignments for this role definition.</span></span> <span data-ttu-id="11240-187">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="11240-187">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11240-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11240-188">JSON Representation</span></span>
<span data-ttu-id="11240-189">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11240-189">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "String"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




