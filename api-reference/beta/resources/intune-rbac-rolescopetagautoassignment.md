---
title: Тип ресурса Ролескопетагаутоассигнмент
description: Содержит свойства для автоматического назначения тега области роли группе, которая будет применена к устройствам.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a308c91eb2a78c50012c348a19b613335915af47
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369187"
---
# <a name="rolescopetagautoassignment-resource-type"></a><span data-ttu-id="5a638-103">Тип ресурса Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-103">roleScopeTagAutoAssignment resource type</span></span>

> <span data-ttu-id="5a638-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a638-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a638-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5a638-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a638-106">Содержит свойства для автоматического назначения тега области роли группе, которая будет применена к устройствам.</span><span class="sxs-lookup"><span data-stu-id="5a638-106">Contains the properties for auto-assigning a Role Scope Tag to a group to be applied to Devices.</span></span>

## <a name="methods"></a><span data-ttu-id="5a638-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5a638-107">Methods</span></span>
|<span data-ttu-id="5a638-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5a638-108">Method</span></span>|<span data-ttu-id="5a638-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a638-109">Return Type</span></span>|<span data-ttu-id="5a638-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5a638-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a638-111">Список Ролескопетагаутоассигнментс</span><span class="sxs-lookup"><span data-stu-id="5a638-111">List roleScopeTagAutoAssignments</span></span>](../api/intune-rbac-rolescopetagautoassignment-list.md)|<span data-ttu-id="5a638-112">Коллекция [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5a638-112">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="5a638-113">Список свойств и связей объектов [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5a638-113">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>|
|[<span data-ttu-id="5a638-114">Получение Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-114">Get roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-get.md)|[<span data-ttu-id="5a638-115">ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-115">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="5a638-116">Чтение свойств и связей объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5a638-116">Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="5a638-117">Создание Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-117">Create roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-create.md)|[<span data-ttu-id="5a638-118">ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-118">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="5a638-119">Создание нового объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5a638-119">Create a new [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|
|[<span data-ttu-id="5a638-120">Удаление Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-120">Delete roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-delete.md)|<span data-ttu-id="5a638-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5a638-121">None</span></span>|<span data-ttu-id="5a638-122">Удаляет объект [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md).</span><span class="sxs-lookup"><span data-stu-id="5a638-122">Deletes a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md).</span></span>|
|[<span data-ttu-id="5a638-123">Обновление Ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-123">Update roleScopeTagAutoAssignment</span></span>](../api/intune-rbac-rolescopetagautoassignment-update.md)|[<span data-ttu-id="5a638-124">ролескопетагаутоассигнмент</span><span class="sxs-lookup"><span data-stu-id="5a638-124">roleScopeTagAutoAssignment</span></span>](../resources/intune-rbac-rolescopetagautoassignment.md)|<span data-ttu-id="5a638-125">Обновление свойств объекта [ролескопетагаутоассигнмент](../resources/intune-rbac-rolescopetagautoassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5a638-125">Update the properties of a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a638-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a638-126">Properties</span></span>
|<span data-ttu-id="5a638-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a638-127">Property</span></span>|<span data-ttu-id="5a638-128">Тип</span><span class="sxs-lookup"><span data-stu-id="5a638-128">Type</span></span>|<span data-ttu-id="5a638-129">Описание</span><span class="sxs-lookup"><span data-stu-id="5a638-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a638-130">id</span><span class="sxs-lookup"><span data-stu-id="5a638-130">id</span></span>|<span data-ttu-id="5a638-131">String</span><span class="sxs-lookup"><span data-stu-id="5a638-131">String</span></span>|<span data-ttu-id="5a638-132">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5a638-132">Key of the entity.</span></span>|
|<span data-ttu-id="5a638-133">target</span><span class="sxs-lookup"><span data-stu-id="5a638-133">target</span></span>|[<span data-ttu-id="5a638-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5a638-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5a638-135">Целевой объект автоматического назначения для определенного тега области применения роли.</span><span class="sxs-lookup"><span data-stu-id="5a638-135">The auto-assignment target for the specific Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a638-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="5a638-136">Relationships</span></span>
<span data-ttu-id="5a638-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5a638-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a638-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a638-138">JSON Representation</span></span>
<span data-ttu-id="5a638-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a638-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



