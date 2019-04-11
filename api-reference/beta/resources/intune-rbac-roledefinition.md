---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fca5f91c5ca708f715b1438f2fe8508060e3b91c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772008"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="31ff5-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-109">roleDefinition resource type</span></span>

> <span data-ttu-id="31ff5-110">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31ff5-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31ff5-111">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31ff5-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31ff5-112">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="31ff5-112">The Role Definition resource.</span></span> <span data-ttu-id="31ff5-113">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="31ff5-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="31ff5-114">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="31ff5-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="31ff5-115">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="31ff5-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="31ff5-116">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="31ff5-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="31ff5-117">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="31ff5-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="31ff5-118">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="31ff5-119">Методы</span><span class="sxs-lookup"><span data-stu-id="31ff5-119">Methods</span></span>
|<span data-ttu-id="31ff5-120">Метод</span><span class="sxs-lookup"><span data-stu-id="31ff5-120">Method</span></span>|<span data-ttu-id="31ff5-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="31ff5-121">Return Type</span></span>|<span data-ttu-id="31ff5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="31ff5-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31ff5-123">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="31ff5-124">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="31ff5-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="31ff5-125">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="31ff5-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="31ff5-126">Получение roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="31ff5-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="31ff5-128">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="31ff5-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="31ff5-129">Создание roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="31ff5-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="31ff5-131">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="31ff5-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="31ff5-132">Удаление roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="31ff5-133">Нет</span><span class="sxs-lookup"><span data-stu-id="31ff5-133">None</span></span>|<span data-ttu-id="31ff5-134">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="31ff5-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="31ff5-135">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="31ff5-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ff5-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="31ff5-137">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="31ff5-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31ff5-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="31ff5-138">Properties</span></span>
|<span data-ttu-id="31ff5-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="31ff5-139">Property</span></span>|<span data-ttu-id="31ff5-140">Тип</span><span class="sxs-lookup"><span data-stu-id="31ff5-140">Type</span></span>|<span data-ttu-id="31ff5-141">Описание</span><span class="sxs-lookup"><span data-stu-id="31ff5-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ff5-142">id</span><span class="sxs-lookup"><span data-stu-id="31ff5-142">id</span></span>|<span data-ttu-id="31ff5-143">Строка</span><span class="sxs-lookup"><span data-stu-id="31ff5-143">String</span></span>|<span data-ttu-id="31ff5-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="31ff5-144">Key of the entity.</span></span> <span data-ttu-id="31ff5-145">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="31ff5-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="31ff5-146">displayName</span><span class="sxs-lookup"><span data-stu-id="31ff5-146">displayName</span></span>|<span data-ttu-id="31ff5-147">String</span><span class="sxs-lookup"><span data-stu-id="31ff5-147">String</span></span>|<span data-ttu-id="31ff5-148">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="31ff5-149">description</span><span class="sxs-lookup"><span data-stu-id="31ff5-149">description</span></span>|<span data-ttu-id="31ff5-150">String</span><span class="sxs-lookup"><span data-stu-id="31ff5-150">String</span></span>|<span data-ttu-id="31ff5-151">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="31ff5-152">permissions</span><span class="sxs-lookup"><span data-stu-id="31ff5-152">permissions</span></span>|<span data-ttu-id="31ff5-153">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="31ff5-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="31ff5-154">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="31ff5-155">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="31ff5-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="31ff5-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="31ff5-156">rolePermissions</span></span>|<span data-ttu-id="31ff5-157">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="31ff5-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="31ff5-158">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="31ff5-159">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="31ff5-159">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="31ff5-160">Исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="31ff5-160">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="31ff5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ff5-161">Boolean</span></span>|<span data-ttu-id="31ff5-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-162">Type of Role.</span></span> <span data-ttu-id="31ff5-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="31ff5-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="31ff5-164">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="31ff5-164">isBuiltIn</span></span>|<span data-ttu-id="31ff5-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="31ff5-165">Boolean</span></span>|<span data-ttu-id="31ff5-166">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-166">Type of Role.</span></span> <span data-ttu-id="31ff5-167">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="31ff5-167">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="31ff5-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31ff5-168">roleScopeTagIds</span></span>|<span data-ttu-id="31ff5-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="31ff5-169">String collection</span></span>|<span data-ttu-id="31ff5-170">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="31ff5-170">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31ff5-171">Связи</span><span class="sxs-lookup"><span data-stu-id="31ff5-171">Relationships</span></span>
|<span data-ttu-id="31ff5-172">Отношение</span><span class="sxs-lookup"><span data-stu-id="31ff5-172">Relationship</span></span>|<span data-ttu-id="31ff5-173">Тип</span><span class="sxs-lookup"><span data-stu-id="31ff5-173">Type</span></span>|<span data-ttu-id="31ff5-174">Описание</span><span class="sxs-lookup"><span data-stu-id="31ff5-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31ff5-175">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="31ff5-175">roleAssignments</span></span>|<span data-ttu-id="31ff5-176">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="31ff5-176">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="31ff5-177">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="31ff5-177">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31ff5-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31ff5-178">JSON Representation</span></span>
<span data-ttu-id="31ff5-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31ff5-179">Here is a JSON representation of the resource.</span></span>
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





