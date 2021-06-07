---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff5403f7741191021d45aeb6dfb87b2a299f4b85
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751190"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="dae6e-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-109">roleDefinition resource type</span></span>

<span data-ttu-id="dae6e-110">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dae6e-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dae6e-111">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dae6e-111">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dae6e-112">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="dae6e-112">The Role Definition resource.</span></span> <span data-ttu-id="dae6e-113">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="dae6e-113">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="dae6e-114">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="dae6e-114">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="dae6e-115">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="dae6e-115">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="dae6e-116">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="dae6e-116">Built-in roles cannot be modified.</span></span> <span data-ttu-id="dae6e-117">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="dae6e-117">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="dae6e-118">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="dae6e-118">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="dae6e-119">Методы</span><span class="sxs-lookup"><span data-stu-id="dae6e-119">Methods</span></span>
|<span data-ttu-id="dae6e-120">Метод</span><span class="sxs-lookup"><span data-stu-id="dae6e-120">Method</span></span>|<span data-ttu-id="dae6e-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dae6e-121">Return Type</span></span>|<span data-ttu-id="dae6e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dae6e-122">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dae6e-123">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-123">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="dae6e-124">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="dae6e-124">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="dae6e-125">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dae6e-125">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="dae6e-126">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-126">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="dae6e-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-127">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="dae6e-128">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dae6e-128">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="dae6e-129">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-129">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="dae6e-130">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-130">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="dae6e-131">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dae6e-131">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="dae6e-132">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-132">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="dae6e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="dae6e-133">None</span></span>|<span data-ttu-id="dae6e-134">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dae6e-134">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="dae6e-135">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-135">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="dae6e-136">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="dae6e-136">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="dae6e-137">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dae6e-137">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dae6e-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="dae6e-138">Properties</span></span>
|<span data-ttu-id="dae6e-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="dae6e-139">Property</span></span>|<span data-ttu-id="dae6e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="dae6e-140">Type</span></span>|<span data-ttu-id="dae6e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="dae6e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dae6e-142">id</span><span class="sxs-lookup"><span data-stu-id="dae6e-142">id</span></span>|<span data-ttu-id="dae6e-143">String</span><span class="sxs-lookup"><span data-stu-id="dae6e-143">String</span></span>|<span data-ttu-id="dae6e-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dae6e-144">Key of the entity.</span></span> <span data-ttu-id="dae6e-145">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="dae6e-145">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="dae6e-146">displayName</span><span class="sxs-lookup"><span data-stu-id="dae6e-146">displayName</span></span>|<span data-ttu-id="dae6e-147">String</span><span class="sxs-lookup"><span data-stu-id="dae6e-147">String</span></span>|<span data-ttu-id="dae6e-148">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="dae6e-148">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="dae6e-149">description</span><span class="sxs-lookup"><span data-stu-id="dae6e-149">description</span></span>|<span data-ttu-id="dae6e-150">String</span><span class="sxs-lookup"><span data-stu-id="dae6e-150">String</span></span>|<span data-ttu-id="dae6e-151">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="dae6e-151">Description of the Role definition.</span></span>|
|<span data-ttu-id="dae6e-152">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="dae6e-152">rolePermissions</span></span>|<span data-ttu-id="dae6e-153">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="dae6e-153">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="dae6e-154">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="dae6e-154">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="dae6e-155">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="dae6e-155">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="dae6e-156">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="dae6e-156">isBuiltIn</span></span>|<span data-ttu-id="dae6e-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="dae6e-157">Boolean</span></span>|<span data-ttu-id="dae6e-158">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="dae6e-158">Type of Role.</span></span> <span data-ttu-id="dae6e-159">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="dae6e-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dae6e-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="dae6e-160">Relationships</span></span>
|<span data-ttu-id="dae6e-161">Связь</span><span class="sxs-lookup"><span data-stu-id="dae6e-161">Relationship</span></span>|<span data-ttu-id="dae6e-162">Тип</span><span class="sxs-lookup"><span data-stu-id="dae6e-162">Type</span></span>|<span data-ttu-id="dae6e-163">Описание</span><span class="sxs-lookup"><span data-stu-id="dae6e-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dae6e-164">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="dae6e-164">roleAssignments</span></span>|<span data-ttu-id="dae6e-165">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dae6e-165">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="dae6e-166">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="dae6e-166">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dae6e-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dae6e-167">JSON Representation</span></span>
<span data-ttu-id="dae6e-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dae6e-168">Here is a JSON representation of the resource.</span></span>
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




