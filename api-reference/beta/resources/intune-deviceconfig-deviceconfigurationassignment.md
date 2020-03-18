---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f86b85cd63c619e5ee5447e3f19a66f2a6524767
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793284"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="2d65e-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2d65e-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="2d65e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d65e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d65e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d65e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d65e-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="2d65e-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="2d65e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2d65e-107">Methods</span></span>
|<span data-ttu-id="2d65e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2d65e-108">Method</span></span>|<span data-ttu-id="2d65e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2d65e-109">Return Type</span></span>|<span data-ttu-id="2d65e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d65e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d65e-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2d65e-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="2d65e-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2d65e-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2d65e-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2d65e-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="2d65e-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2d65e-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="2d65e-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="2d65e-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="2d65e-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2d65e-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2d65e-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2d65e-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="2d65e-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="2d65e-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="2d65e-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2d65e-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2d65e-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2d65e-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="2d65e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2d65e-121">None</span></span>|<span data-ttu-id="2d65e-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2d65e-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="2d65e-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2d65e-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="2d65e-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2d65e-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="2d65e-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2d65e-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d65e-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d65e-126">Properties</span></span>
|<span data-ttu-id="2d65e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d65e-127">Property</span></span>|<span data-ttu-id="2d65e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="2d65e-128">Type</span></span>|<span data-ttu-id="2d65e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2d65e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d65e-130">id</span><span class="sxs-lookup"><span data-stu-id="2d65e-130">id</span></span>|<span data-ttu-id="2d65e-131">String</span><span class="sxs-lookup"><span data-stu-id="2d65e-131">String</span></span>|<span data-ttu-id="2d65e-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="2d65e-132">The key of the assignment.</span></span>|
|<span data-ttu-id="2d65e-133">target</span><span class="sxs-lookup"><span data-stu-id="2d65e-133">target</span></span>|[<span data-ttu-id="2d65e-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2d65e-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2d65e-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="2d65e-135">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="2d65e-136">source</span><span class="sxs-lookup"><span data-stu-id="2d65e-136">source</span></span>|[<span data-ttu-id="2d65e-137">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="2d65e-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="2d65e-138">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="2d65e-138">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="2d65e-139">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d65e-139">This property is read-only.</span></span> <span data-ttu-id="2d65e-140">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="2d65e-140">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="2d65e-141">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2d65e-141">sourceId</span></span>|<span data-ttu-id="2d65e-142">String</span><span class="sxs-lookup"><span data-stu-id="2d65e-142">String</span></span>|<span data-ttu-id="2d65e-143">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="2d65e-143">The identifier of the source of the assignment.</span></span> <span data-ttu-id="2d65e-144">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2d65e-144">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d65e-145">Связи</span><span class="sxs-lookup"><span data-stu-id="2d65e-145">Relationships</span></span>
<span data-ttu-id="2d65e-146">Нет</span><span class="sxs-lookup"><span data-stu-id="2d65e-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d65e-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d65e-147">JSON Representation</span></span>
<span data-ttu-id="2d65e-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d65e-148">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



