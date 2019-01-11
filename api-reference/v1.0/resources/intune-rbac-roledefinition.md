---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
localization_priority: Normal
ms.openlocfilehash: d3f5ef8ddd67302b747b2f35b0e4f62f3f6c00d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804818"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="5e8c4-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-109">roleDefinition resource type</span></span>

> <span data-ttu-id="5e8c4-110">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e8c4-111">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="5e8c4-111">The Role Definition resource.</span></span> <span data-ttu-id="5e8c4-112">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="5e8c4-113">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="5e8c4-114">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="5e8c4-115">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="5e8c4-116">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="5e8c4-117">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="5e8c4-118">Методы</span><span class="sxs-lookup"><span data-stu-id="5e8c4-118">Methods</span></span>
|<span data-ttu-id="5e8c4-119">Метод</span><span class="sxs-lookup"><span data-stu-id="5e8c4-119">Method</span></span>|<span data-ttu-id="5e8c4-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e8c4-120">Return Type</span></span>|<span data-ttu-id="5e8c4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5e8c4-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e8c4-122">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="5e8c4-123">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5e8c4-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="5e8c4-124">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5e8c4-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="5e8c4-125">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|[<span data-ttu-id="5e8c4-126">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-126">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="5e8c4-127">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5e8c4-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="5e8c4-128">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|[<span data-ttu-id="5e8c4-129">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-129">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="5e8c4-130">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5e8c4-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="5e8c4-131">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="5e8c4-132">Нет</span><span class="sxs-lookup"><span data-stu-id="5e8c4-132">None</span></span>|<span data-ttu-id="5e8c4-133">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5e8c4-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="5e8c4-134">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="5e8c4-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="5e8c4-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="5e8c4-136">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="5e8c4-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e8c4-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e8c4-137">Properties</span></span>
|<span data-ttu-id="5e8c4-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e8c4-138">Property</span></span>|<span data-ttu-id="5e8c4-139">Тип</span><span class="sxs-lookup"><span data-stu-id="5e8c4-139">Type</span></span>|<span data-ttu-id="5e8c4-140">Описание</span><span class="sxs-lookup"><span data-stu-id="5e8c4-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e8c4-141">id</span><span class="sxs-lookup"><span data-stu-id="5e8c4-141">id</span></span>|<span data-ttu-id="5e8c4-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5e8c4-142">String</span></span>|<span data-ttu-id="5e8c4-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-143">Key of the entity.</span></span> <span data-ttu-id="5e8c4-144">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="5e8c4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5e8c4-145">displayName</span></span>|<span data-ttu-id="5e8c4-146">String</span><span class="sxs-lookup"><span data-stu-id="5e8c4-146">String</span></span>|<span data-ttu-id="5e8c4-147">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="5e8c4-148">описание</span><span class="sxs-lookup"><span data-stu-id="5e8c4-148">description</span></span>|<span data-ttu-id="5e8c4-149">String</span><span class="sxs-lookup"><span data-stu-id="5e8c4-149">String</span></span>|<span data-ttu-id="5e8c4-150">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="5e8c4-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="5e8c4-151">rolePermissions</span></span>|<span data-ttu-id="5e8c4-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="5e8c4-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5e8c4-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5e8c4-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="5e8c4-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5e8c4-155">isBuiltIn</span></span>|<span data-ttu-id="5e8c4-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e8c4-156">Boolean</span></span>|<span data-ttu-id="5e8c4-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-157">Type of Role.</span></span> <span data-ttu-id="5e8c4-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e8c4-159">Связи</span><span class="sxs-lookup"><span data-stu-id="5e8c4-159">Relationships</span></span>
|<span data-ttu-id="5e8c4-160">Связь</span><span class="sxs-lookup"><span data-stu-id="5e8c4-160">Relationship</span></span>|<span data-ttu-id="5e8c4-161">Тип</span><span class="sxs-lookup"><span data-stu-id="5e8c4-161">Type</span></span>|<span data-ttu-id="5e8c4-162">Описание</span><span class="sxs-lookup"><span data-stu-id="5e8c4-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e8c4-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="5e8c4-163">roleAssignments</span></span>|<span data-ttu-id="5e8c4-164">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5e8c4-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="5e8c4-165">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e8c4-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e8c4-166">JSON Representation</span></span>
<span data-ttu-id="5e8c4-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e8c4-167">Here is a JSON representation of the resource.</span></span>
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



