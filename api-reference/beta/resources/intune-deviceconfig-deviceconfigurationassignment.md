---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e344554804044687c7e5b9aa90c6171055b64a16
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37198196"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="92d99-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="92d99-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="92d99-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92d99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92d99-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92d99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92d99-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="92d99-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="92d99-107">Методы</span><span class="sxs-lookup"><span data-stu-id="92d99-107">Methods</span></span>
|<span data-ttu-id="92d99-108">Метод</span><span class="sxs-lookup"><span data-stu-id="92d99-108">Method</span></span>|<span data-ttu-id="92d99-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92d99-109">Return Type</span></span>|<span data-ttu-id="92d99-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92d99-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92d99-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="92d99-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="92d99-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="92d99-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="92d99-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="92d99-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="92d99-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="92d99-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="92d99-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="92d99-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="92d99-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="92d99-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="92d99-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="92d99-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="92d99-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="92d99-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="92d99-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="92d99-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="92d99-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="92d99-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="92d99-121">Нет</span><span class="sxs-lookup"><span data-stu-id="92d99-121">None</span></span>|<span data-ttu-id="92d99-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="92d99-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="92d99-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="92d99-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="92d99-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="92d99-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="92d99-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="92d99-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="92d99-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="92d99-126">Properties</span></span>
|<span data-ttu-id="92d99-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="92d99-127">Property</span></span>|<span data-ttu-id="92d99-128">Тип</span><span class="sxs-lookup"><span data-stu-id="92d99-128">Type</span></span>|<span data-ttu-id="92d99-129">Описание</span><span class="sxs-lookup"><span data-stu-id="92d99-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92d99-130">id</span><span class="sxs-lookup"><span data-stu-id="92d99-130">id</span></span>|<span data-ttu-id="92d99-131">String</span><span class="sxs-lookup"><span data-stu-id="92d99-131">String</span></span>|<span data-ttu-id="92d99-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="92d99-132">The key of the assignment.</span></span>|
|<span data-ttu-id="92d99-133">target</span><span class="sxs-lookup"><span data-stu-id="92d99-133">target</span></span>|[<span data-ttu-id="92d99-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="92d99-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="92d99-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="92d99-135">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="92d99-136">source</span><span class="sxs-lookup"><span data-stu-id="92d99-136">source</span></span>|[<span data-ttu-id="92d99-137">девицеандаппманажементассигнментсаурце</span><span class="sxs-lookup"><span data-stu-id="92d99-137">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="92d99-138">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="92d99-138">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="92d99-139">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="92d99-139">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="92d99-140">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="92d99-140">sourceId</span></span>|<span data-ttu-id="92d99-141">String.</span><span class="sxs-lookup"><span data-stu-id="92d99-141">String</span></span>|<span data-ttu-id="92d99-142">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="92d99-142">The identifier of the source of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92d99-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="92d99-143">Relationships</span></span>
<span data-ttu-id="92d99-144">Нет</span><span class="sxs-lookup"><span data-stu-id="92d99-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92d99-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92d99-145">JSON Representation</span></span>
<span data-ttu-id="92d99-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92d99-146">Here is a JSON representation of the resource.</span></span>
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



