---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7a5abdd3b5455272de7d1cf73044a1356d728dd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981198"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="21e56-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="21e56-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="21e56-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="21e56-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21e56-105">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="21e56-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="21e56-106">Методы</span><span class="sxs-lookup"><span data-stu-id="21e56-106">Methods</span></span>
|<span data-ttu-id="21e56-107">Метод</span><span class="sxs-lookup"><span data-stu-id="21e56-107">Method</span></span>|<span data-ttu-id="21e56-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="21e56-108">Return Type</span></span>|<span data-ttu-id="21e56-109">Описание</span><span class="sxs-lookup"><span data-stu-id="21e56-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21e56-110">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="21e56-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="21e56-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="21e56-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="21e56-112">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="21e56-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="21e56-113">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="21e56-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="21e56-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="21e56-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="21e56-115">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="21e56-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="21e56-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="21e56-116">Properties</span></span>
|<span data-ttu-id="21e56-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="21e56-117">Property</span></span>|<span data-ttu-id="21e56-118">Тип</span><span class="sxs-lookup"><span data-stu-id="21e56-118">Type</span></span>|<span data-ttu-id="21e56-119">Описание</span><span class="sxs-lookup"><span data-stu-id="21e56-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21e56-120">id</span><span class="sxs-lookup"><span data-stu-id="21e56-120">id</span></span>|<span data-ttu-id="21e56-121">String</span><span class="sxs-lookup"><span data-stu-id="21e56-121">String</span></span>|<span data-ttu-id="21e56-122">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="21e56-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="21e56-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21e56-123">enrolledDeviceCount</span></span>|<span data-ttu-id="21e56-124">Int32</span><span class="sxs-lookup"><span data-stu-id="21e56-124">Int32</span></span>|<span data-ttu-id="21e56-125">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="21e56-125">Total enrolled device count.</span></span> <span data-ttu-id="21e56-126">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="21e56-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="21e56-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="21e56-127">mdmEnrolledCount</span></span>|<span data-ttu-id="21e56-128">Int32</span><span class="sxs-lookup"><span data-stu-id="21e56-128">Int32</span></span>|<span data-ttu-id="21e56-129">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="21e56-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="21e56-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21e56-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="21e56-131">Int32</span><span class="sxs-lookup"><span data-stu-id="21e56-131">Int32</span></span>|<span data-ttu-id="21e56-132">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="21e56-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="21e56-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="21e56-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="21e56-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="21e56-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="21e56-135">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="21e56-135">Device operating system summary.</span></span>|
|<span data-ttu-id="21e56-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="21e56-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="21e56-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="21e56-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="21e56-138">Распределение состояния доступа Exchange Access State в Intune</span><span class="sxs-lookup"><span data-stu-id="21e56-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="21e56-139">Связи</span><span class="sxs-lookup"><span data-stu-id="21e56-139">Relationships</span></span>
<span data-ttu-id="21e56-140">Нет</span><span class="sxs-lookup"><span data-stu-id="21e56-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21e56-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21e56-141">JSON Representation</span></span>
<span data-ttu-id="21e56-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21e56-142">Here is a JSON representation of the resource.</span></span>
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



