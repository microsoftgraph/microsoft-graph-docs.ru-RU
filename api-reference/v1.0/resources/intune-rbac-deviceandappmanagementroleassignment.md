---
title: Тип ресурса deviceAndAppManagementRoleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4293b5e7efc29ccf25a2b4c72b6b8ceb1a377a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037186"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="cbeb0-106">Тип ресурса deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbeb0-106">deviceAndAppManagementRoleAssignment resource type</span></span>

> <span data-ttu-id="cbeb0-107">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbeb0-108">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-108">The Role Assignment resource.</span></span> <span data-ttu-id="cbeb0-109">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-109">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="cbeb0-110">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-110">There can be one or more role assignments per role.</span></span> <span data-ttu-id="cbeb0-111">Это относится как к настраиваемым, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-111">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="cbeb0-112">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-112">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cbeb0-113">Методы</span><span class="sxs-lookup"><span data-stu-id="cbeb0-113">Methods</span></span>
|<span data-ttu-id="cbeb0-114">Метод</span><span class="sxs-lookup"><span data-stu-id="cbeb0-114">Method</span></span>|<span data-ttu-id="cbeb0-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cbeb0-115">Return Type</span></span>|<span data-ttu-id="cbeb0-116">Описание</span><span class="sxs-lookup"><span data-stu-id="cbeb0-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cbeb0-117">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbeb0-117">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="cbeb0-118">Коллекция объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cbeb0-118">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="cbeb0-119">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-119">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="cbeb0-120">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbeb0-120">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|<span data-ttu-id="cbeb0-121">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="cbeb0-121">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span></span>|<span data-ttu-id="cbeb0-122">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-122">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="cbeb0-123">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbeb0-123">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|<span data-ttu-id="cbeb0-124">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="cbeb0-124">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span></span>|<span data-ttu-id="cbeb0-125">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-125">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="cbeb0-126">Удаление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbeb0-126">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="cbeb0-127">Нет</span><span class="sxs-lookup"><span data-stu-id="cbeb0-127">None</span></span>|<span data-ttu-id="cbeb0-128">Удаление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-128">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="cbeb0-129">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbeb0-129">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="cbeb0-130">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="cbeb0-130">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="cbeb0-131">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-131">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbeb0-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbeb0-132">Properties</span></span>
|<span data-ttu-id="cbeb0-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbeb0-133">Property</span></span>|<span data-ttu-id="cbeb0-134">Тип</span><span class="sxs-lookup"><span data-stu-id="cbeb0-134">Type</span></span>|<span data-ttu-id="cbeb0-135">Описание</span><span class="sxs-lookup"><span data-stu-id="cbeb0-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbeb0-136">id</span><span class="sxs-lookup"><span data-stu-id="cbeb0-136">id</span></span>|<span data-ttu-id="cbeb0-137">String</span><span class="sxs-lookup"><span data-stu-id="cbeb0-137">String</span></span>|<span data-ttu-id="cbeb0-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-138">Key of the entity.</span></span> <span data-ttu-id="cbeb0-139">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-139">This is read-only and automatically generated.</span></span> <span data-ttu-id="cbeb0-140">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="cbeb0-141">displayName</span><span class="sxs-lookup"><span data-stu-id="cbeb0-141">displayName</span></span>|<span data-ttu-id="cbeb0-142">Строка</span><span class="sxs-lookup"><span data-stu-id="cbeb0-142">String</span></span>|<span data-ttu-id="cbeb0-143">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-143">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="cbeb0-144">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="cbeb0-145">description</span><span class="sxs-lookup"><span data-stu-id="cbeb0-145">description</span></span>|<span data-ttu-id="cbeb0-146">String</span><span class="sxs-lookup"><span data-stu-id="cbeb0-146">String</span></span>|<span data-ttu-id="cbeb0-147">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-147">Description of the Role Assignment.</span></span> <span data-ttu-id="cbeb0-148">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="cbeb0-149">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="cbeb0-149">resourceScopes</span></span>|<span data-ttu-id="cbeb0-150">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cbeb0-150">String collection</span></span>|<span data-ttu-id="cbeb0-151">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-151">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="cbeb0-152">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-152">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="cbeb0-153">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-153">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="cbeb0-154">members</span><span class="sxs-lookup"><span data-stu-id="cbeb0-154">members</span></span>|<span data-ttu-id="cbeb0-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cbeb0-155">String collection</span></span>|<span data-ttu-id="cbeb0-156">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-156">The list of ids of role member security groups.</span></span> <span data-ttu-id="cbeb0-157">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-157">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbeb0-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="cbeb0-158">Relationships</span></span>
|<span data-ttu-id="cbeb0-159">Отношение</span><span class="sxs-lookup"><span data-stu-id="cbeb0-159">Relationship</span></span>|<span data-ttu-id="cbeb0-160">Тип</span><span class="sxs-lookup"><span data-stu-id="cbeb0-160">Type</span></span>|<span data-ttu-id="cbeb0-161">Описание</span><span class="sxs-lookup"><span data-stu-id="cbeb0-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbeb0-162">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="cbeb0-162">roleDefinition</span></span>|[<span data-ttu-id="cbeb0-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="cbeb0-163">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="cbeb0-164">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-164">Role definition this assignment is part of.</span></span> <span data-ttu-id="cbeb0-165">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="cbeb0-165">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbeb0-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbeb0-166">JSON Representation</span></span>
<span data-ttu-id="cbeb0-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbeb0-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```



