---
title: Тип ресурса deviceAndAppManagementRoleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f0f2fc18315b6c07c24cd95f5d88ce81f72e1f3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360806"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="c7556-109">Тип ресурса deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7556-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="c7556-110">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7556-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7556-111">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="c7556-111">The Role Definition resource.</span></span> <span data-ttu-id="c7556-112">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="c7556-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="c7556-113">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="c7556-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="c7556-114">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="c7556-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="c7556-115">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="c7556-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="c7556-116">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="c7556-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="c7556-117">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="c7556-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>


<span data-ttu-id="c7556-118">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-118">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c7556-119">Методы</span><span class="sxs-lookup"><span data-stu-id="c7556-119">Methods</span></span>
|<span data-ttu-id="c7556-120">Метод</span><span class="sxs-lookup"><span data-stu-id="c7556-120">Method</span></span>|<span data-ttu-id="c7556-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c7556-121">Return Type</span></span>|<span data-ttu-id="c7556-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c7556-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7556-123">Перечисление deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="c7556-123">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="c7556-124">Коллекция [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c7556-124">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="c7556-125">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-125">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="c7556-126">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7556-126">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|<span data-ttu-id="c7556-127">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="c7556-127">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span></span>|<span data-ttu-id="c7556-128">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-128">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="c7556-129">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7556-129">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|<span data-ttu-id="c7556-130">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="c7556-130">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span></span>|<span data-ttu-id="c7556-131">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-131">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="c7556-132">Удаление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7556-132">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="c7556-133">None</span><span class="sxs-lookup"><span data-stu-id="c7556-133">None</span></span>|<span data-ttu-id="c7556-134">Удаление экземпляра [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-134">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="c7556-135">Обновление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7556-135">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="c7556-136">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c7556-136">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="c7556-137">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-137">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7556-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7556-138">Properties</span></span>
|<span data-ttu-id="c7556-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7556-139">Property</span></span>|<span data-ttu-id="c7556-140">Тип</span><span class="sxs-lookup"><span data-stu-id="c7556-140">Type</span></span>|<span data-ttu-id="c7556-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c7556-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7556-142">id</span><span class="sxs-lookup"><span data-stu-id="c7556-142">id</span></span>|<span data-ttu-id="c7556-143">String</span><span class="sxs-lookup"><span data-stu-id="c7556-143">String</span></span>|<span data-ttu-id="c7556-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7556-144">Key of the entity.</span></span> <span data-ttu-id="c7556-145">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="c7556-145">This is read-only and automatically generated.</span></span> <span data-ttu-id="c7556-146">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-146">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7556-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c7556-147">displayName</span></span>|<span data-ttu-id="c7556-148">Строка</span><span class="sxs-lookup"><span data-stu-id="c7556-148">String</span></span>|<span data-ttu-id="c7556-149">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="c7556-149">Display Name of the Role definition.</span></span> <span data-ttu-id="c7556-150">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7556-151">description</span><span class="sxs-lookup"><span data-stu-id="c7556-151">description</span></span>|<span data-ttu-id="c7556-152">String</span><span class="sxs-lookup"><span data-stu-id="c7556-152">String</span></span>|<span data-ttu-id="c7556-153">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="c7556-153">Description of the Role definition.</span></span> <span data-ttu-id="c7556-154">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7556-155">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c7556-155">rolePermissions</span></span>|<span data-ttu-id="c7556-156">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c7556-156">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c7556-157">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="c7556-157">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c7556-158">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="c7556-158">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="c7556-159">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="c7556-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c7556-160">isBuiltIn</span></span>|<span data-ttu-id="c7556-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7556-161">Boolean</span></span>|<span data-ttu-id="c7556-162">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="c7556-162">Type of Role.</span></span> <span data-ttu-id="c7556-163">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="c7556-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="c7556-164">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7556-165">Связи</span><span class="sxs-lookup"><span data-stu-id="c7556-165">Relationships</span></span>
|<span data-ttu-id="c7556-166">Связь</span><span class="sxs-lookup"><span data-stu-id="c7556-166">Relationship</span></span>|<span data-ttu-id="c7556-167">Тип</span><span class="sxs-lookup"><span data-stu-id="c7556-167">Type</span></span>|<span data-ttu-id="c7556-168">Описание</span><span class="sxs-lookup"><span data-stu-id="c7556-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7556-169">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="c7556-169">roleAssignments</span></span>|<span data-ttu-id="c7556-170">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7556-170">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="c7556-171">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="c7556-171">List of Role assignments for this role definition.</span></span> <span data-ttu-id="c7556-172">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c7556-172">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7556-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7556-173">JSON Representation</span></span>
<span data-ttu-id="c7556-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7556-174">Here is a JSON representation of the resource.</span></span>
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




