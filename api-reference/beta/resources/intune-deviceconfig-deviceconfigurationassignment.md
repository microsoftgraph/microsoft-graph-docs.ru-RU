---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dd2dad2bfb846a876e369a3b8fc1a36c846a8276
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154875"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="480cf-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="480cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="480cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="480cf-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="480cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="480cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="480cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="480cf-107">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="480cf-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="480cf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="480cf-108">Methods</span></span>
|<span data-ttu-id="480cf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="480cf-109">Method</span></span>|<span data-ttu-id="480cf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="480cf-110">Return Type</span></span>|<span data-ttu-id="480cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="480cf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="480cf-112">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="480cf-113">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="480cf-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="480cf-114">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="480cf-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="480cf-115">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="480cf-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="480cf-117">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="480cf-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="480cf-118">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="480cf-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="480cf-120">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="480cf-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="480cf-121">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="480cf-122">Нет</span><span class="sxs-lookup"><span data-stu-id="480cf-122">None</span></span>|<span data-ttu-id="480cf-123">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="480cf-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="480cf-124">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="480cf-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="480cf-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="480cf-126">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="480cf-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="480cf-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="480cf-127">Properties</span></span>
|<span data-ttu-id="480cf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="480cf-128">Property</span></span>|<span data-ttu-id="480cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="480cf-129">Type</span></span>|<span data-ttu-id="480cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="480cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="480cf-131">id</span><span class="sxs-lookup"><span data-stu-id="480cf-131">id</span></span>|<span data-ttu-id="480cf-132">String</span><span class="sxs-lookup"><span data-stu-id="480cf-132">String</span></span>|<span data-ttu-id="480cf-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="480cf-133">The key of the assignment.</span></span>|
|<span data-ttu-id="480cf-134">target</span><span class="sxs-lookup"><span data-stu-id="480cf-134">target</span></span>|[<span data-ttu-id="480cf-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="480cf-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="480cf-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="480cf-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="480cf-137">source</span><span class="sxs-lookup"><span data-stu-id="480cf-137">source</span></span>|[<span data-ttu-id="480cf-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="480cf-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="480cf-139">Источник назначения для конфигурации устройства, прямой или сет политик.</span><span class="sxs-lookup"><span data-stu-id="480cf-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="480cf-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="480cf-140">This property is read-only.</span></span> <span data-ttu-id="480cf-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="480cf-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="480cf-142">sourceId</span><span class="sxs-lookup"><span data-stu-id="480cf-142">sourceId</span></span>|<span data-ttu-id="480cf-143">String</span><span class="sxs-lookup"><span data-stu-id="480cf-143">String</span></span>|<span data-ttu-id="480cf-144">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="480cf-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="480cf-145">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="480cf-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="480cf-146">Связи</span><span class="sxs-lookup"><span data-stu-id="480cf-146">Relationships</span></span>
<span data-ttu-id="480cf-147">Нет</span><span class="sxs-lookup"><span data-stu-id="480cf-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="480cf-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="480cf-148">JSON Representation</span></span>
<span data-ttu-id="480cf-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="480cf-149">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  },
  "source": "String",
  "sourceId": "String"
}
```




