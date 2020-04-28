---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f644ddeb540deb4a5c89aa62ee49dd56f9c20ac
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469419"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="a7d12-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a7d12-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="a7d12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7d12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7d12-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7d12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7d12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7d12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7d12-107">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="a7d12-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="a7d12-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a7d12-108">Methods</span></span>
|<span data-ttu-id="a7d12-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a7d12-109">Method</span></span>|<span data-ttu-id="a7d12-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a7d12-110">Return Type</span></span>|<span data-ttu-id="a7d12-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d12-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7d12-112">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a7d12-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="a7d12-113">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a7d12-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a7d12-114">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7d12-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="a7d12-115">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a7d12-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="a7d12-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="a7d12-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="a7d12-117">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7d12-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a7d12-118">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a7d12-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="a7d12-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="a7d12-119">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="a7d12-120">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7d12-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="a7d12-121">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a7d12-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="a7d12-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a7d12-122">None</span></span>|<span data-ttu-id="a7d12-123">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7d12-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="a7d12-124">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a7d12-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="a7d12-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="a7d12-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="a7d12-126">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a7d12-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a7d12-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7d12-127">Properties</span></span>
|<span data-ttu-id="a7d12-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7d12-128">Property</span></span>|<span data-ttu-id="a7d12-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a7d12-129">Type</span></span>|<span data-ttu-id="a7d12-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d12-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7d12-131">id</span><span class="sxs-lookup"><span data-stu-id="a7d12-131">id</span></span>|<span data-ttu-id="a7d12-132">String</span><span class="sxs-lookup"><span data-stu-id="a7d12-132">String</span></span>|<span data-ttu-id="a7d12-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="a7d12-133">The key of the assignment.</span></span>|
|<span data-ttu-id="a7d12-134">target</span><span class="sxs-lookup"><span data-stu-id="a7d12-134">target</span></span>|[<span data-ttu-id="a7d12-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a7d12-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a7d12-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="a7d12-136">The assignment target for the device configuration.</span></span>|
|<span data-ttu-id="a7d12-137">source</span><span class="sxs-lookup"><span data-stu-id="a7d12-137">source</span></span>|[<span data-ttu-id="a7d12-138">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="a7d12-138">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="a7d12-139">Источник назначения для конфигурации устройства, Direct или в упаковке/политике.</span><span class="sxs-lookup"><span data-stu-id="a7d12-139">The assignment source for the device configuration, direct or parcel/policySet.</span></span> <span data-ttu-id="a7d12-140">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7d12-140">This property is read-only.</span></span> <span data-ttu-id="a7d12-141">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="a7d12-141">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="a7d12-142">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a7d12-142">sourceId</span></span>|<span data-ttu-id="a7d12-143">String</span><span class="sxs-lookup"><span data-stu-id="a7d12-143">String</span></span>|<span data-ttu-id="a7d12-144">Идентификатор источника назначения.</span><span class="sxs-lookup"><span data-stu-id="a7d12-144">The identifier of the source of the assignment.</span></span> <span data-ttu-id="a7d12-145">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7d12-145">This property is read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7d12-146">Связи</span><span class="sxs-lookup"><span data-stu-id="a7d12-146">Relationships</span></span>
<span data-ttu-id="a7d12-147">Нет</span><span class="sxs-lookup"><span data-stu-id="a7d12-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7d12-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7d12-148">JSON Representation</span></span>
<span data-ttu-id="a7d12-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7d12-149">Here is a JSON representation of the resource.</span></span>
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



