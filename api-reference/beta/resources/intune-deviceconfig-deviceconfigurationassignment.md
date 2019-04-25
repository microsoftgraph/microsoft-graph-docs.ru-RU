---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69c7fc6dc2a4a3ff90e14d430fba9b564930e0a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567902"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="1ffdc-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1ffdc-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="1ffdc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ffdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ffdc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ffdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ffdc-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="1ffdc-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="1ffdc-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1ffdc-107">Methods</span></span>
|<span data-ttu-id="1ffdc-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1ffdc-108">Method</span></span>|<span data-ttu-id="1ffdc-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1ffdc-109">Return Type</span></span>|<span data-ttu-id="1ffdc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ffdc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1ffdc-111">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1ffdc-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="1ffdc-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1ffdc-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1ffdc-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ffdc-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="1ffdc-114">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1ffdc-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|<span data-ttu-id="1ffdc-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="1ffdc-115">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="1ffdc-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ffdc-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1ffdc-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1ffdc-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|<span data-ttu-id="1ffdc-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md);</span><span class="sxs-lookup"><span data-stu-id="1ffdc-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span></span>|<span data-ttu-id="1ffdc-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ffdc-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="1ffdc-120">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1ffdc-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="1ffdc-121">Нет</span><span class="sxs-lookup"><span data-stu-id="1ffdc-121">None</span></span>|<span data-ttu-id="1ffdc-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ffdc-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="1ffdc-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1ffdc-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="1ffdc-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="1ffdc-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="1ffdc-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1ffdc-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1ffdc-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ffdc-126">Properties</span></span>
|<span data-ttu-id="1ffdc-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ffdc-127">Property</span></span>|<span data-ttu-id="1ffdc-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1ffdc-128">Type</span></span>|<span data-ttu-id="1ffdc-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1ffdc-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ffdc-130">id</span><span class="sxs-lookup"><span data-stu-id="1ffdc-130">id</span></span>|<span data-ttu-id="1ffdc-131">String</span><span class="sxs-lookup"><span data-stu-id="1ffdc-131">String</span></span>|<span data-ttu-id="1ffdc-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="1ffdc-132">The key of the assignment.</span></span>|
|<span data-ttu-id="1ffdc-133">target</span><span class="sxs-lookup"><span data-stu-id="1ffdc-133">target</span></span>|[<span data-ttu-id="1ffdc-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1ffdc-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1ffdc-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="1ffdc-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ffdc-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="1ffdc-136">Relationships</span></span>
<span data-ttu-id="1ffdc-137">Нет</span><span class="sxs-lookup"><span data-stu-id="1ffdc-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ffdc-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ffdc-138">JSON Representation</span></span>
<span data-ttu-id="1ffdc-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ffdc-139">Here is a JSON representation of the resource.</span></span>
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





