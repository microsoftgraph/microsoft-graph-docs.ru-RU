---
title: Тип ресурса roleDefinition
description: 'Ресурс "Определение роли". Определение роли лежит в основе доступа на основе ролей в Intune. Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение. Есть роли двух типов: встроенные и настраиваемые. Встроенные роли невозможно изменить. Как встроенные, так и настраиваемые роли должны включать применяемые назначения. Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fca3587ccb26116257b740a91b376259e1e9dd5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262365"
---
# <a name="roledefinition-resource-type"></a><span data-ttu-id="e0044-109">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0044-109">roleDefinition resource type</span></span>

> <span data-ttu-id="e0044-110">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0044-110">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0044-111">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="e0044-111">The Role Definition resource.</span></span> <span data-ttu-id="e0044-112">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="e0044-112">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="e0044-113">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="e0044-113">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="e0044-114">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="e0044-114">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="e0044-115">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="e0044-115">Built-in roles cannot be modified.</span></span> <span data-ttu-id="e0044-116">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="e0044-116">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="e0044-117">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="e0044-117">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>

## <a name="methods"></a><span data-ttu-id="e0044-118">Методы</span><span class="sxs-lookup"><span data-stu-id="e0044-118">Methods</span></span>
|<span data-ttu-id="e0044-119">Метод</span><span class="sxs-lookup"><span data-stu-id="e0044-119">Method</span></span>|<span data-ttu-id="e0044-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e0044-120">Return Type</span></span>|<span data-ttu-id="e0044-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e0044-121">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0044-122">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0044-122">List roleDefinitions</span></span>](../api/intune-rbac-roledefinition-list.md)|<span data-ttu-id="e0044-123">Коллекция [roleDefinition](../resources/intune-rbac-roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e0044-123">[roleDefinition](../resources/intune-rbac-roledefinition.md) collection</span></span>|<span data-ttu-id="e0044-124">Список свойств и связей объектов [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e0044-124">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="e0044-125">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0044-125">Get roleDefinition</span></span>](../api/intune-rbac-roledefinition-get.md)|<span data-ttu-id="e0044-126">[roleDefinition](../resources/intune-rbac-roledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="e0044-126">[roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|<span data-ttu-id="e0044-127">Чтение свойств и связей объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e0044-127">Read properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="e0044-128">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0044-128">Create roleDefinition</span></span>](../api/intune-rbac-roledefinition-create.md)|<span data-ttu-id="e0044-129">[roleDefinition](../resources/intune-rbac-roledefinition.md);</span><span class="sxs-lookup"><span data-stu-id="e0044-129">[roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|<span data-ttu-id="e0044-130">Создание объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e0044-130">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|
|[<span data-ttu-id="e0044-131">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0044-131">Delete roleDefinition</span></span>](../api/intune-rbac-roledefinition-delete.md)|<span data-ttu-id="e0044-132">Нет</span><span class="sxs-lookup"><span data-stu-id="e0044-132">None</span></span>|<span data-ttu-id="e0044-133">Удаление объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e0044-133">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>|
|[<span data-ttu-id="e0044-134">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0044-134">Update roleDefinition</span></span>](../api/intune-rbac-roledefinition-update.md)|[<span data-ttu-id="e0044-135">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0044-135">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="e0044-136">Обновление свойств объекта [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e0044-136">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0044-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0044-137">Properties</span></span>
|<span data-ttu-id="e0044-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0044-138">Property</span></span>|<span data-ttu-id="e0044-139">Тип</span><span class="sxs-lookup"><span data-stu-id="e0044-139">Type</span></span>|<span data-ttu-id="e0044-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e0044-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0044-141">id</span><span class="sxs-lookup"><span data-stu-id="e0044-141">id</span></span>|<span data-ttu-id="e0044-142">String</span><span class="sxs-lookup"><span data-stu-id="e0044-142">String</span></span>|<span data-ttu-id="e0044-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e0044-143">Key of the entity.</span></span> <span data-ttu-id="e0044-144">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="e0044-144">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e0044-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e0044-145">displayName</span></span>|<span data-ttu-id="e0044-146">String</span><span class="sxs-lookup"><span data-stu-id="e0044-146">String</span></span>|<span data-ttu-id="e0044-147">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="e0044-147">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="e0044-148">description</span><span class="sxs-lookup"><span data-stu-id="e0044-148">description</span></span>|<span data-ttu-id="e0044-149">String</span><span class="sxs-lookup"><span data-stu-id="e0044-149">String</span></span>|<span data-ttu-id="e0044-150">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="e0044-150">Description of the Role definition.</span></span>|
|<span data-ttu-id="e0044-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e0044-151">rolePermissions</span></span>|<span data-ttu-id="e0044-152">Коллекция [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="e0044-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e0044-153">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="e0044-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e0044-154">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="e0044-154">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e0044-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e0044-155">isBuiltIn</span></span>|<span data-ttu-id="e0044-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0044-156">Boolean</span></span>|<span data-ttu-id="e0044-157">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="e0044-157">Type of Role.</span></span> <span data-ttu-id="e0044-158">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="e0044-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0044-159">Связи</span><span class="sxs-lookup"><span data-stu-id="e0044-159">Relationships</span></span>
|<span data-ttu-id="e0044-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="e0044-160">Relationship</span></span>|<span data-ttu-id="e0044-161">Тип</span><span class="sxs-lookup"><span data-stu-id="e0044-161">Type</span></span>|<span data-ttu-id="e0044-162">Описание</span><span class="sxs-lookup"><span data-stu-id="e0044-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0044-163">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="e0044-163">roleAssignments</span></span>|<span data-ttu-id="e0044-164">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e0044-164">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="e0044-165">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="e0044-165">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0044-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0044-166">JSON Representation</span></span>
<span data-ttu-id="e0044-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0044-167">Here is a JSON representation of the resource.</span></span>
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



