---
title: Тип ресурса deviceAndAppManagementRoleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 869538f50d30460faa2cb8f43d7fd5f16666144c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095235"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="5ebdf-109">Тип ресурса deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="5ebdf-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ebdf-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ebdf-111">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ebdf-112">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ebdf-113">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="5ebdf-113">The Role Definition resource.</span></span> <span data-ttu-id="5ebdf-114">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="5ebdf-115">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="5ebdf-116">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="5ebdf-117">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="5ebdf-118">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="5ebdf-119">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="5ebdf-120">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="5ebdf-121">Методы</span><span class="sxs-lookup"><span data-stu-id="5ebdf-121">Methods</span></span>
|<span data-ttu-id="5ebdf-122">Метод</span><span class="sxs-lookup"><span data-stu-id="5ebdf-122">Method</span></span>|<span data-ttu-id="5ebdf-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5ebdf-123">Return Type</span></span>|<span data-ttu-id="5ebdf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5ebdf-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ebdf-125">Перечисление deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="5ebdf-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="5ebdf-126">Коллекция [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5ebdf-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="5ebdf-127">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="5ebdf-128">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="5ebdf-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="5ebdf-130">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="5ebdf-131">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="5ebdf-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="5ebdf-133">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="5ebdf-134">Удаление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="5ebdf-135">None</span><span class="sxs-lookup"><span data-stu-id="5ebdf-135">None</span></span>|<span data-ttu-id="5ebdf-136">Удаление экземпляра [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="5ebdf-137">Обновление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="5ebdf-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5ebdf-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="5ebdf-139">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5ebdf-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ebdf-140">Properties</span></span>
|<span data-ttu-id="5ebdf-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ebdf-141">Property</span></span>|<span data-ttu-id="5ebdf-142">Тип</span><span class="sxs-lookup"><span data-stu-id="5ebdf-142">Type</span></span>|<span data-ttu-id="5ebdf-143">Описание</span><span class="sxs-lookup"><span data-stu-id="5ebdf-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebdf-144">id</span><span class="sxs-lookup"><span data-stu-id="5ebdf-144">id</span></span>|<span data-ttu-id="5ebdf-145">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdf-145">String</span></span>|<span data-ttu-id="5ebdf-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-146">Key of the entity.</span></span> <span data-ttu-id="5ebdf-147">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="5ebdf-148">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5ebdf-149">displayName</span><span class="sxs-lookup"><span data-stu-id="5ebdf-149">displayName</span></span>|<span data-ttu-id="5ebdf-150">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdf-150">String</span></span>|<span data-ttu-id="5ebdf-151">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-151">Display Name of the Role definition.</span></span> <span data-ttu-id="5ebdf-152">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5ebdf-153">description</span><span class="sxs-lookup"><span data-stu-id="5ebdf-153">description</span></span>|<span data-ttu-id="5ebdf-154">Строка</span><span class="sxs-lookup"><span data-stu-id="5ebdf-154">String</span></span>|<span data-ttu-id="5ebdf-155">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-155">Description of the Role definition.</span></span> <span data-ttu-id="5ebdf-156">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5ebdf-157">permissions</span><span class="sxs-lookup"><span data-stu-id="5ebdf-157">permissions</span></span>|<span data-ttu-id="5ebdf-158">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5ebdf-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5ebdf-159">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5ebdf-160">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5ebdf-161">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5ebdf-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="5ebdf-162">rolePermissions</span></span>|<span data-ttu-id="5ebdf-163">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5ebdf-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5ebdf-164">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5ebdf-165">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5ebdf-166">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5ebdf-167">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="5ebdf-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="5ebdf-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebdf-168">Boolean</span></span>|<span data-ttu-id="5ebdf-169">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-169">Type of Role.</span></span> <span data-ttu-id="5ebdf-170">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5ebdf-171">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5ebdf-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5ebdf-172">isBuiltIn</span></span>|<span data-ttu-id="5ebdf-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ebdf-173">Boolean</span></span>|<span data-ttu-id="5ebdf-174">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-174">Type of Role.</span></span> <span data-ttu-id="5ebdf-175">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5ebdf-176">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5ebdf-177">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5ebdf-177">roleScopeTagIds</span></span>|<span data-ttu-id="5ebdf-178">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5ebdf-178">String collection</span></span>|<span data-ttu-id="5ebdf-179">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-179">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5ebdf-180">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-180">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ebdf-181">Связи</span><span class="sxs-lookup"><span data-stu-id="5ebdf-181">Relationships</span></span>
|<span data-ttu-id="5ebdf-182">Связь</span><span class="sxs-lookup"><span data-stu-id="5ebdf-182">Relationship</span></span>|<span data-ttu-id="5ebdf-183">Тип</span><span class="sxs-lookup"><span data-stu-id="5ebdf-183">Type</span></span>|<span data-ttu-id="5ebdf-184">Описание</span><span class="sxs-lookup"><span data-stu-id="5ebdf-184">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ebdf-185">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="5ebdf-185">roleAssignments</span></span>|<span data-ttu-id="5ebdf-186">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5ebdf-186">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="5ebdf-187">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-187">List of Role assignments for this role definition.</span></span> <span data-ttu-id="5ebdf-188">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5ebdf-188">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ebdf-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ebdf-189">JSON Representation</span></span>
<span data-ttu-id="5ebdf-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ebdf-190">Here is a JSON representation of the resource.</span></span>
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






