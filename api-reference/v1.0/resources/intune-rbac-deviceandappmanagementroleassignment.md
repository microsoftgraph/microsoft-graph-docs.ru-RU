---
title: Тип ресурса deviceAndAppManagementRoleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c327790cd34b123e32fd0ad5d96039b22b804b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752296"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="4f077-106">Тип ресурса deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-106">deviceAndAppManagementRoleAssignment resource type</span></span>

<span data-ttu-id="4f077-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f077-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f077-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f077-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f077-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4f077-109">The Role Assignment resource.</span></span> <span data-ttu-id="4f077-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="4f077-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="4f077-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="4f077-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="4f077-112">Это относится как к настраиваемым, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="4f077-112">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="4f077-113">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-113">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4f077-114">Методы</span><span class="sxs-lookup"><span data-stu-id="4f077-114">Methods</span></span>
|<span data-ttu-id="4f077-115">Метод</span><span class="sxs-lookup"><span data-stu-id="4f077-115">Method</span></span>|<span data-ttu-id="4f077-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f077-116">Return Type</span></span>|<span data-ttu-id="4f077-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4f077-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f077-118">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-118">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="4f077-119">Коллекция объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4f077-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="4f077-120">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-120">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="4f077-121">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-121">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="4f077-122">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-122">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="4f077-123">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-123">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="4f077-124">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-124">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="4f077-125">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-125">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="4f077-126">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-126">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="4f077-127">Удаление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-127">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="4f077-128">Нет</span><span class="sxs-lookup"><span data-stu-id="4f077-128">None</span></span>|<span data-ttu-id="4f077-129">Удаление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-129">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="4f077-130">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-130">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="4f077-131">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4f077-131">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="4f077-132">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-132">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f077-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f077-133">Properties</span></span>
|<span data-ttu-id="4f077-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f077-134">Property</span></span>|<span data-ttu-id="4f077-135">Тип</span><span class="sxs-lookup"><span data-stu-id="4f077-135">Type</span></span>|<span data-ttu-id="4f077-136">Описание</span><span class="sxs-lookup"><span data-stu-id="4f077-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f077-137">id</span><span class="sxs-lookup"><span data-stu-id="4f077-137">id</span></span>|<span data-ttu-id="4f077-138">String</span><span class="sxs-lookup"><span data-stu-id="4f077-138">String</span></span>|<span data-ttu-id="4f077-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f077-139">Key of the entity.</span></span> <span data-ttu-id="4f077-140">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="4f077-140">This is read-only and automatically generated.</span></span> <span data-ttu-id="4f077-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="4f077-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4f077-142">displayName</span></span>|<span data-ttu-id="4f077-143">String</span><span class="sxs-lookup"><span data-stu-id="4f077-143">String</span></span>|<span data-ttu-id="4f077-144">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4f077-144">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="4f077-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="4f077-146">description</span><span class="sxs-lookup"><span data-stu-id="4f077-146">description</span></span>|<span data-ttu-id="4f077-147">String</span><span class="sxs-lookup"><span data-stu-id="4f077-147">String</span></span>|<span data-ttu-id="4f077-148">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4f077-148">Description of the Role Assignment.</span></span> <span data-ttu-id="4f077-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="4f077-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="4f077-150">resourceScopes</span></span>|<span data-ttu-id="4f077-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f077-151">String collection</span></span>|<span data-ttu-id="4f077-152">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="4f077-152">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="4f077-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4f077-153">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="4f077-154">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-154">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="4f077-155">members</span><span class="sxs-lookup"><span data-stu-id="4f077-155">members</span></span>|<span data-ttu-id="4f077-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f077-156">String collection</span></span>|<span data-ttu-id="4f077-157">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="4f077-157">The list of ids of role member security groups.</span></span> <span data-ttu-id="4f077-158">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4f077-158">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f077-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="4f077-159">Relationships</span></span>
|<span data-ttu-id="4f077-160">Связь</span><span class="sxs-lookup"><span data-stu-id="4f077-160">Relationship</span></span>|<span data-ttu-id="4f077-161">Тип</span><span class="sxs-lookup"><span data-stu-id="4f077-161">Type</span></span>|<span data-ttu-id="4f077-162">Описание</span><span class="sxs-lookup"><span data-stu-id="4f077-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f077-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f077-163">roleDefinition</span></span>|[<span data-ttu-id="4f077-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="4f077-164">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="4f077-165">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="4f077-165">Role definition this assignment is part of.</span></span> <span data-ttu-id="4f077-166">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4f077-166">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f077-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f077-167">JSON Representation</span></span>
<span data-ttu-id="4f077-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f077-168">Here is a JSON representation of the resource.</span></span>
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




