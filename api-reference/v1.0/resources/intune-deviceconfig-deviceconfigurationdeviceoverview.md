---
title: Тип ресурса deviceConfigurationDeviceOverview
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 1936b8256c5755c44e613c1626664cef3f7a0ccc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324432"
---
# <a name="deviceconfigurationdeviceoverview-resource-type"></a><span data-ttu-id="bc842-103">Тип ресурса deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bc842-103">deviceConfigurationDeviceOverview resource type</span></span>

> <span data-ttu-id="bc842-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc842-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc842-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="bc842-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="bc842-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bc842-106">Methods</span></span>
|<span data-ttu-id="bc842-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bc842-107">Method</span></span>|<span data-ttu-id="bc842-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc842-108">Return Type</span></span>|<span data-ttu-id="bc842-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bc842-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc842-110">Получение объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bc842-110">Get deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-get.md)|[<span data-ttu-id="bc842-111">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bc842-111">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="bc842-112">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bc842-112">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="bc842-113">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bc842-113">Update deviceConfigurationDeviceOverview</span></span>](../api/intune-deviceconfig-deviceconfigurationdeviceoverview-update.md)|[<span data-ttu-id="bc842-114">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bc842-114">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="bc842-115">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bc842-115">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc842-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc842-116">Properties</span></span>
|<span data-ttu-id="bc842-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc842-117">Property</span></span>|<span data-ttu-id="bc842-118">Тип</span><span class="sxs-lookup"><span data-stu-id="bc842-118">Type</span></span>|<span data-ttu-id="bc842-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bc842-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc842-120">id</span><span class="sxs-lookup"><span data-stu-id="bc842-120">id</span></span>|<span data-ttu-id="bc842-121">Строка</span><span class="sxs-lookup"><span data-stu-id="bc842-121">String</span></span>|<span data-ttu-id="bc842-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bc842-122">Key of the entity.</span></span>|
|<span data-ttu-id="bc842-123">pendingCount</span><span class="sxs-lookup"><span data-stu-id="bc842-123">pendingCount</span></span>|<span data-ttu-id="bc842-124">Int32</span><span class="sxs-lookup"><span data-stu-id="bc842-124">Int32</span></span>|<span data-ttu-id="bc842-125">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="bc842-125">Number of pending devices</span></span>|
|<span data-ttu-id="bc842-126">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="bc842-126">notApplicableCount</span></span>|<span data-ttu-id="bc842-127">Int32</span><span class="sxs-lookup"><span data-stu-id="bc842-127">Int32</span></span>|<span data-ttu-id="bc842-128">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="bc842-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="bc842-129">successCount</span><span class="sxs-lookup"><span data-stu-id="bc842-129">successCount</span></span>|<span data-ttu-id="bc842-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bc842-130">Int32</span></span>|<span data-ttu-id="bc842-131">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="bc842-131">Number of succeeded devices</span></span>|
|<span data-ttu-id="bc842-132">errorCount</span><span class="sxs-lookup"><span data-stu-id="bc842-132">errorCount</span></span>|<span data-ttu-id="bc842-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bc842-133">Int32</span></span>|<span data-ttu-id="bc842-134">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="bc842-134">Number of error devices</span></span>|
|<span data-ttu-id="bc842-135">failedCount</span><span class="sxs-lookup"><span data-stu-id="bc842-135">failedCount</span></span>|<span data-ttu-id="bc842-136">Int32</span><span class="sxs-lookup"><span data-stu-id="bc842-136">Int32</span></span>|<span data-ttu-id="bc842-137">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="bc842-137">Number of failed devices</span></span>|
|<span data-ttu-id="bc842-138">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bc842-138">lastUpdateDateTime</span></span>|<span data-ttu-id="bc842-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc842-139">DateTimeOffset</span></span>|<span data-ttu-id="bc842-140">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="bc842-140">Last update time</span></span>|
|<span data-ttu-id="bc842-141">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="bc842-141">configurationVersion</span></span>|<span data-ttu-id="bc842-142">Int32</span><span class="sxs-lookup"><span data-stu-id="bc842-142">Int32</span></span>|<span data-ttu-id="bc842-143">Версия политики для этого обзора</span><span class="sxs-lookup"><span data-stu-id="bc842-143">Version of the policy for that overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc842-144">Связи</span><span class="sxs-lookup"><span data-stu-id="bc842-144">Relationships</span></span>
<span data-ttu-id="bc842-145">Нет</span><span class="sxs-lookup"><span data-stu-id="bc842-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc842-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc842-146">JSON Representation</span></span>
<span data-ttu-id="bc842-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc842-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



