---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: accc6d976db80421cd06fd8071417bf07684a71a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550660"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="7c5a0-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7c5a0-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="7c5a0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c5a0-105">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="7c5a0-105">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="7c5a0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7c5a0-106">Methods</span></span>
|<span data-ttu-id="7c5a0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7c5a0-107">Method</span></span>|<span data-ttu-id="7c5a0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c5a0-108">Return Type</span></span>|<span data-ttu-id="7c5a0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7c5a0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7c5a0-110">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7c5a0-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|<span data-ttu-id="7c5a0-111">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md);</span><span class="sxs-lookup"><span data-stu-id="7c5a0-111">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)</span></span>|<span data-ttu-id="7c5a0-112">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7c5a0-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="7c5a0-113">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7c5a0-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="7c5a0-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7c5a0-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="7c5a0-115">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7c5a0-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c5a0-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c5a0-116">Properties</span></span>
|<span data-ttu-id="7c5a0-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c5a0-117">Property</span></span>|<span data-ttu-id="7c5a0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="7c5a0-118">Type</span></span>|<span data-ttu-id="7c5a0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7c5a0-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c5a0-120">id</span><span class="sxs-lookup"><span data-stu-id="7c5a0-120">id</span></span>|<span data-ttu-id="7c5a0-121">String</span><span class="sxs-lookup"><span data-stu-id="7c5a0-121">String</span></span>|<span data-ttu-id="7c5a0-122">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="7c5a0-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c5a0-123">enrolledDeviceCount</span></span>|<span data-ttu-id="7c5a0-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7c5a0-124">Int32</span></span>|<span data-ttu-id="7c5a0-125">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-125">Total enrolled device count.</span></span> <span data-ttu-id="7c5a0-126">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="7c5a0-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="7c5a0-127">mdmEnrolledCount</span></span>|<span data-ttu-id="7c5a0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7c5a0-128">Int32</span></span>|<span data-ttu-id="7c5a0-129">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="7c5a0-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7c5a0-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="7c5a0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7c5a0-131">Int32</span></span>|<span data-ttu-id="7c5a0-132">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="7c5a0-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7c5a0-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="7c5a0-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7c5a0-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="7c5a0-135">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-135">Device operating system summary.</span></span>|
|<span data-ttu-id="7c5a0-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7c5a0-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="7c5a0-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7c5a0-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="7c5a0-138">Распределение состояния доступа Exchange Access State в Intune</span><span class="sxs-lookup"><span data-stu-id="7c5a0-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c5a0-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="7c5a0-139">Relationships</span></span>
<span data-ttu-id="7c5a0-140">Нет</span><span class="sxs-lookup"><span data-stu-id="7c5a0-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c5a0-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c5a0-141">JSON Representation</span></span>
<span data-ttu-id="7c5a0-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c5a0-142">Here is a JSON representation of the resource.</span></span>
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



