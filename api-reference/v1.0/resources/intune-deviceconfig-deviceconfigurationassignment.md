---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e75d4f76a37fc6497fe0c796f3cd22ac1eda40d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465736"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="eedd9-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eedd9-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="eedd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eedd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eedd9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eedd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eedd9-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="eedd9-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="eedd9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="eedd9-107">Methods</span></span>
|<span data-ttu-id="eedd9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="eedd9-108">Method</span></span>|<span data-ttu-id="eedd9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eedd9-109">Return Type</span></span>|<span data-ttu-id="eedd9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eedd9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eedd9-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eedd9-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="eedd9-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eedd9-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="eedd9-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eedd9-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="eedd9-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eedd9-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="eedd9-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="eedd9-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="eedd9-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eedd9-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="eedd9-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eedd9-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="eedd9-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="eedd9-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="eedd9-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eedd9-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="eedd9-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eedd9-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="eedd9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="eedd9-121">None</span></span>|<span data-ttu-id="eedd9-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eedd9-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="eedd9-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eedd9-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="eedd9-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="eedd9-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="eedd9-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="eedd9-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eedd9-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="eedd9-126">Properties</span></span>
|<span data-ttu-id="eedd9-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="eedd9-127">Property</span></span>|<span data-ttu-id="eedd9-128">Тип</span><span class="sxs-lookup"><span data-stu-id="eedd9-128">Type</span></span>|<span data-ttu-id="eedd9-129">Описание</span><span class="sxs-lookup"><span data-stu-id="eedd9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eedd9-130">id</span><span class="sxs-lookup"><span data-stu-id="eedd9-130">id</span></span>|<span data-ttu-id="eedd9-131">String</span><span class="sxs-lookup"><span data-stu-id="eedd9-131">String</span></span>|<span data-ttu-id="eedd9-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="eedd9-132">The key of the assignment.</span></span>|
|<span data-ttu-id="eedd9-133">target</span><span class="sxs-lookup"><span data-stu-id="eedd9-133">target</span></span>|[<span data-ttu-id="eedd9-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eedd9-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="eedd9-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="eedd9-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eedd9-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="eedd9-136">Relationships</span></span>
<span data-ttu-id="eedd9-137">Нет</span><span class="sxs-lookup"><span data-stu-id="eedd9-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eedd9-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eedd9-138">JSON Representation</span></span>
<span data-ttu-id="eedd9-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eedd9-139">Here is a JSON representation of the resource.</span></span>
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
  }
}
```







