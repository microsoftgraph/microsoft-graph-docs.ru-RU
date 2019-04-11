---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07a6bda1e62088eabc3450cf2dcefc945f3ca898
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771203"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="b207b-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b207b-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="b207b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b207b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b207b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b207b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b207b-106">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="b207b-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="b207b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b207b-107">Methods</span></span>
|<span data-ttu-id="b207b-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b207b-108">Method</span></span>|<span data-ttu-id="b207b-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b207b-109">Return Type</span></span>|<span data-ttu-id="b207b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b207b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b207b-111">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b207b-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="b207b-112">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b207b-112">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b207b-113">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b207b-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="b207b-114">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b207b-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="b207b-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="b207b-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="b207b-116">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="b207b-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b207b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="b207b-117">Properties</span></span>
|<span data-ttu-id="b207b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="b207b-118">Property</span></span>|<span data-ttu-id="b207b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b207b-119">Type</span></span>|<span data-ttu-id="b207b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b207b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b207b-121">id</span><span class="sxs-lookup"><span data-stu-id="b207b-121">id</span></span>|<span data-ttu-id="b207b-122">String</span><span class="sxs-lookup"><span data-stu-id="b207b-122">String</span></span>|<span data-ttu-id="b207b-123">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="b207b-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="b207b-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b207b-124">enrolledDeviceCount</span></span>|<span data-ttu-id="b207b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="b207b-125">Int32</span></span>|<span data-ttu-id="b207b-126">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="b207b-126">Total enrolled device count.</span></span> <span data-ttu-id="b207b-127">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="b207b-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="b207b-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="b207b-128">mdmEnrolledCount</span></span>|<span data-ttu-id="b207b-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b207b-129">Int32</span></span>|<span data-ttu-id="b207b-130">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="b207b-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="b207b-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b207b-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="b207b-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b207b-132">Int32</span></span>|<span data-ttu-id="b207b-133">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="b207b-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="b207b-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b207b-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="b207b-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="b207b-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="b207b-136">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="b207b-136">Device operating system summary.</span></span>|
|<span data-ttu-id="b207b-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b207b-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="b207b-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="b207b-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="b207b-139">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="b207b-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="b207b-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b207b-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="b207b-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="b207b-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="b207b-142">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="b207b-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="b207b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b207b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b207b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b207b-144">DateTimeOffset</span></span>|<span data-ttu-id="b207b-145">Общие сведения о дате и времени последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="b207b-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="b207b-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="b207b-146">Relationships</span></span>
<span data-ttu-id="b207b-147">Нет</span><span class="sxs-lookup"><span data-stu-id="b207b-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b207b-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b207b-148">JSON Representation</span></span>
<span data-ttu-id="b207b-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b207b-149">Here is a JSON representation of the resource.</span></span>
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





