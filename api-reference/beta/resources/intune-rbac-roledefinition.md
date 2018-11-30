---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
ms.openlocfilehash: 872985dd3ba99d4afbdbee3b6bc37055f3800020
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082415"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="44ce9-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-109">roleDefinition resource type</span></span>

> <span data-ttu-id="44ce9-110">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44ce9-110">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44ce9-111">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44ce9-111">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44ce9-112">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="44ce9-112">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44ce9-113">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="44ce9-113">The Role Definition resource.</span></span> <span data-ttu-id="44ce9-114">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="44ce9-114">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="44ce9-115">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="44ce9-115">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="44ce9-116">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="44ce9-116">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="44ce9-117">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="44ce9-117">Built-in roles cannot be modified.</span></span> <span data-ttu-id="44ce9-118">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="44ce9-118">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="44ce9-119">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-119">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="44ce9-120">Методы</span><span class="sxs-lookup"><span data-stu-id="44ce9-120">Methods</span></span>
|<span data-ttu-id="44ce9-121">Метод</span><span class="sxs-lookup"><span data-stu-id="44ce9-121">Method</span></span>|<span data-ttu-id="44ce9-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="44ce9-122">Return Type</span></span>|<span data-ttu-id="44ce9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="44ce9-123">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44ce9-124">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-124">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="44ce9-125">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="44ce9-125">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="44ce9-126">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="44ce9-126">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="44ce9-127">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-127">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="44ce9-128">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-128">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="44ce9-129">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="44ce9-129">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="44ce9-130">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-130">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="44ce9-131">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-131">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="44ce9-132">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="44ce9-132">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="44ce9-133">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-133">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="44ce9-134">Нет</span><span class="sxs-lookup"><span data-stu-id="44ce9-134">None</span></span>|<span data-ttu-id="44ce9-135">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="44ce9-135">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="44ce9-136">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-136">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="44ce9-137">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-137">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="44ce9-138">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="44ce9-138">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44ce9-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="44ce9-139">Properties</span></span>
|<span data-ttu-id="44ce9-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="44ce9-140">Property</span></span>|<span data-ttu-id="44ce9-141">Тип</span><span class="sxs-lookup"><span data-stu-id="44ce9-141">Type</span></span>|<span data-ttu-id="44ce9-142">Описание</span><span class="sxs-lookup"><span data-stu-id="44ce9-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ce9-143">id</span><span class="sxs-lookup"><span data-stu-id="44ce9-143">id</span></span>|<span data-ttu-id="44ce9-144">String</span><span class="sxs-lookup"><span data-stu-id="44ce9-144">String</span></span>|<span data-ttu-id="44ce9-145">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="44ce9-145">Key of the entity.</span></span> <span data-ttu-id="44ce9-146">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="44ce9-146">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="44ce9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="44ce9-147">displayName</span></span>|<span data-ttu-id="44ce9-148">String</span><span class="sxs-lookup"><span data-stu-id="44ce9-148">String</span></span>|<span data-ttu-id="44ce9-149">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-149">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="44ce9-150">описание</span><span class="sxs-lookup"><span data-stu-id="44ce9-150">description</span></span>|<span data-ttu-id="44ce9-151">String</span><span class="sxs-lookup"><span data-stu-id="44ce9-151">String</span></span>|<span data-ttu-id="44ce9-152">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-152">Description of the Role definition.</span></span>|
|<span data-ttu-id="44ce9-153">permissions</span><span class="sxs-lookup"><span data-stu-id="44ce9-153">permissions</span></span>|<span data-ttu-id="44ce9-154">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="44ce9-154">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="44ce9-155">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-155">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="44ce9-156">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="44ce9-156">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="44ce9-157">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="44ce9-157">rolePermissions</span></span>|<span data-ttu-id="44ce9-158">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="44ce9-158">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="44ce9-159">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-159">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="44ce9-160">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="44ce9-160">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="44ce9-161">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="44ce9-161">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="44ce9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="44ce9-162">Boolean</span></span>|<span data-ttu-id="44ce9-163">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-163">Type of Role.</span></span> <span data-ttu-id="44ce9-164">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="44ce9-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="44ce9-165">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="44ce9-165">isBuiltIn</span></span>|<span data-ttu-id="44ce9-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="44ce9-166">Boolean</span></span>|<span data-ttu-id="44ce9-167">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-167">Type of Role.</span></span> <span data-ttu-id="44ce9-168">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="44ce9-168">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44ce9-169">Связи</span><span class="sxs-lookup"><span data-stu-id="44ce9-169">Relationships</span></span>
|<span data-ttu-id="44ce9-170">Связь</span><span class="sxs-lookup"><span data-stu-id="44ce9-170">Relationship</span></span>|<span data-ttu-id="44ce9-171">Тип</span><span class="sxs-lookup"><span data-stu-id="44ce9-171">Type</span></span>|<span data-ttu-id="44ce9-172">Описание</span><span class="sxs-lookup"><span data-stu-id="44ce9-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44ce9-173">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="44ce9-173">roleAssignments</span></span>|<span data-ttu-id="44ce9-174">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="44ce9-174">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="44ce9-175">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="44ce9-175">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44ce9-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44ce9-176">JSON Representation</span></span>
<span data-ttu-id="44ce9-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44ce9-177">Here is a JSON representation of the resource.</span></span>
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
  "isBuiltIn": true
}
```





