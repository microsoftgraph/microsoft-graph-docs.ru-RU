---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 882cabab9fdc72c3847d3c29bf022f255c101224
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970460"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="c2b5e-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2b5e-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="c2b5e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b5e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b5e-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c2b5e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c2b5e-107">Methods</span></span>
|<span data-ttu-id="c2b5e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c2b5e-108">Method</span></span>|<span data-ttu-id="c2b5e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c2b5e-109">Return Type</span></span>|<span data-ttu-id="c2b5e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b5e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c2b5e-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2b5e-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="c2b5e-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c2b5e-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c2b5e-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c2b5e-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="c2b5e-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2b5e-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="c2b5e-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="c2b5e-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="c2b5e-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c2b5e-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c2b5e-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2b5e-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="c2b5e-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="c2b5e-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="c2b5e-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c2b5e-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c2b5e-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2b5e-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="c2b5e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c2b5e-121">None</span></span>|<span data-ttu-id="c2b5e-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c2b5e-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="c2b5e-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2b5e-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="c2b5e-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2b5e-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="c2b5e-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c2b5e-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2b5e-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2b5e-126">Properties</span></span>
|<span data-ttu-id="c2b5e-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2b5e-127">Property</span></span>|<span data-ttu-id="c2b5e-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b5e-128">Type</span></span>|<span data-ttu-id="c2b5e-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b5e-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2b5e-130">id</span><span class="sxs-lookup"><span data-stu-id="c2b5e-130">id</span></span>|<span data-ttu-id="c2b5e-131">String</span><span class="sxs-lookup"><span data-stu-id="c2b5e-131">String</span></span>|<span data-ttu-id="c2b5e-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-132">The key of the assignment.</span></span>|
|<span data-ttu-id="c2b5e-133">target</span><span class="sxs-lookup"><span data-stu-id="c2b5e-133">target</span></span>|[<span data-ttu-id="c2b5e-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c2b5e-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c2b5e-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2b5e-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="c2b5e-136">Relationships</span></span>
<span data-ttu-id="c2b5e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="c2b5e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2b5e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2b5e-138">JSON Representation</span></span>
<span data-ttu-id="c2b5e-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2b5e-139">Here is a JSON representation of the resource.</span></span>
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





