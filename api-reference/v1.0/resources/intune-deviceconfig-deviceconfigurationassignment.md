---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4a527f8b9da9f11d521311c54697fd04c4f019
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940913"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="00477-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="00477-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00477-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00477-105">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="00477-105">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="00477-106">Методы</span><span class="sxs-lookup"><span data-stu-id="00477-106">Methods</span></span>
|<span data-ttu-id="00477-107">Метод</span><span class="sxs-lookup"><span data-stu-id="00477-107">Method</span></span>|<span data-ttu-id="00477-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="00477-108">Return Type</span></span>|<span data-ttu-id="00477-109">Описание</span><span class="sxs-lookup"><span data-stu-id="00477-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="00477-110">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-110">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="00477-111">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="00477-111">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="00477-112">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00477-112">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="00477-113">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-113">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="00477-114">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-114">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="00477-115">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00477-115">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="00477-116">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-116">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="00477-117">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-117">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="00477-118">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00477-118">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="00477-119">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-119">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="00477-120">Нет</span><span class="sxs-lookup"><span data-stu-id="00477-120">None</span></span>|<span data-ttu-id="00477-121">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00477-121">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="00477-122">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-122">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="00477-123">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="00477-123">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="00477-124">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="00477-124">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="00477-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="00477-125">Properties</span></span>
|<span data-ttu-id="00477-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="00477-126">Property</span></span>|<span data-ttu-id="00477-127">Тип</span><span class="sxs-lookup"><span data-stu-id="00477-127">Type</span></span>|<span data-ttu-id="00477-128">Описание</span><span class="sxs-lookup"><span data-stu-id="00477-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00477-129">id</span><span class="sxs-lookup"><span data-stu-id="00477-129">id</span></span>|<span data-ttu-id="00477-130">String</span><span class="sxs-lookup"><span data-stu-id="00477-130">String</span></span>|<span data-ttu-id="00477-131">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="00477-131">The key of the assignment.</span></span>|
|<span data-ttu-id="00477-132">target</span><span class="sxs-lookup"><span data-stu-id="00477-132">target</span></span>|[<span data-ttu-id="00477-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="00477-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="00477-134">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="00477-134">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00477-135">Связи</span><span class="sxs-lookup"><span data-stu-id="00477-135">Relationships</span></span>
<span data-ttu-id="00477-136">Нет</span><span class="sxs-lookup"><span data-stu-id="00477-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00477-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00477-137">JSON Representation</span></span>
<span data-ttu-id="00477-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00477-138">Here is a JSON representation of the resource.</span></span>
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



