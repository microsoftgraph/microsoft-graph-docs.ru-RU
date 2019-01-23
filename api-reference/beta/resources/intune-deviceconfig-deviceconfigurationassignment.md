---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 115cbd779e53f303bdbf95dc28916879726676ee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402603"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="e4869-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="e4869-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4869-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4869-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4869-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4869-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4869-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4869-107">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="e4869-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="e4869-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e4869-108">Methods</span></span>
|<span data-ttu-id="e4869-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e4869-109">Method</span></span>|<span data-ttu-id="e4869-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4869-110">Return Type</span></span>|<span data-ttu-id="e4869-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e4869-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4869-112">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="e4869-113">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e4869-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="e4869-114">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4869-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="e4869-115">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="e4869-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e4869-117">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4869-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e4869-118">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="e4869-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e4869-120">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4869-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="e4869-121">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="e4869-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e4869-122">None</span></span>|<span data-ttu-id="e4869-123">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4869-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="e4869-124">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="e4869-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e4869-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="e4869-126">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e4869-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4869-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4869-127">Properties</span></span>
|<span data-ttu-id="e4869-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4869-128">Property</span></span>|<span data-ttu-id="e4869-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e4869-129">Type</span></span>|<span data-ttu-id="e4869-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e4869-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4869-131">id</span><span class="sxs-lookup"><span data-stu-id="e4869-131">id</span></span>|<span data-ttu-id="e4869-132">String</span><span class="sxs-lookup"><span data-stu-id="e4869-132">String</span></span>|<span data-ttu-id="e4869-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="e4869-133">The key of the assignment.</span></span>|
|<span data-ttu-id="e4869-134">target</span><span class="sxs-lookup"><span data-stu-id="e4869-134">target</span></span>|[<span data-ttu-id="e4869-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e4869-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e4869-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="e4869-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4869-137">Связи</span><span class="sxs-lookup"><span data-stu-id="e4869-137">Relationships</span></span>
<span data-ttu-id="e4869-138">Нет</span><span class="sxs-lookup"><span data-stu-id="e4869-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4869-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4869-139">JSON Representation</span></span>
<span data-ttu-id="e4869-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4869-140">Here is a JSON representation of the resource.</span></span>
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




