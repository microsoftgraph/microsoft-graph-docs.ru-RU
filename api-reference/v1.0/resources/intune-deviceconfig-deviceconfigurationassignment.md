---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1bd93f86fa7284a1ba672de1782983a8da586bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972669"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="d15b3-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="d15b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d15b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d15b3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d15b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d15b3-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="d15b3-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="d15b3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d15b3-107">Methods</span></span>
|<span data-ttu-id="d15b3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d15b3-108">Method</span></span>|<span data-ttu-id="d15b3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d15b3-109">Return Type</span></span>|<span data-ttu-id="d15b3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d15b3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d15b3-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="d15b3-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d15b3-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d15b3-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d15b3-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="d15b3-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="d15b3-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="d15b3-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d15b3-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="d15b3-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="d15b3-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="d15b3-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d15b3-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="d15b3-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="d15b3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d15b3-121">None</span></span>|<span data-ttu-id="d15b3-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d15b3-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="d15b3-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="d15b3-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="d15b3-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="d15b3-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d15b3-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d15b3-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="d15b3-126">Properties</span></span>
|<span data-ttu-id="d15b3-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="d15b3-127">Property</span></span>|<span data-ttu-id="d15b3-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d15b3-128">Type</span></span>|<span data-ttu-id="d15b3-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d15b3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d15b3-130">id</span><span class="sxs-lookup"><span data-stu-id="d15b3-130">id</span></span>|<span data-ttu-id="d15b3-131">String</span><span class="sxs-lookup"><span data-stu-id="d15b3-131">String</span></span>|<span data-ttu-id="d15b3-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="d15b3-132">The key of the assignment.</span></span>|
|<span data-ttu-id="d15b3-133">target</span><span class="sxs-lookup"><span data-stu-id="d15b3-133">target</span></span>|[<span data-ttu-id="d15b3-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d15b3-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d15b3-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="d15b3-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d15b3-136">Связи</span><span class="sxs-lookup"><span data-stu-id="d15b3-136">Relationships</span></span>
<span data-ttu-id="d15b3-137">Нет</span><span class="sxs-lookup"><span data-stu-id="d15b3-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d15b3-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d15b3-138">JSON Representation</span></span>
<span data-ttu-id="d15b3-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d15b3-139">Here is a JSON representation of the resource.</span></span>
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









