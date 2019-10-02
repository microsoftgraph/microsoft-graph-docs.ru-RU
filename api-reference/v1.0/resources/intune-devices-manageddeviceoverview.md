---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a09564d6ec2cb51e561cc1934f99c3d57868fdc
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359798"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="9863f-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9863f-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="9863f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9863f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9863f-105">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="9863f-105">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="9863f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9863f-106">Methods</span></span>
|<span data-ttu-id="9863f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9863f-107">Method</span></span>|<span data-ttu-id="9863f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9863f-108">Return Type</span></span>|<span data-ttu-id="9863f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9863f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9863f-110">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9863f-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|<span data-ttu-id="9863f-111">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md);</span><span class="sxs-lookup"><span data-stu-id="9863f-111">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)</span></span>|<span data-ttu-id="9863f-112">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9863f-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="9863f-113">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9863f-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="9863f-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9863f-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="9863f-115">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9863f-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9863f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9863f-116">Properties</span></span>
|<span data-ttu-id="9863f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9863f-117">Property</span></span>|<span data-ttu-id="9863f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9863f-118">Type</span></span>|<span data-ttu-id="9863f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9863f-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9863f-120">id</span><span class="sxs-lookup"><span data-stu-id="9863f-120">id</span></span>|<span data-ttu-id="9863f-121">String</span><span class="sxs-lookup"><span data-stu-id="9863f-121">String</span></span>|<span data-ttu-id="9863f-122">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="9863f-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="9863f-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9863f-123">enrolledDeviceCount</span></span>|<span data-ttu-id="9863f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="9863f-124">Int32</span></span>|<span data-ttu-id="9863f-125">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="9863f-125">Total enrolled device count.</span></span> <span data-ttu-id="9863f-126">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="9863f-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="9863f-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="9863f-127">mdmEnrolledCount</span></span>|<span data-ttu-id="9863f-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9863f-128">Int32</span></span>|<span data-ttu-id="9863f-129">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="9863f-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="9863f-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9863f-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="9863f-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9863f-131">Int32</span></span>|<span data-ttu-id="9863f-132">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="9863f-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="9863f-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9863f-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="9863f-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9863f-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="9863f-135">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="9863f-135">Device operating system summary.</span></span>|
|<span data-ttu-id="9863f-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="9863f-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="9863f-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="9863f-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="9863f-138">Распределение состояния доступа Exchange Access State в Intune</span><span class="sxs-lookup"><span data-stu-id="9863f-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="9863f-139">Связи</span><span class="sxs-lookup"><span data-stu-id="9863f-139">Relationships</span></span>
<span data-ttu-id="9863f-140">Нет</span><span class="sxs-lookup"><span data-stu-id="9863f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9863f-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9863f-141">JSON Representation</span></span>
<span data-ttu-id="9863f-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9863f-142">Here is a JSON representation of the resource.</span></span>
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




