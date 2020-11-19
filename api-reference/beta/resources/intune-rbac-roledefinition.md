---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 811ce1674c4538c0e6712332bb4ff5b7ad78d881
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222473"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="728ad-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-109">roleDefinition resource type</span></span>

<span data-ttu-id="728ad-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="728ad-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="728ad-111">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="728ad-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="728ad-112">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="728ad-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="728ad-113">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="728ad-113">The Role Definition resource.</span></span> <span data-ttu-id="728ad-114">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="728ad-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="728ad-115">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="728ad-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="728ad-116">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="728ad-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="728ad-117">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="728ad-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="728ad-118">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="728ad-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="728ad-119">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="728ad-120">Методы</span><span class="sxs-lookup"><span data-stu-id="728ad-120">Methods</span></span>
|<span data-ttu-id="728ad-121">Метод</span><span class="sxs-lookup"><span data-stu-id="728ad-121">Method</span></span>|<span data-ttu-id="728ad-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="728ad-122">Return Type</span></span>|<span data-ttu-id="728ad-123">Описание</span><span class="sxs-lookup"><span data-stu-id="728ad-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="728ad-124">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="728ad-125">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="728ad-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="728ad-126">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="728ad-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="728ad-127">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="728ad-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="728ad-129">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="728ad-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="728ad-130">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="728ad-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="728ad-132">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="728ad-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="728ad-133">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="728ad-134">Нет</span><span class="sxs-lookup"><span data-stu-id="728ad-134">None</span></span>|<span data-ttu-id="728ad-135">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="728ad-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="728ad-136">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="728ad-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="728ad-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="728ad-138">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="728ad-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="728ad-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="728ad-139">Properties</span></span>
|<span data-ttu-id="728ad-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="728ad-140">Property</span></span>|<span data-ttu-id="728ad-141">Тип</span><span class="sxs-lookup"><span data-stu-id="728ad-141">Type</span></span>|<span data-ttu-id="728ad-142">Описание</span><span class="sxs-lookup"><span data-stu-id="728ad-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="728ad-143">id</span><span class="sxs-lookup"><span data-stu-id="728ad-143">id</span></span>|<span data-ttu-id="728ad-144">String</span><span class="sxs-lookup"><span data-stu-id="728ad-144">String</span></span>|<span data-ttu-id="728ad-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="728ad-145">Key of the entity.</span></span> <span data-ttu-id="728ad-146">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="728ad-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="728ad-147">displayName</span><span class="sxs-lookup"><span data-stu-id="728ad-147">displayName</span></span>|<span data-ttu-id="728ad-148">String</span><span class="sxs-lookup"><span data-stu-id="728ad-148">String</span></span>|<span data-ttu-id="728ad-149">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="728ad-150">description</span><span class="sxs-lookup"><span data-stu-id="728ad-150">description</span></span>|<span data-ttu-id="728ad-151">String</span><span class="sxs-lookup"><span data-stu-id="728ad-151">String</span></span>|<span data-ttu-id="728ad-152">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="728ad-153">permissions</span><span class="sxs-lookup"><span data-stu-id="728ad-153">permissions</span></span>|<span data-ttu-id="728ad-154">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="728ad-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="728ad-155">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="728ad-156">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="728ad-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="728ad-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="728ad-157">rolePermissions</span></span>|<span data-ttu-id="728ad-158">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="728ad-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="728ad-159">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="728ad-160">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="728ad-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="728ad-161">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="728ad-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="728ad-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="728ad-162">Boolean</span></span>|<span data-ttu-id="728ad-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-163">Type of Role.</span></span> <span data-ttu-id="728ad-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="728ad-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="728ad-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="728ad-165">isBuiltIn</span></span>|<span data-ttu-id="728ad-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="728ad-166">Boolean</span></span>|<span data-ttu-id="728ad-167">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-167">Type of Role.</span></span> <span data-ttu-id="728ad-168">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="728ad-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="728ad-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="728ad-169">roleScopeTagIds</span></span>|<span data-ttu-id="728ad-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="728ad-170">String collection</span></span>|<span data-ttu-id="728ad-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="728ad-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="728ad-172">Связи</span><span class="sxs-lookup"><span data-stu-id="728ad-172">Relationships</span></span>
|<span data-ttu-id="728ad-173">Связь</span><span class="sxs-lookup"><span data-stu-id="728ad-173">Relationship</span></span>|<span data-ttu-id="728ad-174">Тип</span><span class="sxs-lookup"><span data-stu-id="728ad-174">Type</span></span>|<span data-ttu-id="728ad-175">Описание</span><span class="sxs-lookup"><span data-stu-id="728ad-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="728ad-176">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="728ad-176">roleAssignments</span></span>|<span data-ttu-id="728ad-177">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="728ad-177">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="728ad-178">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="728ad-178">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="728ad-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="728ad-179">JSON Representation</span></span>
<span data-ttu-id="728ad-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="728ad-180">Here is a JSON representation of the resource.</span></span>
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




