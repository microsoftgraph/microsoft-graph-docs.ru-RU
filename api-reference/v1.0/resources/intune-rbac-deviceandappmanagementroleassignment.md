---
title: Тип ресурса deviceAndAppManagementRoleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 866b7ce675bc3b6765100d730db300eabdd7f0fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037817"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="75224-106">Тип ресурса deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-106">deviceAndAppManagementRoleAssignment resource type</span></span>

<span data-ttu-id="75224-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75224-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75224-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75224-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75224-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="75224-109">The Role Assignment resource.</span></span> <span data-ttu-id="75224-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="75224-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="75224-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="75224-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="75224-112">Это относится как к настраиваемым, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="75224-112">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="75224-113">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-113">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="75224-114">Методы</span><span class="sxs-lookup"><span data-stu-id="75224-114">Methods</span></span>
|<span data-ttu-id="75224-115">Метод</span><span class="sxs-lookup"><span data-stu-id="75224-115">Method</span></span>|<span data-ttu-id="75224-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="75224-116">Return Type</span></span>|<span data-ttu-id="75224-117">Описание</span><span class="sxs-lookup"><span data-stu-id="75224-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75224-118">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-118">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="75224-119">Коллекция объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="75224-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="75224-120">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-120">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="75224-121">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-121">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|[<span data-ttu-id="75224-122">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-122">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="75224-123">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-123">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="75224-124">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-124">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|[<span data-ttu-id="75224-125">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-125">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="75224-126">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-126">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="75224-127">Удаление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-127">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="75224-128">Нет</span><span class="sxs-lookup"><span data-stu-id="75224-128">None</span></span>|<span data-ttu-id="75224-129">Удаление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-129">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="75224-130">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-130">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="75224-131">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75224-131">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="75224-132">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-132">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75224-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="75224-133">Properties</span></span>
|<span data-ttu-id="75224-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="75224-134">Property</span></span>|<span data-ttu-id="75224-135">Тип</span><span class="sxs-lookup"><span data-stu-id="75224-135">Type</span></span>|<span data-ttu-id="75224-136">Описание</span><span class="sxs-lookup"><span data-stu-id="75224-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75224-137">id</span><span class="sxs-lookup"><span data-stu-id="75224-137">id</span></span>|<span data-ttu-id="75224-138">String</span><span class="sxs-lookup"><span data-stu-id="75224-138">String</span></span>|<span data-ttu-id="75224-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75224-139">Key of the entity.</span></span> <span data-ttu-id="75224-140">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="75224-140">This is read-only and automatically generated.</span></span> <span data-ttu-id="75224-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="75224-142">displayName</span><span class="sxs-lookup"><span data-stu-id="75224-142">displayName</span></span>|<span data-ttu-id="75224-143">String</span><span class="sxs-lookup"><span data-stu-id="75224-143">String</span></span>|<span data-ttu-id="75224-144">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="75224-144">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="75224-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="75224-146">description</span><span class="sxs-lookup"><span data-stu-id="75224-146">description</span></span>|<span data-ttu-id="75224-147">String</span><span class="sxs-lookup"><span data-stu-id="75224-147">String</span></span>|<span data-ttu-id="75224-148">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="75224-148">Description of the Role Assignment.</span></span> <span data-ttu-id="75224-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="75224-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="75224-150">resourceScopes</span></span>|<span data-ttu-id="75224-151">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="75224-151">String collection</span></span>|<span data-ttu-id="75224-152">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="75224-152">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="75224-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="75224-153">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="75224-154">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-154">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="75224-155">members</span><span class="sxs-lookup"><span data-stu-id="75224-155">members</span></span>|<span data-ttu-id="75224-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="75224-156">String collection</span></span>|<span data-ttu-id="75224-157">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="75224-157">The list of ids of role member security groups.</span></span> <span data-ttu-id="75224-158">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="75224-158">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75224-159">Связи</span><span class="sxs-lookup"><span data-stu-id="75224-159">Relationships</span></span>
|<span data-ttu-id="75224-160">Связь</span><span class="sxs-lookup"><span data-stu-id="75224-160">Relationship</span></span>|<span data-ttu-id="75224-161">Тип</span><span class="sxs-lookup"><span data-stu-id="75224-161">Type</span></span>|<span data-ttu-id="75224-162">Описание</span><span class="sxs-lookup"><span data-stu-id="75224-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75224-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="75224-163">roleDefinition</span></span>|[<span data-ttu-id="75224-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="75224-164">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="75224-165">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="75224-165">Role definition this assignment is part of.</span></span> <span data-ttu-id="75224-166">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="75224-166">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75224-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75224-167">JSON Representation</span></span>
<span data-ttu-id="75224-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75224-168">Here is a JSON representation of the resource.</span></span>
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









