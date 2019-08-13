---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к пользовательским, так и ко встроенным ролям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9f9a76366ca97464b4180a693e85d8d68d7358a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369257"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="55eab-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="55eab-106">roleAssignment resource type</span></span>

> <span data-ttu-id="55eab-107">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55eab-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55eab-108">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55eab-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55eab-109">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="55eab-109">The Role Assignment resource.</span></span> <span data-ttu-id="55eab-110">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="55eab-110">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="55eab-111">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="55eab-111">There can be one or more role assignments per role.</span></span> <span data-ttu-id="55eab-112">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="55eab-112">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="55eab-113">Методы</span><span class="sxs-lookup"><span data-stu-id="55eab-113">Methods</span></span>
|<span data-ttu-id="55eab-114">Метод</span><span class="sxs-lookup"><span data-stu-id="55eab-114">Method</span></span>|<span data-ttu-id="55eab-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55eab-115">Return Type</span></span>|<span data-ttu-id="55eab-116">Описание</span><span class="sxs-lookup"><span data-stu-id="55eab-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="55eab-117">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="55eab-117">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="55eab-118">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="55eab-118">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="55eab-119">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55eab-119">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="55eab-120">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="55eab-120">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|<span data-ttu-id="55eab-121">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="55eab-121">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="55eab-122">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55eab-122">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="55eab-123">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="55eab-123">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|<span data-ttu-id="55eab-124">[roleAssignment](../resources/intune-rbac-roleassignment.md);</span><span class="sxs-lookup"><span data-stu-id="55eab-124">[roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|<span data-ttu-id="55eab-125">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55eab-125">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="55eab-126">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="55eab-126">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="55eab-127">Нет</span><span class="sxs-lookup"><span data-stu-id="55eab-127">None</span></span>|<span data-ttu-id="55eab-128">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55eab-128">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="55eab-129">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="55eab-129">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="55eab-130">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="55eab-130">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="55eab-131">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55eab-131">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="55eab-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="55eab-132">Properties</span></span>
|<span data-ttu-id="55eab-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="55eab-133">Property</span></span>|<span data-ttu-id="55eab-134">Тип</span><span class="sxs-lookup"><span data-stu-id="55eab-134">Type</span></span>|<span data-ttu-id="55eab-135">Описание</span><span class="sxs-lookup"><span data-stu-id="55eab-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55eab-136">id</span><span class="sxs-lookup"><span data-stu-id="55eab-136">id</span></span>|<span data-ttu-id="55eab-137">String</span><span class="sxs-lookup"><span data-stu-id="55eab-137">String</span></span>|<span data-ttu-id="55eab-138">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="55eab-138">Key of the entity.</span></span> <span data-ttu-id="55eab-139">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="55eab-139">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="55eab-140">displayName</span><span class="sxs-lookup"><span data-stu-id="55eab-140">displayName</span></span>|<span data-ttu-id="55eab-141">Строка</span><span class="sxs-lookup"><span data-stu-id="55eab-141">String</span></span>|<span data-ttu-id="55eab-142">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="55eab-142">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="55eab-143">description</span><span class="sxs-lookup"><span data-stu-id="55eab-143">description</span></span>|<span data-ttu-id="55eab-144">String</span><span class="sxs-lookup"><span data-stu-id="55eab-144">String</span></span>|<span data-ttu-id="55eab-145">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="55eab-145">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="55eab-146">скопемемберс</span><span class="sxs-lookup"><span data-stu-id="55eab-146">scopeMembers</span></span>|<span data-ttu-id="55eab-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="55eab-147">String collection</span></span>|<span data-ttu-id="55eab-148">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="55eab-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="55eab-149">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="55eab-149">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="55eab-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="55eab-150">scopeType</span></span>|<span data-ttu-id="55eab-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="55eab-151">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="55eab-152">Задает тип области для назначения роли.</span><span class="sxs-lookup"><span data-stu-id="55eab-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="55eab-153">Тип по умолчанию "Ресаурцескопе" позволяет назначать Ресаурцескопес.</span><span class="sxs-lookup"><span data-stu-id="55eab-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="55eab-154">Для "Аллдевицес", "Алллиценседусерс" и "Аллдевицесандлиценседусерс" свойство Ресаурцескопес должно оставаться пустым.</span><span class="sxs-lookup"><span data-stu-id="55eab-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="55eab-155">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="55eab-155">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="55eab-156">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="55eab-156">resourceScopes</span></span>|<span data-ttu-id="55eab-157">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="55eab-157">String collection</span></span>|<span data-ttu-id="55eab-158">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="55eab-158">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="55eab-159">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="55eab-159">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55eab-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="55eab-160">Relationships</span></span>
|<span data-ttu-id="55eab-161">Отношение</span><span class="sxs-lookup"><span data-stu-id="55eab-161">Relationship</span></span>|<span data-ttu-id="55eab-162">Тип</span><span class="sxs-lookup"><span data-stu-id="55eab-162">Type</span></span>|<span data-ttu-id="55eab-163">Описание</span><span class="sxs-lookup"><span data-stu-id="55eab-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55eab-164">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="55eab-164">roleDefinition</span></span>|[<span data-ttu-id="55eab-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="55eab-165">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="55eab-166">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="55eab-166">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55eab-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55eab-167">JSON Representation</span></span>
<span data-ttu-id="55eab-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55eab-168">Here is a JSON representation of the resource.</span></span>
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



