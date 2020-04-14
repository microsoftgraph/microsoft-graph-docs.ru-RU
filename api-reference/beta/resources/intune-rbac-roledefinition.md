---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8570b97edc71a86e5ade007a3d7d512683ca4332
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356942"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="eccbd-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eccbd-109">roleDefinition resource type</span></span>

<span data-ttu-id="eccbd-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eccbd-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eccbd-111">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eccbd-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eccbd-112">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eccbd-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eccbd-113">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="eccbd-113">The Role Definition resource.</span></span> <span data-ttu-id="eccbd-114">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="eccbd-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="eccbd-115">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="eccbd-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="eccbd-116">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="eccbd-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="eccbd-117">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="eccbd-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="eccbd-118">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="eccbd-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="eccbd-119">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="eccbd-120">Методы</span><span class="sxs-lookup"><span data-stu-id="eccbd-120">Methods</span></span>
|<span data-ttu-id="eccbd-121">Метод</span><span class="sxs-lookup"><span data-stu-id="eccbd-121">Method</span></span>|<span data-ttu-id="eccbd-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eccbd-122">Return Type</span></span>|<span data-ttu-id="eccbd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="eccbd-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eccbd-124">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eccbd-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="eccbd-125">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eccbd-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="eccbd-126">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="eccbd-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="eccbd-127">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eccbd-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|<span data-ttu-id="eccbd-128">[roleDefinition](../resources/intune-rbac-roledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="eccbd-128">[roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|<span data-ttu-id="eccbd-129">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="eccbd-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="eccbd-130">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eccbd-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|<span data-ttu-id="eccbd-131">[roleDefinition](../resources/intune-rbac-roledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="eccbd-131">[roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|<span data-ttu-id="eccbd-132">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="eccbd-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="eccbd-133">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eccbd-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="eccbd-134">Нет</span><span class="sxs-lookup"><span data-stu-id="eccbd-134">None</span></span>|<span data-ttu-id="eccbd-135">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="eccbd-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="eccbd-136">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eccbd-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="eccbd-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eccbd-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="eccbd-138">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="eccbd-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eccbd-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="eccbd-139">Properties</span></span>
|<span data-ttu-id="eccbd-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="eccbd-140">Property</span></span>|<span data-ttu-id="eccbd-141">Тип</span><span class="sxs-lookup"><span data-stu-id="eccbd-141">Type</span></span>|<span data-ttu-id="eccbd-142">Описание</span><span class="sxs-lookup"><span data-stu-id="eccbd-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eccbd-143">id</span><span class="sxs-lookup"><span data-stu-id="eccbd-143">id</span></span>|<span data-ttu-id="eccbd-144">String</span><span class="sxs-lookup"><span data-stu-id="eccbd-144">String</span></span>|<span data-ttu-id="eccbd-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eccbd-145">Key of the entity.</span></span> <span data-ttu-id="eccbd-146">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="eccbd-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="eccbd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="eccbd-147">displayName</span></span>|<span data-ttu-id="eccbd-148">Строка</span><span class="sxs-lookup"><span data-stu-id="eccbd-148">String</span></span>|<span data-ttu-id="eccbd-149">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="eccbd-150">description</span><span class="sxs-lookup"><span data-stu-id="eccbd-150">description</span></span>|<span data-ttu-id="eccbd-151">String</span><span class="sxs-lookup"><span data-stu-id="eccbd-151">String</span></span>|<span data-ttu-id="eccbd-152">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="eccbd-153">permissions</span><span class="sxs-lookup"><span data-stu-id="eccbd-153">permissions</span></span>|<span data-ttu-id="eccbd-154">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="eccbd-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="eccbd-155">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="eccbd-156">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="eccbd-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="eccbd-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="eccbd-157">rolePermissions</span></span>|<span data-ttu-id="eccbd-158">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="eccbd-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="eccbd-159">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="eccbd-160">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="eccbd-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="eccbd-161">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="eccbd-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="eccbd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eccbd-162">Boolean</span></span>|<span data-ttu-id="eccbd-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-163">Type of Role.</span></span> <span data-ttu-id="eccbd-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="eccbd-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="eccbd-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="eccbd-165">isBuiltIn</span></span>|<span data-ttu-id="eccbd-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="eccbd-166">Boolean</span></span>|<span data-ttu-id="eccbd-167">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-167">Type of Role.</span></span> <span data-ttu-id="eccbd-168">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="eccbd-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="eccbd-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eccbd-169">roleScopeTagIds</span></span>|<span data-ttu-id="eccbd-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eccbd-170">String collection</span></span>|<span data-ttu-id="eccbd-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="eccbd-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eccbd-172">Связи</span><span class="sxs-lookup"><span data-stu-id="eccbd-172">Relationships</span></span>
|<span data-ttu-id="eccbd-173">Связь</span><span class="sxs-lookup"><span data-stu-id="eccbd-173">Relationship</span></span>|<span data-ttu-id="eccbd-174">Тип</span><span class="sxs-lookup"><span data-stu-id="eccbd-174">Type</span></span>|<span data-ttu-id="eccbd-175">Описание</span><span class="sxs-lookup"><span data-stu-id="eccbd-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eccbd-176">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="eccbd-176">roleAssignments</span></span>|<span data-ttu-id="eccbd-177">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eccbd-177">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="eccbd-178">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="eccbd-178">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eccbd-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eccbd-179">JSON Representation</span></span>
<span data-ttu-id="eccbd-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eccbd-180">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
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



