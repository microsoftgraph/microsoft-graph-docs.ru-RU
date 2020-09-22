---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 686482077d201f952d73af46519650122d60e8b9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091126"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="b912b-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b912b-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="b912b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b912b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b912b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b912b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b912b-106">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="b912b-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="b912b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b912b-107">Methods</span></span>
|<span data-ttu-id="b912b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b912b-108">Method</span></span>|<span data-ttu-id="b912b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b912b-109">Return Type</span></span>|<span data-ttu-id="b912b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b912b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b912b-111">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b912b-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="b912b-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b912b-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b912b-113">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b912b-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b912b-114">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b912b-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="b912b-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b912b-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b912b-116">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b912b-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b912b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="b912b-117">Properties</span></span>
|<span data-ttu-id="b912b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="b912b-118">Property</span></span>|<span data-ttu-id="b912b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b912b-119">Type</span></span>|<span data-ttu-id="b912b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b912b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b912b-121">id</span><span class="sxs-lookup"><span data-stu-id="b912b-121">id</span></span>|<span data-ttu-id="b912b-122">Строка</span><span class="sxs-lookup"><span data-stu-id="b912b-122">String</span></span>|<span data-ttu-id="b912b-123">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="b912b-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="b912b-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b912b-124">enrolledDeviceCount</span></span>|<span data-ttu-id="b912b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b912b-125">Int32</span></span>|<span data-ttu-id="b912b-126">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="b912b-126">Total enrolled device count.</span></span> <span data-ttu-id="b912b-127">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="b912b-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="b912b-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="b912b-128">mdmEnrolledCount</span></span>|<span data-ttu-id="b912b-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b912b-129">Int32</span></span>|<span data-ttu-id="b912b-130">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="b912b-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="b912b-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b912b-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="b912b-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b912b-132">Int32</span></span>|<span data-ttu-id="b912b-133">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="b912b-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="b912b-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b912b-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="b912b-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b912b-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="b912b-136">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="b912b-136">Device operating system summary.</span></span>|
|<span data-ttu-id="b912b-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b912b-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="b912b-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b912b-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="b912b-139">Распределение состояния доступа Exchange Access State в Intune</span><span class="sxs-lookup"><span data-stu-id="b912b-139">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="b912b-140">Связи</span><span class="sxs-lookup"><span data-stu-id="b912b-140">Relationships</span></span>
<span data-ttu-id="b912b-141">Нет</span><span class="sxs-lookup"><span data-stu-id="b912b-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b912b-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b912b-142">JSON Representation</span></span>
<span data-ttu-id="b912b-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b912b-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "String (identifier)",
  "enrolledDeviceCount": 1024,
  "mdmEnrolledCount": 1024,
  "dualEnrolledDeviceCount": 1024,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 1024,
    "iosCount": 1024,
    "macOSCount": 1024,
    "windowsMobileCount": 1024,
    "windowsCount": 1024,
    "unknownCount": 1024
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 1024,
    "blockedDeviceCount": 1024,
    "quarantinedDeviceCount": 1024,
    "unknownDeviceCount": 1024,
    "unavailableDeviceCount": 1024
  }
}
```









