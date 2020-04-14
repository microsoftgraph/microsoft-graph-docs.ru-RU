---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 03e8d7086a2612428e56e81648d6a76e2d58afb2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443941"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="8373c-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8373c-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="8373c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8373c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8373c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8373c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8373c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8373c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8373c-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="8373c-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="8373c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8373c-108">Methods</span></span>
|<span data-ttu-id="8373c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8373c-109">Method</span></span>|<span data-ttu-id="8373c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8373c-110">Return Type</span></span>|<span data-ttu-id="8373c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8373c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8373c-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8373c-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|<span data-ttu-id="8373c-113">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md);</span><span class="sxs-lookup"><span data-stu-id="8373c-113">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)</span></span>|<span data-ttu-id="8373c-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8373c-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="8373c-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8373c-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="8373c-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8373c-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="8373c-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8373c-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8373c-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="8373c-118">Properties</span></span>
|<span data-ttu-id="8373c-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="8373c-119">Property</span></span>|<span data-ttu-id="8373c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="8373c-120">Type</span></span>|<span data-ttu-id="8373c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8373c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8373c-122">id</span><span class="sxs-lookup"><span data-stu-id="8373c-122">id</span></span>|<span data-ttu-id="8373c-123">String</span><span class="sxs-lookup"><span data-stu-id="8373c-123">String</span></span>|<span data-ttu-id="8373c-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="8373c-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="8373c-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8373c-125">enrolledDeviceCount</span></span>|<span data-ttu-id="8373c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="8373c-126">Int32</span></span>|<span data-ttu-id="8373c-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="8373c-127">Total enrolled device count.</span></span> <span data-ttu-id="8373c-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="8373c-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="8373c-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="8373c-129">mdmEnrolledCount</span></span>|<span data-ttu-id="8373c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8373c-130">Int32</span></span>|<span data-ttu-id="8373c-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="8373c-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="8373c-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8373c-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="8373c-133">Int32</span><span class="sxs-lookup"><span data-stu-id="8373c-133">Int32</span></span>|<span data-ttu-id="8373c-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="8373c-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="8373c-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="8373c-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="8373c-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="8373c-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="8373c-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="8373c-137">Device operating system summary.</span></span>|
|<span data-ttu-id="8373c-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="8373c-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="8373c-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="8373c-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="8373c-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="8373c-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="8373c-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="8373c-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="8373c-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="8373c-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="8373c-143">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="8373c-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="8373c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8373c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="8373c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8373c-145">DateTimeOffset</span></span>|<span data-ttu-id="8373c-146">Общие сведения о дате и времени последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="8373c-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="8373c-147">Связи</span><span class="sxs-lookup"><span data-stu-id="8373c-147">Relationships</span></span>
<span data-ttu-id="8373c-148">Нет</span><span class="sxs-lookup"><span data-stu-id="8373c-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8373c-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8373c-149">JSON Representation</span></span>
<span data-ttu-id="8373c-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8373c-150">Here is a JSON representation of the resource.</span></span>
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



