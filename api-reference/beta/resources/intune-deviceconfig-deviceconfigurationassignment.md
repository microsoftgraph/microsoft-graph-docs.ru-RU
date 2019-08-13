---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ba4aae7fb8706996e0d80d3c3a227b99233b792d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333039"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="4d62a-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4d62a-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="4d62a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4d62a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d62a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4d62a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d62a-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="4d62a-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="4d62a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4d62a-107">Methods</span></span>
|<span data-ttu-id="4d62a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4d62a-108">Method</span></span>|<span data-ttu-id="4d62a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4d62a-109">Return Type</span></span>|<span data-ttu-id="4d62a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4d62a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4d62a-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4d62a-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="4d62a-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4d62a-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4d62a-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4d62a-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="4d62a-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4d62a-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="4d62a-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="4d62a-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="4d62a-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4d62a-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4d62a-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4d62a-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="4d62a-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="4d62a-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="4d62a-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4d62a-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="4d62a-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4d62a-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="4d62a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4d62a-121">None</span></span>|<span data-ttu-id="4d62a-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4d62a-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="4d62a-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4d62a-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="4d62a-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4d62a-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="4d62a-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4d62a-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4d62a-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d62a-126">Properties</span></span>
|<span data-ttu-id="4d62a-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d62a-127">Property</span></span>|<span data-ttu-id="4d62a-128">Тип</span><span class="sxs-lookup"><span data-stu-id="4d62a-128">Type</span></span>|<span data-ttu-id="4d62a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4d62a-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d62a-130">id</span><span class="sxs-lookup"><span data-stu-id="4d62a-130">id</span></span>|<span data-ttu-id="4d62a-131">String</span><span class="sxs-lookup"><span data-stu-id="4d62a-131">String</span></span>|<span data-ttu-id="4d62a-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="4d62a-132">The key of the assignment.</span></span>|
|<span data-ttu-id="4d62a-133">target</span><span class="sxs-lookup"><span data-stu-id="4d62a-133">target</span></span>|[<span data-ttu-id="4d62a-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4d62a-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4d62a-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="4d62a-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d62a-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="4d62a-136">Relationships</span></span>
<span data-ttu-id="4d62a-137">Нет</span><span class="sxs-lookup"><span data-stu-id="4d62a-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d62a-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4d62a-138">JSON Representation</span></span>
<span data-ttu-id="4d62a-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d62a-139">Here is a JSON representation of the resource.</span></span>
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



