---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8031566663d9113fa40014bdb7bdd7603d3c6174
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842422"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="df98a-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="df98a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="df98a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df98a-105">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="df98a-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="df98a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="df98a-106">Methods</span></span>
|<span data-ttu-id="df98a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="df98a-107">Method</span></span>|<span data-ttu-id="df98a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="df98a-108">Return Type</span></span>|<span data-ttu-id="df98a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="df98a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df98a-110">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="df98a-111">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="df98a-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="df98a-112">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df98a-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="df98a-113">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="df98a-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="df98a-115">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df98a-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="df98a-116">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="df98a-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="df98a-118">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df98a-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="df98a-119">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="df98a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="df98a-120">None</span></span>|<span data-ttu-id="df98a-121">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df98a-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="df98a-122">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="df98a-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="df98a-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="df98a-124">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="df98a-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="df98a-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="df98a-125">Properties</span></span>
|<span data-ttu-id="df98a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="df98a-126">Property</span></span>|<span data-ttu-id="df98a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="df98a-127">Type</span></span>|<span data-ttu-id="df98a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="df98a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df98a-129">id</span><span class="sxs-lookup"><span data-stu-id="df98a-129">id</span></span>|<span data-ttu-id="df98a-130">String</span><span class="sxs-lookup"><span data-stu-id="df98a-130">String</span></span>|<span data-ttu-id="df98a-131">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="df98a-131">The key of the assignment.</span></span>|
|<span data-ttu-id="df98a-132">target</span><span class="sxs-lookup"><span data-stu-id="df98a-132">target</span></span>|[<span data-ttu-id="df98a-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="df98a-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="df98a-134">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="df98a-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df98a-135">Связи</span><span class="sxs-lookup"><span data-stu-id="df98a-135">Relationships</span></span>
<span data-ttu-id="df98a-136">Нет</span><span class="sxs-lookup"><span data-stu-id="df98a-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df98a-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df98a-137">JSON Representation</span></span>
<span data-ttu-id="df98a-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df98a-138">Here is a JSON representation of the resource.</span></span>
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



