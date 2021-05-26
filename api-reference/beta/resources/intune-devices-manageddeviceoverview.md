---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d6ec4b67826e5fab4155abb84f3286e412fbb5c6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662860"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="f67e0-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f67e0-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="f67e0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f67e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f67e0-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f67e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f67e0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f67e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f67e0-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="f67e0-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="f67e0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f67e0-108">Methods</span></span>
|<span data-ttu-id="f67e0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f67e0-109">Method</span></span>|<span data-ttu-id="f67e0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f67e0-110">Return Type</span></span>|<span data-ttu-id="f67e0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f67e0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f67e0-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f67e0-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="f67e0-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f67e0-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="f67e0-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f67e0-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="f67e0-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f67e0-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="f67e0-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f67e0-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="f67e0-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f67e0-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f67e0-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f67e0-118">Properties</span></span>
|<span data-ttu-id="f67e0-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f67e0-119">Property</span></span>|<span data-ttu-id="f67e0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f67e0-120">Type</span></span>|<span data-ttu-id="f67e0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f67e0-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f67e0-122">id</span><span class="sxs-lookup"><span data-stu-id="f67e0-122">id</span></span>|<span data-ttu-id="f67e0-123">Строка</span><span class="sxs-lookup"><span data-stu-id="f67e0-123">String</span></span>|<span data-ttu-id="f67e0-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="f67e0-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="f67e0-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f67e0-125">enrolledDeviceCount</span></span>|<span data-ttu-id="f67e0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="f67e0-126">Int32</span></span>|<span data-ttu-id="f67e0-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="f67e0-127">Total enrolled device count.</span></span> <span data-ttu-id="f67e0-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="f67e0-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="f67e0-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="f67e0-129">mdmEnrolledCount</span></span>|<span data-ttu-id="f67e0-130">Int32</span><span class="sxs-lookup"><span data-stu-id="f67e0-130">Int32</span></span>|<span data-ttu-id="f67e0-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="f67e0-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="f67e0-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f67e0-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="f67e0-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f67e0-133">Int32</span></span>|<span data-ttu-id="f67e0-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="f67e0-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="f67e0-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f67e0-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="f67e0-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="f67e0-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="f67e0-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="f67e0-137">Device operating system summary.</span></span>|
|<span data-ttu-id="f67e0-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f67e0-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="f67e0-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="f67e0-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="f67e0-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="f67e0-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="f67e0-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f67e0-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="f67e0-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="f67e0-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="f67e0-143">Модели и производство meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="f67e0-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="f67e0-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f67e0-144">lastModifiedDateTime</span></span>|<span data-ttu-id="f67e0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f67e0-145">DateTimeOffset</span></span>|<span data-ttu-id="f67e0-146">Последнее измененное время даты обзора устройства</span><span class="sxs-lookup"><span data-stu-id="f67e0-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="f67e0-147">Связи</span><span class="sxs-lookup"><span data-stu-id="f67e0-147">Relationships</span></span>
<span data-ttu-id="f67e0-148">Нет</span><span class="sxs-lookup"><span data-stu-id="f67e0-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f67e0-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f67e0-149">JSON Representation</span></span>
<span data-ttu-id="f67e0-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f67e0-150">Here is a JSON representation of the resource.</span></span>
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
    "configMgrDeviceCount": 1024,
    "aospUserlessCount": 1024,
    "aospUserAssociatedCount": 1024,
    "linuxCount": 1024,
    "chromeOSCount": 1024
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




