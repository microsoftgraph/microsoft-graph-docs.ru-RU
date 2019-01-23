---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к настраиваемым, так и ко встроенным ролям.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 11fc37502fa017494ff884cb70f0006277a42600
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415126"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="90121-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-106">roleAssignment resource type</span></span>

> <span data-ttu-id="90121-107">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90121-107">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="90121-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90121-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90121-109">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90121-109">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90121-110">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="90121-110">The Role Assignment resource.</span></span> <span data-ttu-id="90121-111">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="90121-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="90121-112">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="90121-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="90121-113">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="90121-113">This applies to custom and built-in roles.</span></span>

## <a name="methods"></a><span data-ttu-id="90121-114">Методы</span><span class="sxs-lookup"><span data-stu-id="90121-114">Methods</span></span>
|<span data-ttu-id="90121-115">Метод</span><span class="sxs-lookup"><span data-stu-id="90121-115">Method</span></span>|<span data-ttu-id="90121-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90121-116">Return Type</span></span>|<span data-ttu-id="90121-117">Описание</span><span class="sxs-lookup"><span data-stu-id="90121-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90121-118">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="90121-119">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="90121-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="90121-120">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="90121-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="90121-121">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="90121-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="90121-123">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="90121-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="90121-124">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="90121-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="90121-126">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="90121-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="90121-127">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="90121-128">Нет</span><span class="sxs-lookup"><span data-stu-id="90121-128">None</span></span>|<span data-ttu-id="90121-129">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="90121-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="90121-130">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="90121-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="90121-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="90121-132">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="90121-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90121-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="90121-133">Properties</span></span>
|<span data-ttu-id="90121-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="90121-134">Property</span></span>|<span data-ttu-id="90121-135">Тип</span><span class="sxs-lookup"><span data-stu-id="90121-135">Type</span></span>|<span data-ttu-id="90121-136">Описание</span><span class="sxs-lookup"><span data-stu-id="90121-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90121-137">id</span><span class="sxs-lookup"><span data-stu-id="90121-137">id</span></span>|<span data-ttu-id="90121-138">String</span><span class="sxs-lookup"><span data-stu-id="90121-138">String</span></span>|<span data-ttu-id="90121-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90121-139">Key of the entity.</span></span> <span data-ttu-id="90121-140">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="90121-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="90121-141">displayName</span><span class="sxs-lookup"><span data-stu-id="90121-141">displayName</span></span>|<span data-ttu-id="90121-142">String</span><span class="sxs-lookup"><span data-stu-id="90121-142">String</span></span>|<span data-ttu-id="90121-143">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="90121-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="90121-144">description</span><span class="sxs-lookup"><span data-stu-id="90121-144">description</span></span>|<span data-ttu-id="90121-145">String</span><span class="sxs-lookup"><span data-stu-id="90121-145">String</span></span>|<span data-ttu-id="90121-146">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="90121-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="90121-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="90121-147">scopeMembers</span></span>|<span data-ttu-id="90121-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90121-148">String collection</span></span>|<span data-ttu-id="90121-149">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="90121-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="90121-150">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="90121-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="90121-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="90121-151">scopeType</span></span>|<span data-ttu-id="90121-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="90121-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="90121-153">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="90121-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="90121-154">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="90121-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="90121-155">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="90121-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="90121-156">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="90121-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="90121-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="90121-157">resourceScopes</span></span>|<span data-ttu-id="90121-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90121-158">String collection</span></span>|<span data-ttu-id="90121-159">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="90121-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="90121-160">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="90121-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90121-161">Связи</span><span class="sxs-lookup"><span data-stu-id="90121-161">Relationships</span></span>
|<span data-ttu-id="90121-162">Связь</span><span class="sxs-lookup"><span data-stu-id="90121-162">Relationship</span></span>|<span data-ttu-id="90121-163">Тип</span><span class="sxs-lookup"><span data-stu-id="90121-163">Type</span></span>|<span data-ttu-id="90121-164">Описание</span><span class="sxs-lookup"><span data-stu-id="90121-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90121-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="90121-165">roleDefinition</span></span>|[<span data-ttu-id="90121-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="90121-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="90121-167">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="90121-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90121-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90121-168">JSON Representation</span></span>
<span data-ttu-id="90121-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90121-169">Here is a JSON representation of the resource.</span></span>
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




