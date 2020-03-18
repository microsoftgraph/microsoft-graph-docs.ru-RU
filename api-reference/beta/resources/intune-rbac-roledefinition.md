---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0821ff106a6e4265d1b2db9012a433a70ae8af38
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773240"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="4f6cc-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f6cc-109">roleDefinition resource type</span></span>

> <span data-ttu-id="4f6cc-110">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-110">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f6cc-111">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f6cc-112">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="4f6cc-112">The Role Definition resource.</span></span> <span data-ttu-id="4f6cc-113">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="4f6cc-114">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="4f6cc-115">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="4f6cc-116">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="4f6cc-117">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="4f6cc-118">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="4f6cc-119">Методы</span><span class="sxs-lookup"><span data-stu-id="4f6cc-119">Methods</span></span>
|<span data-ttu-id="4f6cc-120">Метод</span><span class="sxs-lookup"><span data-stu-id="4f6cc-120">Method</span></span>|<span data-ttu-id="4f6cc-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f6cc-121">Return Type</span></span>|<span data-ttu-id="4f6cc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6cc-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f6cc-123">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f6cc-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="4f6cc-124">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4f6cc-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="4f6cc-125">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4f6cc-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="4f6cc-126">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f6cc-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|<span data-ttu-id="4f6cc-127">[roleDefinition](../resources/intune-rbac-roledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="4f6cc-127">[roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|<span data-ttu-id="4f6cc-128">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4f6cc-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="4f6cc-129">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f6cc-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|<span data-ttu-id="4f6cc-130">[roleDefinition](../resources/intune-rbac-roledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="4f6cc-130">[roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|<span data-ttu-id="4f6cc-131">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4f6cc-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="4f6cc-132">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f6cc-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="4f6cc-133">Нет</span><span class="sxs-lookup"><span data-stu-id="4f6cc-133">None</span></span>|<span data-ttu-id="4f6cc-134">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4f6cc-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="4f6cc-135">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f6cc-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="4f6cc-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f6cc-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="4f6cc-137">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="4f6cc-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f6cc-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f6cc-138">Properties</span></span>
|<span data-ttu-id="4f6cc-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f6cc-139">Property</span></span>|<span data-ttu-id="4f6cc-140">Тип</span><span class="sxs-lookup"><span data-stu-id="4f6cc-140">Type</span></span>|<span data-ttu-id="4f6cc-141">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6cc-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f6cc-142">id</span><span class="sxs-lookup"><span data-stu-id="4f6cc-142">id</span></span>|<span data-ttu-id="4f6cc-143">String</span><span class="sxs-lookup"><span data-stu-id="4f6cc-143">String</span></span>|<span data-ttu-id="4f6cc-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-144">Key of the entity.</span></span> <span data-ttu-id="4f6cc-145">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="4f6cc-146">displayName</span><span class="sxs-lookup"><span data-stu-id="4f6cc-146">displayName</span></span>|<span data-ttu-id="4f6cc-147">Строка</span><span class="sxs-lookup"><span data-stu-id="4f6cc-147">String</span></span>|<span data-ttu-id="4f6cc-148">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="4f6cc-149">description</span><span class="sxs-lookup"><span data-stu-id="4f6cc-149">description</span></span>|<span data-ttu-id="4f6cc-150">String</span><span class="sxs-lookup"><span data-stu-id="4f6cc-150">String</span></span>|<span data-ttu-id="4f6cc-151">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="4f6cc-152">permissions</span><span class="sxs-lookup"><span data-stu-id="4f6cc-152">permissions</span></span>|<span data-ttu-id="4f6cc-153">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4f6cc-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4f6cc-154">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4f6cc-155">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4f6cc-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="4f6cc-156">rolePermissions</span></span>|<span data-ttu-id="4f6cc-157">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="4f6cc-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="4f6cc-158">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="4f6cc-159">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-159">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="4f6cc-160">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="4f6cc-160">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="4f6cc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f6cc-161">Boolean</span></span>|<span data-ttu-id="4f6cc-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-162">Type of Role.</span></span> <span data-ttu-id="4f6cc-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="4f6cc-164">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="4f6cc-164">isBuiltIn</span></span>|<span data-ttu-id="4f6cc-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f6cc-165">Boolean</span></span>|<span data-ttu-id="4f6cc-166">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-166">Type of Role.</span></span> <span data-ttu-id="4f6cc-167">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-167">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="4f6cc-168">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f6cc-168">roleScopeTagIds</span></span>|<span data-ttu-id="4f6cc-169">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f6cc-169">String collection</span></span>|<span data-ttu-id="4f6cc-170">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-170">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f6cc-171">Связи</span><span class="sxs-lookup"><span data-stu-id="4f6cc-171">Relationships</span></span>
|<span data-ttu-id="4f6cc-172">Связь</span><span class="sxs-lookup"><span data-stu-id="4f6cc-172">Relationship</span></span>|<span data-ttu-id="4f6cc-173">Тип</span><span class="sxs-lookup"><span data-stu-id="4f6cc-173">Type</span></span>|<span data-ttu-id="4f6cc-174">Описание</span><span class="sxs-lookup"><span data-stu-id="4f6cc-174">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f6cc-175">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="4f6cc-175">roleAssignments</span></span>|<span data-ttu-id="4f6cc-176">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4f6cc-176">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="4f6cc-177">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-177">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f6cc-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f6cc-178">JSON Representation</span></span>
<span data-ttu-id="4f6cc-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f6cc-179">Here is a JSON representation of the resource.</span></span>
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



