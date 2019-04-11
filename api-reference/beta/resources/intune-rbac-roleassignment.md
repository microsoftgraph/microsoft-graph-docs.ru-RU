---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cffebe54ba79d9b013068b9162f9e3a17447b15
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786093"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="ea336-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-106">roleAssignment resource type</span></span>

> <span data-ttu-id="ea336-107">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea336-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea336-108">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea336-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea336-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ea336-109">The Role Assignment resource.</span></span> <span data-ttu-id="ea336-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="ea336-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="ea336-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="ea336-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="ea336-112">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="ea336-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="ea336-113">Методы</span><span class="sxs-lookup"><span data-stu-id="ea336-113">Methods</span></span>
|<span data-ttu-id="ea336-114">Метод</span><span class="sxs-lookup"><span data-stu-id="ea336-114">Method</span></span>|<span data-ttu-id="ea336-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ea336-115">Return Type</span></span>|<span data-ttu-id="ea336-116">Описание</span><span class="sxs-lookup"><span data-stu-id="ea336-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea336-117">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="ea336-118">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ea336-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="ea336-119">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea336-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="ea336-120">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="ea336-121">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-121">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="ea336-122">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea336-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="ea336-123">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="ea336-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-124">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="ea336-125">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea336-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="ea336-126">Удаление roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="ea336-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ea336-127">None</span></span>|<span data-ttu-id="ea336-128">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea336-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="ea336-129">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="ea336-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea336-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="ea336-131">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ea336-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea336-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea336-132">Properties</span></span>
|<span data-ttu-id="ea336-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea336-133">Property</span></span>|<span data-ttu-id="ea336-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ea336-134">Type</span></span>|<span data-ttu-id="ea336-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ea336-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea336-136">id</span><span class="sxs-lookup"><span data-stu-id="ea336-136">id</span></span>|<span data-ttu-id="ea336-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ea336-137">String</span></span>|<span data-ttu-id="ea336-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea336-138">Key of the entity.</span></span> <span data-ttu-id="ea336-139">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ea336-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="ea336-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ea336-140">displayName</span></span>|<span data-ttu-id="ea336-141">String</span><span class="sxs-lookup"><span data-stu-id="ea336-141">String</span></span>|<span data-ttu-id="ea336-142">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ea336-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="ea336-143">description</span><span class="sxs-lookup"><span data-stu-id="ea336-143">description</span></span>|<span data-ttu-id="ea336-144">String</span><span class="sxs-lookup"><span data-stu-id="ea336-144">String</span></span>|<span data-ttu-id="ea336-145">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ea336-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="ea336-146">Скопемемберс</span><span class="sxs-lookup"><span data-stu-id="ea336-146">scopeMembers</span></span>|<span data-ttu-id="ea336-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea336-147">String collection</span></span>|<span data-ttu-id="ea336-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="ea336-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ea336-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea336-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="ea336-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="ea336-150">scopeType</span></span>|[<span data-ttu-id="ea336-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="ea336-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="ea336-152">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ea336-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="ea336-153">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="ea336-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="ea336-154">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="ea336-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="ea336-155">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="ea336-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="ea336-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="ea336-156">resourceScopes</span></span>|<span data-ttu-id="ea336-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea336-157">String collection</span></span>|<span data-ttu-id="ea336-158">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="ea336-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ea336-159">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ea336-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea336-160">Связи</span><span class="sxs-lookup"><span data-stu-id="ea336-160">Relationships</span></span>
|<span data-ttu-id="ea336-161">Отношение</span><span class="sxs-lookup"><span data-stu-id="ea336-161">Relationship</span></span>|<span data-ttu-id="ea336-162">Тип</span><span class="sxs-lookup"><span data-stu-id="ea336-162">Type</span></span>|<span data-ttu-id="ea336-163">Описание</span><span class="sxs-lookup"><span data-stu-id="ea336-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea336-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ea336-164">roleDefinition</span></span>|[<span data-ttu-id="ea336-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ea336-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="ea336-166">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="ea336-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea336-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea336-167">JSON Representation</span></span>
<span data-ttu-id="ea336-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea336-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```





