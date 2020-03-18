---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3b086cb553040d05dbb5349ab4b63fd31de1132
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773275"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="ffcc1-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcc1-106">roleAssignment resource type</span></span>

> <span data-ttu-id="ffcc1-107">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffcc1-108">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffcc1-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-109">The Role Assignment resource.</span></span> <span data-ttu-id="ffcc1-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="ffcc1-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="ffcc1-112">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="ffcc1-113">Методы</span><span class="sxs-lookup"><span data-stu-id="ffcc1-113">Methods</span></span>
|<span data-ttu-id="ffcc1-114">Метод</span><span class="sxs-lookup"><span data-stu-id="ffcc1-114">Method</span></span>|<span data-ttu-id="ffcc1-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ffcc1-115">Return Type</span></span>|<span data-ttu-id="ffcc1-116">Описание</span><span class="sxs-lookup"><span data-stu-id="ffcc1-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ffcc1-117">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcc1-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="ffcc1-118">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ffcc1-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="ffcc1-119">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffcc1-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="ffcc1-120">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcc1-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|<span data-ttu-id="ffcc1-121">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="ffcc1-121">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="ffcc1-122">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffcc1-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="ffcc1-123">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcc1-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|<span data-ttu-id="ffcc1-124">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="ffcc1-124">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="ffcc1-125">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffcc1-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="ffcc1-126">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcc1-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="ffcc1-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ffcc1-127">None</span></span>|<span data-ttu-id="ffcc1-128">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffcc1-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="ffcc1-129">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcc1-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="ffcc1-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="ffcc1-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="ffcc1-131">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ffcc1-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ffcc1-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffcc1-132">Properties</span></span>
|<span data-ttu-id="ffcc1-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffcc1-133">Property</span></span>|<span data-ttu-id="ffcc1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="ffcc1-134">Type</span></span>|<span data-ttu-id="ffcc1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="ffcc1-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffcc1-136">id</span><span class="sxs-lookup"><span data-stu-id="ffcc1-136">id</span></span>|<span data-ttu-id="ffcc1-137">String</span><span class="sxs-lookup"><span data-stu-id="ffcc1-137">String</span></span>|<span data-ttu-id="ffcc1-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-138">Key of the entity.</span></span> <span data-ttu-id="ffcc1-139">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="ffcc1-140">displayName</span><span class="sxs-lookup"><span data-stu-id="ffcc1-140">displayName</span></span>|<span data-ttu-id="ffcc1-141">Строка</span><span class="sxs-lookup"><span data-stu-id="ffcc1-141">String</span></span>|<span data-ttu-id="ffcc1-142">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="ffcc1-143">description</span><span class="sxs-lookup"><span data-stu-id="ffcc1-143">description</span></span>|<span data-ttu-id="ffcc1-144">String</span><span class="sxs-lookup"><span data-stu-id="ffcc1-144">String</span></span>|<span data-ttu-id="ffcc1-145">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="ffcc1-146">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="ffcc1-146">scopeMembers</span></span>|<span data-ttu-id="ffcc1-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ffcc1-147">String collection</span></span>|<span data-ttu-id="ffcc1-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ffcc1-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="ffcc1-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="ffcc1-150">scopeType</span></span>|<span data-ttu-id="ffcc1-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="ffcc1-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="ffcc1-152">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="ffcc1-153">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="ffcc1-154">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="ffcc1-155">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="ffcc1-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="ffcc1-156">resourceScopes</span></span>|<span data-ttu-id="ffcc1-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ffcc1-157">String collection</span></span>|<span data-ttu-id="ffcc1-158">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="ffcc1-159">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffcc1-160">Связи</span><span class="sxs-lookup"><span data-stu-id="ffcc1-160">Relationships</span></span>
|<span data-ttu-id="ffcc1-161">Связь</span><span class="sxs-lookup"><span data-stu-id="ffcc1-161">Relationship</span></span>|<span data-ttu-id="ffcc1-162">Тип</span><span class="sxs-lookup"><span data-stu-id="ffcc1-162">Type</span></span>|<span data-ttu-id="ffcc1-163">Описание</span><span class="sxs-lookup"><span data-stu-id="ffcc1-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffcc1-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ffcc1-164">roleDefinition</span></span>|[<span data-ttu-id="ffcc1-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="ffcc1-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="ffcc1-166">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffcc1-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffcc1-167">JSON Representation</span></span>
<span data-ttu-id="ffcc1-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffcc1-168">Here is a JSON representation of the resource.</span></span>
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



