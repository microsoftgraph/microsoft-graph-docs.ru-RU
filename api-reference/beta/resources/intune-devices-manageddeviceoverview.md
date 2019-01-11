---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1eeb349e8ec77adce3d69df9d61f43e43fb3b770
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872550"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="b70da-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b70da-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="b70da-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b70da-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b70da-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b70da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b70da-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b70da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b70da-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="b70da-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="b70da-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b70da-108">Methods</span></span>
|<span data-ttu-id="b70da-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b70da-109">Method</span></span>|<span data-ttu-id="b70da-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b70da-110">Return Type</span></span>|<span data-ttu-id="b70da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b70da-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b70da-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b70da-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="b70da-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b70da-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b70da-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b70da-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b70da-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b70da-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="b70da-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b70da-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b70da-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b70da-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b70da-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b70da-118">Properties</span></span>
|<span data-ttu-id="b70da-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="b70da-119">Property</span></span>|<span data-ttu-id="b70da-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b70da-120">Type</span></span>|<span data-ttu-id="b70da-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b70da-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b70da-122">id</span><span class="sxs-lookup"><span data-stu-id="b70da-122">id</span></span>|<span data-ttu-id="b70da-123">String</span><span class="sxs-lookup"><span data-stu-id="b70da-123">String</span></span>|<span data-ttu-id="b70da-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="b70da-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="b70da-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b70da-125">enrolledDeviceCount</span></span>|<span data-ttu-id="b70da-126">Int32</span><span class="sxs-lookup"><span data-stu-id="b70da-126">Int32</span></span>|<span data-ttu-id="b70da-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="b70da-127">Total enrolled device count.</span></span> <span data-ttu-id="b70da-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="b70da-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="b70da-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="b70da-129">mdmEnrolledCount</span></span>|<span data-ttu-id="b70da-130">Int32</span><span class="sxs-lookup"><span data-stu-id="b70da-130">Int32</span></span>|<span data-ttu-id="b70da-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="b70da-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="b70da-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b70da-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="b70da-133">Int32</span><span class="sxs-lookup"><span data-stu-id="b70da-133">Int32</span></span>|<span data-ttu-id="b70da-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="b70da-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="b70da-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b70da-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="b70da-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b70da-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="b70da-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="b70da-137">Device operating system summary.</span></span>|
|<span data-ttu-id="b70da-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b70da-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="b70da-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b70da-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="b70da-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="b70da-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="b70da-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b70da-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="b70da-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b70da-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="b70da-143">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="b70da-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="b70da-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b70da-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b70da-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b70da-145">DateTimeOffset</span></span>|<span data-ttu-id="b70da-146">Время последнего изменения Обзор устройства</span><span class="sxs-lookup"><span data-stu-id="b70da-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="b70da-147">Связи</span><span class="sxs-lookup"><span data-stu-id="b70da-147">Relationships</span></span>
<span data-ttu-id="b70da-148">Нет</span><span class="sxs-lookup"><span data-stu-id="b70da-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b70da-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b70da-149">JSON Representation</span></span>
<span data-ttu-id="b70da-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b70da-150">Here is a JSON representation of the resource.</span></span>
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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "String"
    ],
    "deviceManufacturers": [
      "String"
    ]
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```





