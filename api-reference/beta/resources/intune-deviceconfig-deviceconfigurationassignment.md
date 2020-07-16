---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40723914ff9b4a7dddd54f3484fedd98ac2569b5
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788075"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="93ed2-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ed2-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="93ed2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93ed2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93ed2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93ed2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93ed2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93ed2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93ed2-107">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="93ed2-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="93ed2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="93ed2-108">Methods</span></span>
|<span data-ttu-id="93ed2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="93ed2-109">Method</span></span>|<span data-ttu-id="93ed2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="93ed2-110">Return Type</span></span>|<span data-ttu-id="93ed2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="93ed2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93ed2-112">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ed2-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="93ed2-113">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="93ed2-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="93ed2-114">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ed2-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="93ed2-115">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ed2-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="93ed2-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="93ed2-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="93ed2-117">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ed2-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="93ed2-118">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ed2-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="93ed2-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="93ed2-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="93ed2-120">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ed2-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="93ed2-121">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ed2-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="93ed2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="93ed2-122">None</span></span>|<span data-ttu-id="93ed2-123">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ed2-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="93ed2-124">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ed2-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="93ed2-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="93ed2-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="93ed2-126">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="93ed2-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="93ed2-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="93ed2-127">Properties</span></span>
|<span data-ttu-id="93ed2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="93ed2-128">Property</span></span>|<span data-ttu-id="93ed2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="93ed2-129">Type</span></span>|<span data-ttu-id="93ed2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="93ed2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ed2-131">id</span><span class="sxs-lookup"><span data-stu-id="93ed2-131">id</span></span>|<span data-ttu-id="93ed2-132">String</span><span class="sxs-lookup"><span data-stu-id="93ed2-132">String</span></span>|<span data-ttu-id="93ed2-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="93ed2-133">The key of the assignment.</span></span>|
|<span data-ttu-id="93ed2-134">target</span><span class="sxs-lookup"><span data-stu-id="93ed2-134">target</span></span>|[<span data-ttu-id="93ed2-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="93ed2-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="93ed2-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="93ed2-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="93ed2-137">source</span><span class="sxs-lookup"><span data-stu-id="93ed2-137">source</span></span>|[<span data-ttu-id="93ed2-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="93ed2-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="93ed2-139">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="93ed2-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="93ed2-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="93ed2-140">This property is read-only.</span></span> <span data-ttu-id="93ed2-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="93ed2-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="93ed2-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="93ed2-142">sourceId</span></span>|<span data-ttu-id="93ed2-143">String</span><span class="sxs-lookup"><span data-stu-id="93ed2-143">String</span></span>|<span data-ttu-id="93ed2-144">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="93ed2-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="93ed2-145">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="93ed2-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93ed2-146">Связи</span><span class="sxs-lookup"><span data-stu-id="93ed2-146">Relationships</span></span>
<span data-ttu-id="93ed2-147">Нет</span><span class="sxs-lookup"><span data-stu-id="93ed2-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93ed2-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93ed2-148">JSON Representation</span></span>
<span data-ttu-id="93ed2-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93ed2-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```



