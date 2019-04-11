---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69c7fc6dc2a4a3ff90e14d430fba9b564930e0a7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774724"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="f7beb-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="f7beb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7beb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7beb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7beb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7beb-106">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="f7beb-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="f7beb-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f7beb-107">Methods</span></span>
|<span data-ttu-id="f7beb-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f7beb-108">Method</span></span>|<span data-ttu-id="f7beb-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7beb-109">Return Type</span></span>|<span data-ttu-id="f7beb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f7beb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f7beb-111">Перечисление объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="f7beb-112">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f7beb-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f7beb-113">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f7beb-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="f7beb-114">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="f7beb-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="f7beb-116">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f7beb-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="f7beb-117">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="f7beb-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="f7beb-119">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f7beb-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="f7beb-120">Delete deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="f7beb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f7beb-121">None</span></span>|<span data-ttu-id="f7beb-122">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f7beb-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="f7beb-123">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="f7beb-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f7beb-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="f7beb-125">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f7beb-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7beb-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7beb-126">Properties</span></span>
|<span data-ttu-id="f7beb-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7beb-127">Property</span></span>|<span data-ttu-id="f7beb-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f7beb-128">Type</span></span>|<span data-ttu-id="f7beb-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f7beb-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7beb-130">id</span><span class="sxs-lookup"><span data-stu-id="f7beb-130">id</span></span>|<span data-ttu-id="f7beb-131">String</span><span class="sxs-lookup"><span data-stu-id="f7beb-131">String</span></span>|<span data-ttu-id="f7beb-132">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="f7beb-132">The key of the assignment.</span></span>|
|<span data-ttu-id="f7beb-133">target</span><span class="sxs-lookup"><span data-stu-id="f7beb-133">target</span></span>|[<span data-ttu-id="f7beb-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f7beb-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f7beb-135">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="f7beb-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7beb-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="f7beb-136">Relationships</span></span>
<span data-ttu-id="f7beb-137">Нет</span><span class="sxs-lookup"><span data-stu-id="f7beb-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7beb-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7beb-138">JSON Representation</span></span>
<span data-ttu-id="f7beb-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7beb-139">Here is a JSON representation of the resource.</span></span>
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





