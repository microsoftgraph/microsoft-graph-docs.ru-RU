---
title: Тип ресурса roleAssignment
description: Ресурс назначения роли. Назначения ролей объединяют определение роли с участниками и областями. Одной роли может соответствовать одно или несколько назначений. Это относится как к настраиваемым, так и ко встроенным ролям.
author: tfitzmac
ms.openlocfilehash: 5c4b09151a7957f52dbaa525f696b89479a898ef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302102"
---
# <a name="roleassignment-resource-type"></a><span data-ttu-id="d8a7b-106">Тип ресурса roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-106">roleAssignment resource type</span></span>

> <span data-ttu-id="d8a7b-107">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-107">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8a7b-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-108">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8a7b-109">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-109">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8a7b-110">Ресурс назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-110">The Role Assignment resource.</span></span> <span data-ttu-id="d8a7b-111">Назначения ролей объединяют определение роли с участниками и областями.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-111">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="d8a7b-112">Одной роли может соответствовать одно или несколько назначений.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-112">There can be one or more role assignments per role.</span></span> <span data-ttu-id="d8a7b-113">Это относится как к пользовательским, так и ко встроенным ролям.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-113">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="d8a7b-114">Методы</span><span class="sxs-lookup"><span data-stu-id="d8a7b-114">Methods</span></span>
|<span data-ttu-id="d8a7b-115">Метод</span><span class="sxs-lookup"><span data-stu-id="d8a7b-115">Method</span></span>|<span data-ttu-id="d8a7b-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8a7b-116">Return Type</span></span>|<span data-ttu-id="d8a7b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a7b-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8a7b-118">Список объектов roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-118">List roleAssignments</span></span>](../api/intune-rbac-roleassignment-list.md)|<span data-ttu-id="d8a7b-119">Коллекция объектов [roleAssignment](../resources/intune-rbac-roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d8a7b-119">[roleAssignment](../resources/intune-rbac-roleassignment.md) collection</span></span>|<span data-ttu-id="d8a7b-120">Список свойств и связей объектов [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8a7b-120">List properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="d8a7b-121">Получение объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-121">Get roleAssignment</span></span>](../api/intune-rbac-roleassignment-get.md)|[<span data-ttu-id="d8a7b-122">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-122">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="d8a7b-123">Чтение свойств и связей объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8a7b-123">Read properties and relationships of the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="d8a7b-124">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-124">Create roleAssignment</span></span>](../api/intune-rbac-roleassignment-create.md)|[<span data-ttu-id="d8a7b-125">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-125">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="d8a7b-126">Создание объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8a7b-126">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|
|[<span data-ttu-id="d8a7b-127">Удаление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-127">Delete roleAssignment</span></span>](../api/intune-rbac-roleassignment-delete.md)|<span data-ttu-id="d8a7b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d8a7b-128">None</span></span>|<span data-ttu-id="d8a7b-129">Удаляет объект [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8a7b-129">Deletes a [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>|
|[<span data-ttu-id="d8a7b-130">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-130">Update roleAssignment</span></span>](../api/intune-rbac-roleassignment-update.md)|[<span data-ttu-id="d8a7b-131">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="d8a7b-131">roleAssignment</span></span>](../resources/intune-rbac-roleassignment.md)|<span data-ttu-id="d8a7b-132">Обновление свойств объекта [roleAssignment](../resources/intune-rbac-roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d8a7b-132">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8a7b-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8a7b-133">Properties</span></span>
|<span data-ttu-id="d8a7b-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8a7b-134">Property</span></span>|<span data-ttu-id="d8a7b-135">Тип</span><span class="sxs-lookup"><span data-stu-id="d8a7b-135">Type</span></span>|<span data-ttu-id="d8a7b-136">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a7b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8a7b-137">id</span><span class="sxs-lookup"><span data-stu-id="d8a7b-137">id</span></span>|<span data-ttu-id="d8a7b-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d8a7b-138">String</span></span>|<span data-ttu-id="d8a7b-139">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-139">Key of the entity.</span></span> <span data-ttu-id="d8a7b-140">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-140">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="d8a7b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d8a7b-141">displayName</span></span>|<span data-ttu-id="d8a7b-142">String</span><span class="sxs-lookup"><span data-stu-id="d8a7b-142">String</span></span>|<span data-ttu-id="d8a7b-143">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-143">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="d8a7b-144">описание</span><span class="sxs-lookup"><span data-stu-id="d8a7b-144">description</span></span>|<span data-ttu-id="d8a7b-145">String</span><span class="sxs-lookup"><span data-stu-id="d8a7b-145">String</span></span>|<span data-ttu-id="d8a7b-146">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-146">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="d8a7b-147">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="d8a7b-147">scopeMembers</span></span>|<span data-ttu-id="d8a7b-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d8a7b-148">String collection</span></span>|<span data-ttu-id="d8a7b-149">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-149">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d8a7b-150">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-150">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="d8a7b-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="d8a7b-151">scopeType</span></span>|<span data-ttu-id="d8a7b-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md);</span><span class="sxs-lookup"><span data-stu-id="d8a7b-152">[roleAssignmentScopeType](../resources/intune-rbac-roleassignmentscopetype.md)</span></span>|<span data-ttu-id="d8a7b-153">Указывает тип области для назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="d8a7b-154">Тип по умолчанию «ResourceScope» позволяет присваивать ResourceScopes.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="d8a7b-155">Для «AllDevices», «AllLicensedUsers» и «AllDevicesAndLicensedUsers» свойство ResourceScopes должно быть пустым.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="d8a7b-156">Возможные значения: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="d8a7b-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="d8a7b-157">resourceScopes</span></span>|<span data-ttu-id="d8a7b-158">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d8a7b-158">String collection</span></span>|<span data-ttu-id="d8a7b-159">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="d8a7b-160">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-160">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8a7b-161">Связи</span><span class="sxs-lookup"><span data-stu-id="d8a7b-161">Relationships</span></span>
|<span data-ttu-id="d8a7b-162">Связь</span><span class="sxs-lookup"><span data-stu-id="d8a7b-162">Relationship</span></span>|<span data-ttu-id="d8a7b-163">Тип</span><span class="sxs-lookup"><span data-stu-id="d8a7b-163">Type</span></span>|<span data-ttu-id="d8a7b-164">Описание</span><span class="sxs-lookup"><span data-stu-id="d8a7b-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8a7b-165">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d8a7b-165">roleDefinition</span></span>|[<span data-ttu-id="d8a7b-166">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="d8a7b-166">roleDefinition</span></span>](../resources/intune-rbac-roledefinition.md)|<span data-ttu-id="d8a7b-167">Определение роли, частью которого является это назначение.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-167">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8a7b-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8a7b-168">JSON Representation</span></span>
<span data-ttu-id="d8a7b-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8a7b-169">Here is a JSON representation of the resource.</span></span>
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





