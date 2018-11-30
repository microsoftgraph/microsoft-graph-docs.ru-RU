---
title: Тип ресурса deviceAndAppManagementRoleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
ms.openlocfilehash: 90c701afc33a16cfb2747c40d53d47e74c3cedde
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078080"
---
# <a name="deviceandappmanagementroledefinition-resource-type"></a><span data-ttu-id="a91de-109">Тип ресурса deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-109">deviceAndAppManagementRoleDefinition resource type</span></span>

> <span data-ttu-id="a91de-110">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a91de-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a91de-111">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91de-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a91de-112">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a91de-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a91de-113">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="a91de-113">The Role Definition resource.</span></span> <span data-ttu-id="a91de-114">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="a91de-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="a91de-115">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="a91de-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="a91de-116">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="a91de-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="a91de-117">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="a91de-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="a91de-118">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="a91de-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="a91de-119">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

<span data-ttu-id="a91de-120">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-120">Inherits from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a91de-121">Методы</span><span class="sxs-lookup"><span data-stu-id="a91de-121">Methods</span></span>
|<span data-ttu-id="a91de-122">Метод</span><span class="sxs-lookup"><span data-stu-id="a91de-122">Method</span></span>|<span data-ttu-id="a91de-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a91de-123">Return Type</span></span>|<span data-ttu-id="a91de-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a91de-124">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a91de-125">Перечисление deviceAndAppManagementRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="a91de-125">List deviceAndAppManagementRoleDefinitions</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-list.md)|<span data-ttu-id="a91de-126">Коллекция [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="a91de-126">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) collection</span></span>|<span data-ttu-id="a91de-127">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-127">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>|
|[<span data-ttu-id="a91de-128">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-128">Get deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-get.md)|[<span data-ttu-id="a91de-129">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-129">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="a91de-130">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-130">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="a91de-131">Создание deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-131">Create deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-create.md)|[<span data-ttu-id="a91de-132">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-132">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="a91de-133">Создание объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-133">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|
|[<span data-ttu-id="a91de-134">Удаление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-134">Delete deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-delete.md)|<span data-ttu-id="a91de-135">None</span><span class="sxs-lookup"><span data-stu-id="a91de-135">None</span></span>|<span data-ttu-id="a91de-136">Удаление экземпляра [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-136">Deletes a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>|
|[<span data-ttu-id="a91de-137">Обновление deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-137">Update deviceAndAppManagementRoleDefinition</span></span>](../api/intune-rbac-deviceandappmanagementroledefinition-update.md)|[<span data-ttu-id="a91de-138">deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-138">deviceAndAppManagementRoleDefinition</span></span>](../resources/intune-rbac-deviceandappmanagementroledefinition.md)|<span data-ttu-id="a91de-139">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-139">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a91de-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="a91de-140">Properties</span></span>
|<span data-ttu-id="a91de-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="a91de-141">Property</span></span>|<span data-ttu-id="a91de-142">Тип</span><span class="sxs-lookup"><span data-stu-id="a91de-142">Type</span></span>|<span data-ttu-id="a91de-143">Описание</span><span class="sxs-lookup"><span data-stu-id="a91de-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a91de-144">id</span><span class="sxs-lookup"><span data-stu-id="a91de-144">id</span></span>|<span data-ttu-id="a91de-145">String</span><span class="sxs-lookup"><span data-stu-id="a91de-145">String</span></span>|<span data-ttu-id="a91de-146">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a91de-146">Key of the entity.</span></span> <span data-ttu-id="a91de-147">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="a91de-147">This is read-only and automatically generated.</span></span> <span data-ttu-id="a91de-148">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a91de-149">displayName</span><span class="sxs-lookup"><span data-stu-id="a91de-149">displayName</span></span>|<span data-ttu-id="a91de-150">String</span><span class="sxs-lookup"><span data-stu-id="a91de-150">String</span></span>|<span data-ttu-id="a91de-151">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-151">Display Name of the Role definition.</span></span> <span data-ttu-id="a91de-152">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-152">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a91de-153">описание</span><span class="sxs-lookup"><span data-stu-id="a91de-153">description</span></span>|<span data-ttu-id="a91de-154">String</span><span class="sxs-lookup"><span data-stu-id="a91de-154">String</span></span>|<span data-ttu-id="a91de-155">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-155">Description of the Role definition.</span></span> <span data-ttu-id="a91de-156">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-156">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a91de-157">permissions</span><span class="sxs-lookup"><span data-stu-id="a91de-157">permissions</span></span>|<span data-ttu-id="a91de-158">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a91de-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a91de-159">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a91de-160">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="a91de-160">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="a91de-161">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-161">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a91de-162">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a91de-162">rolePermissions</span></span>|<span data-ttu-id="a91de-163">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="a91de-163">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a91de-164">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-164">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a91de-165">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="a91de-165">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="a91de-166">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-166">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a91de-167">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a91de-167">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="a91de-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a91de-168">Boolean</span></span>|<span data-ttu-id="a91de-169">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-169">Type of Role.</span></span> <span data-ttu-id="a91de-170">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="a91de-170">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="a91de-171">Наследуется от объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-171">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="a91de-172">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a91de-172">isBuiltIn</span></span>|<span data-ttu-id="a91de-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a91de-173">Boolean</span></span>|<span data-ttu-id="a91de-174">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-174">Type of Role.</span></span> <span data-ttu-id="a91de-175">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="a91de-175">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="a91de-176">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-176">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a91de-177">Связи</span><span class="sxs-lookup"><span data-stu-id="a91de-177">Relationships</span></span>
|<span data-ttu-id="a91de-178">Связь</span><span class="sxs-lookup"><span data-stu-id="a91de-178">Relationship</span></span>|<span data-ttu-id="a91de-179">Тип</span><span class="sxs-lookup"><span data-stu-id="a91de-179">Type</span></span>|<span data-ttu-id="a91de-180">Описание</span><span class="sxs-lookup"><span data-stu-id="a91de-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a91de-181">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="a91de-181">roleAssignments</span></span>|<span data-ttu-id="a91de-182">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a91de-182">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="a91de-183">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="a91de-183">List of Role assignments for this role definition.</span></span> <span data-ttu-id="a91de-184">Наследуется от [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="a91de-184">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a91de-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a91de-185">JSON Representation</span></span>
<span data-ttu-id="a91de-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a91de-186">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





