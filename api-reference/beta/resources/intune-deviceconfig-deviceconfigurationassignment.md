---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 91181a787be06613302e618301ee8b8075bf41b6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725892"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="e6a45-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="e6a45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6a45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6a45-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6a45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6a45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6a45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6a45-107">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="e6a45-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="e6a45-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e6a45-108">Methods</span></span>
|<span data-ttu-id="e6a45-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e6a45-109">Method</span></span>|<span data-ttu-id="e6a45-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6a45-110">Return Type</span></span>|<span data-ttu-id="e6a45-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e6a45-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6a45-112">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="e6a45-113">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e6a45-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e6a45-114">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e6a45-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="e6a45-115">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="e6a45-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e6a45-117">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e6a45-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e6a45-118">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="e6a45-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e6a45-120">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e6a45-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e6a45-121">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="e6a45-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e6a45-122">None</span></span>|<span data-ttu-id="e6a45-123">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e6a45-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="e6a45-124">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="e6a45-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e6a45-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e6a45-126">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e6a45-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6a45-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6a45-127">Properties</span></span>
|<span data-ttu-id="e6a45-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6a45-128">Property</span></span>|<span data-ttu-id="e6a45-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e6a45-129">Type</span></span>|<span data-ttu-id="e6a45-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e6a45-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6a45-131">id</span><span class="sxs-lookup"><span data-stu-id="e6a45-131">id</span></span>|<span data-ttu-id="e6a45-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e6a45-132">String</span></span>|<span data-ttu-id="e6a45-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="e6a45-133">The key of the assignment.</span></span>|
|<span data-ttu-id="e6a45-134">target</span><span class="sxs-lookup"><span data-stu-id="e6a45-134">target</span></span>|[<span data-ttu-id="e6a45-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e6a45-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e6a45-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="e6a45-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="e6a45-137">source</span><span class="sxs-lookup"><span data-stu-id="e6a45-137">source</span></span>|[<span data-ttu-id="e6a45-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="e6a45-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="e6a45-139">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="e6a45-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="e6a45-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6a45-140">This property is read-only.</span></span> <span data-ttu-id="e6a45-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="e6a45-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="e6a45-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="e6a45-142">sourceId</span></span>|<span data-ttu-id="e6a45-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e6a45-143">String</span></span>|<span data-ttu-id="e6a45-144">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="e6a45-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="e6a45-145">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6a45-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6a45-146">Связи</span><span class="sxs-lookup"><span data-stu-id="e6a45-146">Relationships</span></span>
<span data-ttu-id="e6a45-147">Нет</span><span class="sxs-lookup"><span data-stu-id="e6a45-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6a45-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6a45-148">JSON Representation</span></span>
<span data-ttu-id="e6a45-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6a45-149">Here is a JSON representation of the resource.</span></span>
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





