---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к настраиваемым, так и ко встроенным ролям.
ms.openlocfilehash: a0c3e1d6a9f9611a67916075cdc6a2f90210d89d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078105"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="31a87-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-106">roleAssignment resource type</span></span>

> <span data-ttu-id="31a87-107">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31a87-107">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31a87-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31a87-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31a87-109">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="31a87-109">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31a87-110">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31a87-110">The Role Assignment resource.</span></span> <span data-ttu-id="31a87-111">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="31a87-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="31a87-112">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="31a87-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="31a87-113">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="31a87-113">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="31a87-114">Методы</span><span class="sxs-lookup"><span data-stu-id="31a87-114">Methods</span></span>
|<span data-ttu-id="31a87-115">Метод</span><span class="sxs-lookup"><span data-stu-id="31a87-115">Method</span></span>|<span data-ttu-id="31a87-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="31a87-116">Return Type</span></span>|<span data-ttu-id="31a87-117">Описание</span><span class="sxs-lookup"><span data-stu-id="31a87-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="31a87-118">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="31a87-119">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="31a87-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="31a87-120">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a87-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="31a87-121">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="31a87-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="31a87-123">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a87-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="31a87-124">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="31a87-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="31a87-126">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a87-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="31a87-127">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="31a87-128">Нет</span><span class="sxs-lookup"><span data-stu-id="31a87-128">None</span></span>|<span data-ttu-id="31a87-129">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a87-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="31a87-130">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="31a87-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="31a87-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="31a87-132">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="31a87-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="31a87-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="31a87-133">Properties</span></span>
|<span data-ttu-id="31a87-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="31a87-134">Property</span></span>|<span data-ttu-id="31a87-135">Тип</span><span class="sxs-lookup"><span data-stu-id="31a87-135">Type</span></span>|<span data-ttu-id="31a87-136">Описание</span><span class="sxs-lookup"><span data-stu-id="31a87-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31a87-137">id</span><span class="sxs-lookup"><span data-stu-id="31a87-137">id</span></span>|<span data-ttu-id="31a87-138">String</span><span class="sxs-lookup"><span data-stu-id="31a87-138">String</span></span>|<span data-ttu-id="31a87-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="31a87-139">Key of the entity.</span></span> <span data-ttu-id="31a87-140">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="31a87-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="31a87-141">displayName</span><span class="sxs-lookup"><span data-stu-id="31a87-141">displayName</span></span>|<span data-ttu-id="31a87-142">String</span><span class="sxs-lookup"><span data-stu-id="31a87-142">String</span></span>|<span data-ttu-id="31a87-143">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31a87-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="31a87-144">описание</span><span class="sxs-lookup"><span data-stu-id="31a87-144">description</span></span>|<span data-ttu-id="31a87-145">String</span><span class="sxs-lookup"><span data-stu-id="31a87-145">String</span></span>|<span data-ttu-id="31a87-146">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="31a87-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="31a87-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="31a87-147">scopeMembers</span></span>|<span data-ttu-id="31a87-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="31a87-148">String collection</span></span>|<span data-ttu-id="31a87-149">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="31a87-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="31a87-150">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31a87-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="31a87-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="31a87-151">scopeType</span></span>|<span data-ttu-id="31a87-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="31a87-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="31a87-153">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="31a87-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="31a87-154">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="31a87-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="31a87-155">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="31a87-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="31a87-156">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="31a87-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="31a87-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="31a87-157">resourceScopes</span></span>|<span data-ttu-id="31a87-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="31a87-158">String collection</span></span>|<span data-ttu-id="31a87-159">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="31a87-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="31a87-160">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31a87-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31a87-161">Связи</span><span class="sxs-lookup"><span data-stu-id="31a87-161">Relationships</span></span>
|<span data-ttu-id="31a87-162">Связь</span><span class="sxs-lookup"><span data-stu-id="31a87-162">Relationship</span></span>|<span data-ttu-id="31a87-163">Тип</span><span class="sxs-lookup"><span data-stu-id="31a87-163">Type</span></span>|<span data-ttu-id="31a87-164">Описание</span><span class="sxs-lookup"><span data-stu-id="31a87-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31a87-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31a87-165">roleDefinition</span></span>|[<span data-ttu-id="31a87-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="31a87-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="31a87-167">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="31a87-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31a87-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31a87-168">JSON Representation</span></span>
<span data-ttu-id="31a87-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31a87-169">Here is a JSON representation of the resource.</span></span>
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





