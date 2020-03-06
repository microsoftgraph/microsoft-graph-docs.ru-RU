---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 522fbcadd2d8326249600dcf352d8c3dfc54cf8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530783"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="daa81-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="daa81-103">deviceConfigurationAssignment resource type</span></span>

<span data-ttu-id="daa81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daa81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daa81-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daa81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daa81-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="daa81-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="daa81-107">Методы</span><span class="sxs-lookup"><span data-stu-id="daa81-107">Methods</span></span>
|<span data-ttu-id="daa81-108">Метод</span><span class="sxs-lookup"><span data-stu-id="daa81-108">Method</span></span>|<span data-ttu-id="daa81-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="daa81-109">Return Type</span></span>|<span data-ttu-id="daa81-110">Описание</span><span class="sxs-lookup"><span data-stu-id="daa81-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="daa81-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="daa81-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="daa81-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="daa81-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="daa81-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="daa81-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="daa81-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="daa81-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="daa81-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="daa81-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="daa81-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="daa81-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="daa81-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="daa81-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="daa81-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="daa81-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="daa81-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="daa81-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="daa81-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="daa81-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="daa81-121">Нет</span><span class="sxs-lookup"><span data-stu-id="daa81-121">None</span></span>|<span data-ttu-id="daa81-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="daa81-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="daa81-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="daa81-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="daa81-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="daa81-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="daa81-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="daa81-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="daa81-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="daa81-126">Properties</span></span>
|<span data-ttu-id="daa81-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="daa81-127">Property</span></span>|<span data-ttu-id="daa81-128">Тип</span><span class="sxs-lookup"><span data-stu-id="daa81-128">Type</span></span>|<span data-ttu-id="daa81-129">Описание</span><span class="sxs-lookup"><span data-stu-id="daa81-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daa81-130">id</span><span class="sxs-lookup"><span data-stu-id="daa81-130">id</span></span>|<span data-ttu-id="daa81-131">Строка</span><span class="sxs-lookup"><span data-stu-id="daa81-131">String</span></span>|<span data-ttu-id="daa81-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="daa81-132">The key of the assignment.</span></span>|
|<span data-ttu-id="daa81-133">target</span><span class="sxs-lookup"><span data-stu-id="daa81-133">target</span></span>|[<span data-ttu-id="daa81-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="daa81-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="daa81-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="daa81-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daa81-136">Связи</span><span class="sxs-lookup"><span data-stu-id="daa81-136">Relationships</span></span>
<span data-ttu-id="daa81-137">Нет</span><span class="sxs-lookup"><span data-stu-id="daa81-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="daa81-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daa81-138">JSON Representation</span></span>
<span data-ttu-id="daa81-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daa81-139">Here is a JSON representation of the resource.</span></span>
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




