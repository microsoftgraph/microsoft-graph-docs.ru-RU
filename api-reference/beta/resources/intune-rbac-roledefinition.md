---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d8ec600773f90aba8ecc86bc509efc8da2992fdb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039505"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="581db-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-109">roleDefinition resource type</span></span>

<span data-ttu-id="581db-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="581db-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="581db-111">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="581db-111">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="581db-112">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="581db-112">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="581db-113">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="581db-113">The Role Definition resource.</span></span> <span data-ttu-id="581db-114">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="581db-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="581db-115">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="581db-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="581db-116">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="581db-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="581db-117">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="581db-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="581db-118">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="581db-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="581db-119">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="581db-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="581db-120">Методы</span><span class="sxs-lookup"><span data-stu-id="581db-120">Methods</span></span>
|<span data-ttu-id="581db-121">Метод</span><span class="sxs-lookup"><span data-stu-id="581db-121">Method</span></span>|<span data-ttu-id="581db-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="581db-122">Return Type</span></span>|<span data-ttu-id="581db-123">Описание</span><span class="sxs-lookup"><span data-stu-id="581db-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="581db-124">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="581db-125">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="581db-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="581db-126">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="581db-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="581db-127">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="581db-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="581db-129">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="581db-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="581db-130">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="581db-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="581db-132">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="581db-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="581db-133">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="581db-134">Нет</span><span class="sxs-lookup"><span data-stu-id="581db-134">None</span></span>|<span data-ttu-id="581db-135">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="581db-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="581db-136">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="581db-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="581db-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="581db-138">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="581db-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="581db-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="581db-139">Properties</span></span>
|<span data-ttu-id="581db-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="581db-140">Property</span></span>|<span data-ttu-id="581db-141">Тип</span><span class="sxs-lookup"><span data-stu-id="581db-141">Type</span></span>|<span data-ttu-id="581db-142">Описание</span><span class="sxs-lookup"><span data-stu-id="581db-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581db-143">id</span><span class="sxs-lookup"><span data-stu-id="581db-143">id</span></span>|<span data-ttu-id="581db-144">String</span><span class="sxs-lookup"><span data-stu-id="581db-144">String</span></span>|<span data-ttu-id="581db-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="581db-145">Key of the entity.</span></span> <span data-ttu-id="581db-146">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="581db-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="581db-147">displayName</span><span class="sxs-lookup"><span data-stu-id="581db-147">displayName</span></span>|<span data-ttu-id="581db-148">String</span><span class="sxs-lookup"><span data-stu-id="581db-148">String</span></span>|<span data-ttu-id="581db-149">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="581db-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="581db-150">description</span><span class="sxs-lookup"><span data-stu-id="581db-150">description</span></span>|<span data-ttu-id="581db-151">String</span><span class="sxs-lookup"><span data-stu-id="581db-151">String</span></span>|<span data-ttu-id="581db-152">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="581db-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="581db-153">permissions</span><span class="sxs-lookup"><span data-stu-id="581db-153">permissions</span></span>|<span data-ttu-id="581db-154">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="581db-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="581db-155">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="581db-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="581db-156">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="581db-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="581db-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="581db-157">rolePermissions</span></span>|<span data-ttu-id="581db-158">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="581db-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="581db-159">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="581db-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="581db-160">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="581db-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="581db-161">исбуилтинроледефинитион</span><span class="sxs-lookup"><span data-stu-id="581db-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="581db-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="581db-162">Boolean</span></span>|<span data-ttu-id="581db-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="581db-163">Type of Role.</span></span> <span data-ttu-id="581db-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="581db-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="581db-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="581db-165">isBuiltIn</span></span>|<span data-ttu-id="581db-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="581db-166">Boolean</span></span>|<span data-ttu-id="581db-167">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="581db-167">Type of Role.</span></span> <span data-ttu-id="581db-168">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="581db-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="581db-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="581db-169">roleScopeTagIds</span></span>|<span data-ttu-id="581db-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="581db-170">String collection</span></span>|<span data-ttu-id="581db-171">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="581db-171">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="581db-172">Отношения</span><span class="sxs-lookup"><span data-stu-id="581db-172">Relationships</span></span>
|<span data-ttu-id="581db-173">Связь</span><span class="sxs-lookup"><span data-stu-id="581db-173">Relationship</span></span>|<span data-ttu-id="581db-174">Тип</span><span class="sxs-lookup"><span data-stu-id="581db-174">Type</span></span>|<span data-ttu-id="581db-175">Описание</span><span class="sxs-lookup"><span data-stu-id="581db-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581db-176">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="581db-176">roleAssignments</span></span>|<span data-ttu-id="581db-177">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="581db-177">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="581db-178">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="581db-178">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="581db-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="581db-179">JSON Representation</span></span>
<span data-ttu-id="581db-180">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="581db-180">Here is a JSON representation of the resource.</span></span>
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






