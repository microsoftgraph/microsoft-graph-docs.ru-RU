---
title: Тип ресурса deviceConfigurationDeviceStateSummary
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 24da8858e899b8781763cccb22306a6a219848b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820162"
---
# <a name="deviceconfigurationdevicestatesummary-resource-type"></a><span data-ttu-id="a8862-103">Тип ресурса deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a8862-103">deviceConfigurationDeviceStateSummary resource type</span></span>

> <span data-ttu-id="a8862-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a8862-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8862-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a8862-105">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="a8862-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a8862-106">Methods</span></span>
|<span data-ttu-id="a8862-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a8862-107">Method</span></span>|<span data-ttu-id="a8862-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8862-108">Return Type</span></span>|<span data-ttu-id="a8862-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a8862-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8862-110">Получение объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a8862-110">Get deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-get.md)|[<span data-ttu-id="a8862-111">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a8862-111">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="a8862-112">Чтение свойств и связей объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8862-112">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|
|[<span data-ttu-id="a8862-113">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a8862-113">Update deviceConfigurationDeviceStateSummary</span></span>](../api/intune-deviceconfig-deviceconfigurationdevicestatesummary-update.md)|[<span data-ttu-id="a8862-114">deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="a8862-114">deviceConfigurationDeviceStateSummary</span></span>](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md)|<span data-ttu-id="a8862-115">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="a8862-115">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8862-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8862-116">Properties</span></span>
|<span data-ttu-id="a8862-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8862-117">Property</span></span>|<span data-ttu-id="a8862-118">Тип</span><span class="sxs-lookup"><span data-stu-id="a8862-118">Type</span></span>|<span data-ttu-id="a8862-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a8862-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8862-120">id</span><span class="sxs-lookup"><span data-stu-id="a8862-120">id</span></span>|<span data-ttu-id="a8862-121">Строка</span><span class="sxs-lookup"><span data-stu-id="a8862-121">String</span></span>|<span data-ttu-id="a8862-122">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a8862-122">Key of the entity.</span></span>|
|<span data-ttu-id="a8862-123">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8862-123">unknownDeviceCount</span></span>|<span data-ttu-id="a8862-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a8862-124">Int32</span></span>|<span data-ttu-id="a8862-125">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="a8862-125">Number of unknown devices</span></span>|
|<span data-ttu-id="a8862-126">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8862-126">notApplicableDeviceCount</span></span>|<span data-ttu-id="a8862-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a8862-127">Int32</span></span>|<span data-ttu-id="a8862-128">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="a8862-128">Number of not applicable devices</span></span>|
|<span data-ttu-id="a8862-129">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8862-129">compliantDeviceCount</span></span>|<span data-ttu-id="a8862-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a8862-130">Int32</span></span>|<span data-ttu-id="a8862-131">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="a8862-131">Number of compliant devices</span></span>|
|<span data-ttu-id="a8862-132">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8862-132">remediatedDeviceCount</span></span>|<span data-ttu-id="a8862-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a8862-133">Int32</span></span>|<span data-ttu-id="a8862-134">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="a8862-134">Number of remediated devices</span></span>|
|<span data-ttu-id="a8862-135">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8862-135">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a8862-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a8862-136">Int32</span></span>|<span data-ttu-id="a8862-137">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="a8862-137">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="a8862-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8862-138">errorDeviceCount</span></span>|<span data-ttu-id="a8862-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a8862-139">Int32</span></span>|<span data-ttu-id="a8862-140">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="a8862-140">Number of error devices</span></span>|
|<span data-ttu-id="a8862-141">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a8862-141">conflictDeviceCount</span></span>|<span data-ttu-id="a8862-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a8862-142">Int32</span></span>|<span data-ttu-id="a8862-143">Количество конфликтующих устройств</span><span class="sxs-lookup"><span data-stu-id="a8862-143">Number of conflict devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8862-144">Связи</span><span class="sxs-lookup"><span data-stu-id="a8862-144">Relationships</span></span>
<span data-ttu-id="a8862-145">Нет</span><span class="sxs-lookup"><span data-stu-id="a8862-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8862-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8862-146">JSON Representation</span></span>
<span data-ttu-id="a8862-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8862-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



