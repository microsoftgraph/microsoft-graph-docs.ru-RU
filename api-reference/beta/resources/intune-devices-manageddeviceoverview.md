---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aafcb3813dd1a11c05613ac3819a7f5b5d4fdcbc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292984"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="c537b-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c537b-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="c537b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c537b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c537b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c537b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c537b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c537b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c537b-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="c537b-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="c537b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c537b-108">Methods</span></span>
|<span data-ttu-id="c537b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c537b-109">Method</span></span>|<span data-ttu-id="c537b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c537b-110">Return Type</span></span>|<span data-ttu-id="c537b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c537b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c537b-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c537b-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="c537b-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c537b-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="c537b-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="c537b-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="c537b-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c537b-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="c537b-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="c537b-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="c537b-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="c537b-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c537b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c537b-118">Properties</span></span>
|<span data-ttu-id="c537b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c537b-119">Property</span></span>|<span data-ttu-id="c537b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c537b-120">Type</span></span>|<span data-ttu-id="c537b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c537b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c537b-122">id</span><span class="sxs-lookup"><span data-stu-id="c537b-122">id</span></span>|<span data-ttu-id="c537b-123">String</span><span class="sxs-lookup"><span data-stu-id="c537b-123">String</span></span>|<span data-ttu-id="c537b-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="c537b-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="c537b-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c537b-125">enrolledDeviceCount</span></span>|<span data-ttu-id="c537b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c537b-126">Int32</span></span>|<span data-ttu-id="c537b-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="c537b-127">Total enrolled device count.</span></span> <span data-ttu-id="c537b-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="c537b-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="c537b-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="c537b-129">mdmEnrolledCount</span></span>|<span data-ttu-id="c537b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="c537b-130">Int32</span></span>|<span data-ttu-id="c537b-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="c537b-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="c537b-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c537b-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="c537b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c537b-133">Int32</span></span>|<span data-ttu-id="c537b-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="c537b-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="c537b-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="c537b-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="c537b-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="c537b-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="c537b-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="c537b-137">Device operating system summary.</span></span>|
|<span data-ttu-id="c537b-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="c537b-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="c537b-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="c537b-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="c537b-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="c537b-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="c537b-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="c537b-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="c537b-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="c537b-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="c537b-143">Модели и производства меатадата для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="c537b-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="c537b-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c537b-144">lastModifiedDateTime</span></span>|<span data-ttu-id="c537b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c537b-145">DateTimeOffset</span></span>|<span data-ttu-id="c537b-146">Общие сведения о дате и времени последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="c537b-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="c537b-147">Связи</span><span class="sxs-lookup"><span data-stu-id="c537b-147">Relationships</span></span>
<span data-ttu-id="c537b-148">Нет</span><span class="sxs-lookup"><span data-stu-id="c537b-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c537b-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c537b-149">JSON Representation</span></span>
<span data-ttu-id="c537b-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c537b-150">Here is a JSON representation of the resource.</span></span>
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
    "aospUserlessCount": 1024
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




