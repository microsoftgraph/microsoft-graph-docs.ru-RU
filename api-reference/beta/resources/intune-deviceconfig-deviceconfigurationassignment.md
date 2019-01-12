---
title: Тип ресурса deviceConfigurationAssignment
description: Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7860a7526fc3b0251f4d9b07974170039d4c3312
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991974"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="05134-103">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="05134-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05134-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05134-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05134-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05134-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05134-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05134-107">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="05134-107">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="05134-108">Методы</span><span class="sxs-lookup"><span data-stu-id="05134-108">Methods</span></span>
|<span data-ttu-id="05134-109">Метод</span><span class="sxs-lookup"><span data-stu-id="05134-109">Method</span></span>|<span data-ttu-id="05134-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05134-110">Return Type</span></span>|<span data-ttu-id="05134-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05134-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05134-112">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-112">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="05134-113">Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="05134-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="05134-114">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="05134-114">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="05134-115">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-115">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="05134-116">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-116">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="05134-117">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="05134-117">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="05134-118">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-118">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="05134-119">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-119">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="05134-120">Создание объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="05134-120">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="05134-121">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-121">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="05134-122">Нет</span><span class="sxs-lookup"><span data-stu-id="05134-122">None</span></span>|<span data-ttu-id="05134-123">Удаляет объект [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="05134-123">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="05134-124">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-124">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="05134-125">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="05134-125">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="05134-126">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="05134-126">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="05134-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="05134-127">Properties</span></span>
|<span data-ttu-id="05134-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="05134-128">Property</span></span>|<span data-ttu-id="05134-129">Тип</span><span class="sxs-lookup"><span data-stu-id="05134-129">Type</span></span>|<span data-ttu-id="05134-130">Описание</span><span class="sxs-lookup"><span data-stu-id="05134-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05134-131">id</span><span class="sxs-lookup"><span data-stu-id="05134-131">id</span></span>|<span data-ttu-id="05134-132">String</span><span class="sxs-lookup"><span data-stu-id="05134-132">String</span></span>|<span data-ttu-id="05134-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="05134-133">The key of the assignment.</span></span>|
|<span data-ttu-id="05134-134">target</span><span class="sxs-lookup"><span data-stu-id="05134-134">target</span></span>|[<span data-ttu-id="05134-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="05134-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="05134-136">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="05134-136">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05134-137">Связи</span><span class="sxs-lookup"><span data-stu-id="05134-137">Relationships</span></span>
<span data-ttu-id="05134-138">Нет</span><span class="sxs-lookup"><span data-stu-id="05134-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05134-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05134-139">JSON Representation</span></span>
<span data-ttu-id="05134-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05134-140">Here is a JSON representation of the resource.</span></span>
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





