---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 02f0f159886b652f75ef01d31c731fb1f4424d7e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538786"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="7b6a0-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7b6a0-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="7b6a0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b6a0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b6a0-106">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="7b6a0-106">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="7b6a0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7b6a0-107">Methods</span></span>
|<span data-ttu-id="7b6a0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7b6a0-108">Method</span></span>|<span data-ttu-id="7b6a0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7b6a0-109">Return Type</span></span>|<span data-ttu-id="7b6a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b6a0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7b6a0-111">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7b6a0-111">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|<span data-ttu-id="7b6a0-112">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md);</span><span class="sxs-lookup"><span data-stu-id="7b6a0-112">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md)</span></span>|<span data-ttu-id="7b6a0-113">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7b6a0-113">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="7b6a0-114">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7b6a0-114">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="7b6a0-115">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7b6a0-115">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="7b6a0-116">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="7b6a0-116">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b6a0-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b6a0-117">Properties</span></span>
|<span data-ttu-id="7b6a0-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b6a0-118">Property</span></span>|<span data-ttu-id="7b6a0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7b6a0-119">Type</span></span>|<span data-ttu-id="7b6a0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7b6a0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b6a0-121">id</span><span class="sxs-lookup"><span data-stu-id="7b6a0-121">id</span></span>|<span data-ttu-id="7b6a0-122">String</span><span class="sxs-lookup"><span data-stu-id="7b6a0-122">String</span></span>|<span data-ttu-id="7b6a0-123">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-123">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="7b6a0-124">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b6a0-124">enrolledDeviceCount</span></span>|<span data-ttu-id="7b6a0-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7b6a0-125">Int32</span></span>|<span data-ttu-id="7b6a0-126">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-126">Total enrolled device count.</span></span> <span data-ttu-id="7b6a0-127">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-127">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="7b6a0-128">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="7b6a0-128">mdmEnrolledCount</span></span>|<span data-ttu-id="7b6a0-129">Int32</span><span class="sxs-lookup"><span data-stu-id="7b6a0-129">Int32</span></span>|<span data-ttu-id="7b6a0-130">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-130">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="7b6a0-131">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7b6a0-131">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="7b6a0-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7b6a0-132">Int32</span></span>|<span data-ttu-id="7b6a0-133">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-133">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="7b6a0-134">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7b6a0-134">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="7b6a0-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="7b6a0-135">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="7b6a0-136">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-136">Device operating system summary.</span></span>|
|<span data-ttu-id="7b6a0-137">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7b6a0-137">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="7b6a0-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="7b6a0-138">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="7b6a0-139">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-139">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="7b6a0-140">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="7b6a0-140">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="7b6a0-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="7b6a0-141">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="7b6a0-142">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="7b6a0-142">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="7b6a0-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b6a0-143">lastModifiedDateTime</span></span>|<span data-ttu-id="7b6a0-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7b6a0-144">DateTimeOffset</span></span>|<span data-ttu-id="7b6a0-145">Общие сведения о дате и времени последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="7b6a0-145">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b6a0-146">Связи</span><span class="sxs-lookup"><span data-stu-id="7b6a0-146">Relationships</span></span>
<span data-ttu-id="7b6a0-147">Нет</span><span class="sxs-lookup"><span data-stu-id="7b6a0-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b6a0-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b6a0-148">JSON Representation</span></span>
<span data-ttu-id="7b6a0-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b6a0-149">Here is a JSON representation of the resource.</span></span>
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
    "androidWorkProfileCount": 1024
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



