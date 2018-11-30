---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
ms.openlocfilehash: 0d99d16b8f6ca8f71e419f39f473571d80703dc1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027019"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="9fa23-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9fa23-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="9fa23-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9fa23-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fa23-105">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="9fa23-105">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="9fa23-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9fa23-106">Methods</span></span>
|<span data-ttu-id="9fa23-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9fa23-107">Method</span></span>|<span data-ttu-id="9fa23-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9fa23-108">Return Type</span></span>|<span data-ttu-id="9fa23-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9fa23-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9fa23-110">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9fa23-110">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="9fa23-111">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9fa23-111">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="9fa23-112">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9fa23-112">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="9fa23-113">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9fa23-113">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="9fa23-114">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="9fa23-114">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="9fa23-115">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="9fa23-115">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9fa23-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fa23-116">Properties</span></span>
|<span data-ttu-id="9fa23-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fa23-117">Property</span></span>|<span data-ttu-id="9fa23-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9fa23-118">Type</span></span>|<span data-ttu-id="9fa23-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9fa23-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fa23-120">id</span><span class="sxs-lookup"><span data-stu-id="9fa23-120">id</span></span>|<span data-ttu-id="9fa23-121">String</span><span class="sxs-lookup"><span data-stu-id="9fa23-121">String</span></span>|<span data-ttu-id="9fa23-122">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="9fa23-122">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="9fa23-123">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fa23-123">enrolledDeviceCount</span></span>|<span data-ttu-id="9fa23-124">Int32</span><span class="sxs-lookup"><span data-stu-id="9fa23-124">Int32</span></span>|<span data-ttu-id="9fa23-125">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="9fa23-125">Total enrolled device count.</span></span> <span data-ttu-id="9fa23-126">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="9fa23-126">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="9fa23-127">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="9fa23-127">mdmEnrolledCount</span></span>|<span data-ttu-id="9fa23-128">Int32</span><span class="sxs-lookup"><span data-stu-id="9fa23-128">Int32</span></span>|<span data-ttu-id="9fa23-129">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="9fa23-129">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="9fa23-130">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9fa23-130">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="9fa23-131">Int32</span><span class="sxs-lookup"><span data-stu-id="9fa23-131">Int32</span></span>|<span data-ttu-id="9fa23-132">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="9fa23-132">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="9fa23-133">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9fa23-133">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="9fa23-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="9fa23-134">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="9fa23-135">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="9fa23-135">Device operating system summary.</span></span>|
|<span data-ttu-id="9fa23-136">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="9fa23-136">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="9fa23-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="9fa23-137">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="9fa23-138">Распределение состояния доступа Exchange Access State в Intune</span><span class="sxs-lookup"><span data-stu-id="9fa23-138">Distribution of Exchange Access State in Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fa23-139">Связи</span><span class="sxs-lookup"><span data-stu-id="9fa23-139">Relationships</span></span>
<span data-ttu-id="9fa23-140">Нет</span><span class="sxs-lookup"><span data-stu-id="9fa23-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9fa23-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fa23-141">JSON Representation</span></span>
<span data-ttu-id="9fa23-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fa23-142">Here is a JSON representation of the resource.</span></span>
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



