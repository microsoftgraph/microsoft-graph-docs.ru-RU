---
title: Тип ресурса deviceAndAppManagementRoleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e703909f818535eac7ae00284d15620bce55ba80
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253430"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="022b6-109">Тип ресурса deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="022b6-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="022b6-110">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="022b6-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="022b6-111">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="022b6-111">The Role Definition resource.</span></span> <span data-ttu-id="022b6-112">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="022b6-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="022b6-113">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="022b6-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="022b6-114">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="022b6-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="022b6-115">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="022b6-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="022b6-116">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="022b6-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="022b6-117">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="022b6-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="022b6-118">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="022b6-119">Методы</span><span class="sxs-lookup"><span data-stu-id="022b6-119">Methods</span></span>
|<span data-ttu-id="022b6-120">Метод</span><span class="sxs-lookup"><span data-stu-id="022b6-120">Method</span></span>|<span data-ttu-id="022b6-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="022b6-121">Return Type</span></span>|<span data-ttu-id="022b6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="022b6-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="022b6-123">Перечисление deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="022b6-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="022b6-124">Коллекция [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="022b6-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="022b6-125">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="022b6-126">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="022b6-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|<span data-ttu-id="022b6-127">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="022b6-127">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span></span>|<span data-ttu-id="022b6-128">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="022b6-129">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="022b6-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|<span data-ttu-id="022b6-130">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="022b6-130">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span></span>|<span data-ttu-id="022b6-131">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="022b6-132">Удаление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="022b6-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="022b6-133">None</span><span class="sxs-lookup"><span data-stu-id="022b6-133">None</span></span>|<span data-ttu-id="022b6-134">Удаление экземпляра [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="022b6-135">Обновление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="022b6-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="022b6-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="022b6-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="022b6-137">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="022b6-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="022b6-138">Properties</span></span>
|<span data-ttu-id="022b6-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="022b6-139">Property</span></span>|<span data-ttu-id="022b6-140">Тип</span><span class="sxs-lookup"><span data-stu-id="022b6-140">Type</span></span>|<span data-ttu-id="022b6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="022b6-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="022b6-142">id</span><span class="sxs-lookup"><span data-stu-id="022b6-142">id</span></span>|<span data-ttu-id="022b6-143">String</span><span class="sxs-lookup"><span data-stu-id="022b6-143">String</span></span>|<span data-ttu-id="022b6-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="022b6-144">Key of the entity.</span></span> <span data-ttu-id="022b6-145">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="022b6-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="022b6-146">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="022b6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="022b6-147">displayName</span></span>|<span data-ttu-id="022b6-148">String</span><span class="sxs-lookup"><span data-stu-id="022b6-148">String</span></span>|<span data-ttu-id="022b6-149">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="022b6-149">Display Name of the Role definition.</span></span> <span data-ttu-id="022b6-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="022b6-151">description</span><span class="sxs-lookup"><span data-stu-id="022b6-151">description</span></span>|<span data-ttu-id="022b6-152">String</span><span class="sxs-lookup"><span data-stu-id="022b6-152">String</span></span>|<span data-ttu-id="022b6-153">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="022b6-153">Description of the Role definition.</span></span> <span data-ttu-id="022b6-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="022b6-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="022b6-155">rolePermissions</span></span>|<span data-ttu-id="022b6-156">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="022b6-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="022b6-157">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="022b6-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="022b6-158">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="022b6-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="022b6-159">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="022b6-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="022b6-160">isBuiltIn</span></span>|<span data-ttu-id="022b6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="022b6-161">Boolean</span></span>|<span data-ttu-id="022b6-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="022b6-162">Type of Role.</span></span> <span data-ttu-id="022b6-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="022b6-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="022b6-164">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="022b6-165">Связи</span><span class="sxs-lookup"><span data-stu-id="022b6-165">Relationships</span></span>
|<span data-ttu-id="022b6-166">Отношение</span><span class="sxs-lookup"><span data-stu-id="022b6-166">Relationship</span></span>|<span data-ttu-id="022b6-167">Тип</span><span class="sxs-lookup"><span data-stu-id="022b6-167">Type</span></span>|<span data-ttu-id="022b6-168">Описание</span><span class="sxs-lookup"><span data-stu-id="022b6-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="022b6-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="022b6-169">roleAssignments</span></span>|<span data-ttu-id="022b6-170">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="022b6-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="022b6-171">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="022b6-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="022b6-172">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="022b6-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="022b6-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="022b6-173">JSON Representation</span></span>
<span data-ttu-id="022b6-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="022b6-174">Here is a JSON representation of the resource.</span></span>
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



