---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 582d836ae2b9e701f640026d171046bf962eab92
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124116"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="bba70-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bba70-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="bba70-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bba70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bba70-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bba70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bba70-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bba70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bba70-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="bba70-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="bba70-108">Методы</span><span class="sxs-lookup"><span data-stu-id="bba70-108">Methods</span></span>
|<span data-ttu-id="bba70-109">Метод</span><span class="sxs-lookup"><span data-stu-id="bba70-109">Method</span></span>|<span data-ttu-id="bba70-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bba70-110">Return Type</span></span>|<span data-ttu-id="bba70-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bba70-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bba70-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bba70-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|<span data-ttu-id="bba70-113">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md);</span><span class="sxs-lookup"><span data-stu-id="bba70-113">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)</span></span>|<span data-ttu-id="bba70-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bba70-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="bba70-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bba70-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="bba70-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bba70-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="bba70-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="bba70-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bba70-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="bba70-118">Properties</span></span>
|<span data-ttu-id="bba70-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="bba70-119">Property</span></span>|<span data-ttu-id="bba70-120">Тип</span><span class="sxs-lookup"><span data-stu-id="bba70-120">Type</span></span>|<span data-ttu-id="bba70-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bba70-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba70-122">id</span><span class="sxs-lookup"><span data-stu-id="bba70-122">id</span></span>|<span data-ttu-id="bba70-123">String</span><span class="sxs-lookup"><span data-stu-id="bba70-123">String</span></span>|<span data-ttu-id="bba70-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="bba70-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="bba70-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bba70-125">enrolledDeviceCount</span></span>|<span data-ttu-id="bba70-126">Int32</span><span class="sxs-lookup"><span data-stu-id="bba70-126">Int32</span></span>|<span data-ttu-id="bba70-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="bba70-127">Total enrolled device count.</span></span> <span data-ttu-id="bba70-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="bba70-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="bba70-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="bba70-129">mdmEnrolledCount</span></span>|<span data-ttu-id="bba70-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bba70-130">Int32</span></span>|<span data-ttu-id="bba70-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="bba70-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="bba70-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bba70-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="bba70-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bba70-133">Int32</span></span>|<span data-ttu-id="bba70-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="bba70-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="bba70-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="bba70-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="bba70-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="bba70-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="bba70-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="bba70-137">Device operating system summary.</span></span>|
|<span data-ttu-id="bba70-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="bba70-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="bba70-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="bba70-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="bba70-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="bba70-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="bba70-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="bba70-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="bba70-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="bba70-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="bba70-143">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="bba70-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="bba70-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bba70-144">lastModifiedDateTime</span></span>|<span data-ttu-id="bba70-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bba70-145">DateTimeOffset</span></span>|<span data-ttu-id="bba70-146">Общие сведения о дате и времени последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="bba70-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="bba70-147">Связи</span><span class="sxs-lookup"><span data-stu-id="bba70-147">Relationships</span></span>
<span data-ttu-id="bba70-148">Нет</span><span class="sxs-lookup"><span data-stu-id="bba70-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bba70-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bba70-149">JSON Representation</span></span>
<span data-ttu-id="bba70-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bba70-150">Here is a JSON representation of the resource.</span></span>
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
    "unknownCount": 1024,
    "androidDedicatedCount": 1024,
    "androidDeviceAdminCount": 1024,
    "androidFullyManagedCount": 1024,
    "androidWorkProfileCount": 1024,
    "androidCorporateWorkProfileCount": 1024,
    "configMgrDeviceCount": 1024
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



