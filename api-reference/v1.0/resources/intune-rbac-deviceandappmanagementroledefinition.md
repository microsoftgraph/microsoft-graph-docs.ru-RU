---
title: Тип ресурса deviceAndAppManagementRoleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a63a990a5a6055c58477cad9d136499a21c68e49
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756787"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="c7e85-109">Тип ресурса deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-109">deviceAndAppManagementRoleDefinition resource type</span></span>

<span data-ttu-id="c7e85-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7e85-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7e85-111">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7e85-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e85-112">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="c7e85-112">The Role Definition resource.</span></span> <span data-ttu-id="c7e85-113">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="c7e85-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="c7e85-114">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="c7e85-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="c7e85-115">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="c7e85-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="c7e85-116">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="c7e85-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="c7e85-117">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="c7e85-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="c7e85-118">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="c7e85-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="c7e85-119">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-119">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c7e85-120">Методы</span><span class="sxs-lookup"><span data-stu-id="c7e85-120">Methods</span></span>
|<span data-ttu-id="c7e85-121">Метод</span><span class="sxs-lookup"><span data-stu-id="c7e85-121">Method</span></span>|<span data-ttu-id="c7e85-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c7e85-122">Return Type</span></span>|<span data-ttu-id="c7e85-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c7e85-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7e85-124">Перечисление deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c7e85-124">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="c7e85-125">Коллекция [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c7e85-125">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="c7e85-126">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-126">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="c7e85-127">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-127">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="c7e85-128">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-128">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="c7e85-129">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-129">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="c7e85-130">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-130">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="c7e85-131">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-131">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="c7e85-132">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-132">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="c7e85-133">Удаление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-133">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="c7e85-134">None</span><span class="sxs-lookup"><span data-stu-id="c7e85-134">None</span></span>|<span data-ttu-id="c7e85-135">Удаление экземпляра [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-135">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="c7e85-136">Обновление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-136">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="c7e85-137">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7e85-137">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="c7e85-138">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-138">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7e85-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7e85-139">Properties</span></span>
|<span data-ttu-id="c7e85-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7e85-140">Property</span></span>|<span data-ttu-id="c7e85-141">Тип</span><span class="sxs-lookup"><span data-stu-id="c7e85-141">Type</span></span>|<span data-ttu-id="c7e85-142">Описание</span><span class="sxs-lookup"><span data-stu-id="c7e85-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e85-143">id</span><span class="sxs-lookup"><span data-stu-id="c7e85-143">id</span></span>|<span data-ttu-id="c7e85-144">String</span><span class="sxs-lookup"><span data-stu-id="c7e85-144">String</span></span>|<span data-ttu-id="c7e85-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7e85-145">Key of the entity.</span></span> <span data-ttu-id="c7e85-146">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="c7e85-146">This is read-only and automatically generated.</span></span> <span data-ttu-id="c7e85-147">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-147">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7e85-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c7e85-148">displayName</span></span>|<span data-ttu-id="c7e85-149">String</span><span class="sxs-lookup"><span data-stu-id="c7e85-149">String</span></span>|<span data-ttu-id="c7e85-150">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="c7e85-150">Display Name of the Role definition.</span></span> <span data-ttu-id="c7e85-151">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-151">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7e85-152">description</span><span class="sxs-lookup"><span data-stu-id="c7e85-152">description</span></span>|<span data-ttu-id="c7e85-153">String</span><span class="sxs-lookup"><span data-stu-id="c7e85-153">String</span></span>|<span data-ttu-id="c7e85-154">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="c7e85-154">Description of the Role definition.</span></span> <span data-ttu-id="c7e85-155">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7e85-156">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c7e85-156">rolePermissions</span></span>|<span data-ttu-id="c7e85-157">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c7e85-157">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c7e85-158">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="c7e85-158">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c7e85-159">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c7e85-159">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="c7e85-160">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7e85-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c7e85-161">isBuiltIn</span></span>|<span data-ttu-id="c7e85-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7e85-162">Boolean</span></span>|<span data-ttu-id="c7e85-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="c7e85-163">Type of Role.</span></span> <span data-ttu-id="c7e85-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="c7e85-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="c7e85-165">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7e85-166">Отношения</span><span class="sxs-lookup"><span data-stu-id="c7e85-166">Relationships</span></span>
|<span data-ttu-id="c7e85-167">Связь</span><span class="sxs-lookup"><span data-stu-id="c7e85-167">Relationship</span></span>|<span data-ttu-id="c7e85-168">Тип</span><span class="sxs-lookup"><span data-stu-id="c7e85-168">Type</span></span>|<span data-ttu-id="c7e85-169">Описание</span><span class="sxs-lookup"><span data-stu-id="c7e85-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e85-170">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c7e85-170">roleAssignments</span></span>|<span data-ttu-id="c7e85-171">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7e85-171">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="c7e85-172">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="c7e85-172">List of Role assignments for this role definition.</span></span> <span data-ttu-id="c7e85-173">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7e85-173">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7e85-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7e85-174">JSON Representation</span></span>
<span data-ttu-id="c7e85-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7e85-175">Here is a JSON representation of the resource.</span></span>
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
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
  "isBuiltIn": true
}
```




