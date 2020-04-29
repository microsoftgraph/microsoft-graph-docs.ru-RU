---
title: Тип ресурса deviceAndAppManagementRoleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84a4999e2738d4b068daf88e97896c418f2db6b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441663"
---
# <a name="deviceandappmanagementroleassignment-resource-type"></a><span data-ttu-id="714fe-106">Тип ресурса deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="714fe-106">deviceAndAppManagementRoleAssignment resource type</span></span>

<span data-ttu-id="714fe-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="714fe-107">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="714fe-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="714fe-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="714fe-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="714fe-109">The Role Assignment resource.</span></span> <span data-ttu-id="714fe-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="714fe-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="714fe-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="714fe-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="714fe-112">Это относится как к настраиваемым, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="714fe-112">This applies to custom and built-in roles.</span></span>


<span data-ttu-id="714fe-113">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-113">Inherits from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>

## <a name="methods"></a><span data-ttu-id="714fe-114">Методы</span><span class="sxs-lookup"><span data-stu-id="714fe-114">Methods</span></span>
|<span data-ttu-id="714fe-115">Метод</span><span class="sxs-lookup"><span data-stu-id="714fe-115">Method</span></span>|<span data-ttu-id="714fe-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="714fe-116">Return Type</span></span>|<span data-ttu-id="714fe-117">Описание</span><span class="sxs-lookup"><span data-stu-id="714fe-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="714fe-118">Перечисление объектов deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="714fe-118">List deviceAndAppManagementRoleAssignments</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-list.md)|<span data-ttu-id="714fe-119">Коллекция объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="714fe-119">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="714fe-120">Список свойств и связей объектов [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-120">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>|
|[<span data-ttu-id="714fe-121">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="714fe-121">Get deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-get.md)|<span data-ttu-id="714fe-122">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="714fe-122">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span></span>|<span data-ttu-id="714fe-123">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-123">Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="714fe-124">Создание объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="714fe-124">Create deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-create.md)|<span data-ttu-id="714fe-125">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="714fe-125">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md)</span></span>|<span data-ttu-id="714fe-126">Создание объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-126">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|
|[<span data-ttu-id="714fe-127">Удаление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="714fe-127">Delete deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-delete.md)|<span data-ttu-id="714fe-128">Нет</span><span class="sxs-lookup"><span data-stu-id="714fe-128">None</span></span>|<span data-ttu-id="714fe-129">Удаление объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-129">Deletes a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>|
|[<span data-ttu-id="714fe-130">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="714fe-130">Update deviceAndAppManagementRoleAssignment</span></span>](../api/intune-rbac-deviceandappmanagementroleassignment-update.md)|[<span data-ttu-id="714fe-131">deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="714fe-131">deviceAndAppManagementRoleAssignment</span></span>](../resources/intune-rbac-deviceandappmanagementroleassignment.md)|<span data-ttu-id="714fe-132">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-132">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="714fe-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="714fe-133">Properties</span></span>
|<span data-ttu-id="714fe-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="714fe-134">Property</span></span>|<span data-ttu-id="714fe-135">Тип</span><span class="sxs-lookup"><span data-stu-id="714fe-135">Type</span></span>|<span data-ttu-id="714fe-136">Описание</span><span class="sxs-lookup"><span data-stu-id="714fe-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="714fe-137">id</span><span class="sxs-lookup"><span data-stu-id="714fe-137">id</span></span>|<span data-ttu-id="714fe-138">String</span><span class="sxs-lookup"><span data-stu-id="714fe-138">String</span></span>|<span data-ttu-id="714fe-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="714fe-139">Key of the entity.</span></span> <span data-ttu-id="714fe-140">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="714fe-140">This is read-only and automatically generated.</span></span> <span data-ttu-id="714fe-141">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="714fe-142">displayName</span><span class="sxs-lookup"><span data-stu-id="714fe-142">displayName</span></span>|<span data-ttu-id="714fe-143">Строка</span><span class="sxs-lookup"><span data-stu-id="714fe-143">String</span></span>|<span data-ttu-id="714fe-144">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="714fe-144">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="714fe-145">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="714fe-146">description</span><span class="sxs-lookup"><span data-stu-id="714fe-146">description</span></span>|<span data-ttu-id="714fe-147">String</span><span class="sxs-lookup"><span data-stu-id="714fe-147">String</span></span>|<span data-ttu-id="714fe-148">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="714fe-148">Description of the Role Assignment.</span></span> <span data-ttu-id="714fe-149">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="714fe-150">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="714fe-150">resourceScopes</span></span>|<span data-ttu-id="714fe-151">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="714fe-151">String collection</span></span>|<span data-ttu-id="714fe-152">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="714fe-152">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="714fe-153">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="714fe-153">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="714fe-154">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-154">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="714fe-155">members</span><span class="sxs-lookup"><span data-stu-id="714fe-155">members</span></span>|<span data-ttu-id="714fe-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="714fe-156">String collection</span></span>|<span data-ttu-id="714fe-157">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="714fe-157">The list of ids of role member security groups.</span></span> <span data-ttu-id="714fe-158">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="714fe-158">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="714fe-159">Связи</span><span class="sxs-lookup"><span data-stu-id="714fe-159">Relationships</span></span>
|<span data-ttu-id="714fe-160">Связь</span><span class="sxs-lookup"><span data-stu-id="714fe-160">Relationship</span></span>|<span data-ttu-id="714fe-161">Тип</span><span class="sxs-lookup"><span data-stu-id="714fe-161">Type</span></span>|<span data-ttu-id="714fe-162">Описание</span><span class="sxs-lookup"><span data-stu-id="714fe-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="714fe-163">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="714fe-163">roleDefinition</span></span>|[<span data-ttu-id="714fe-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="714fe-164">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="714fe-165">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="714fe-165">Role definition this assignment is part of.</span></span> <span data-ttu-id="714fe-166">Наследуется от объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="714fe-166">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="714fe-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="714fe-167">JSON Representation</span></span>
<span data-ttu-id="714fe-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="714fe-168">Here is a JSON representation of the resource.</span></span>
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







