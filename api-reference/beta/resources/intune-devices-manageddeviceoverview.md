---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2a0345b19c2c2954b0bce231ca05d1bc2d2adcb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158495"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="fa56a-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa56a-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="fa56a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa56a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa56a-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa56a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa56a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa56a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa56a-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="fa56a-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="fa56a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="fa56a-108">Methods</span></span>
|<span data-ttu-id="fa56a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="fa56a-109">Method</span></span>|<span data-ttu-id="fa56a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fa56a-110">Return Type</span></span>|<span data-ttu-id="fa56a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa56a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fa56a-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa56a-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="fa56a-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa56a-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="fa56a-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="fa56a-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="fa56a-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa56a-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="fa56a-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="fa56a-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="fa56a-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="fa56a-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa56a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa56a-118">Properties</span></span>
|<span data-ttu-id="fa56a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa56a-119">Property</span></span>|<span data-ttu-id="fa56a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fa56a-120">Type</span></span>|<span data-ttu-id="fa56a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fa56a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa56a-122">id</span><span class="sxs-lookup"><span data-stu-id="fa56a-122">id</span></span>|<span data-ttu-id="fa56a-123">String</span><span class="sxs-lookup"><span data-stu-id="fa56a-123">String</span></span>|<span data-ttu-id="fa56a-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="fa56a-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="fa56a-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa56a-125">enrolledDeviceCount</span></span>|<span data-ttu-id="fa56a-126">Int32</span><span class="sxs-lookup"><span data-stu-id="fa56a-126">Int32</span></span>|<span data-ttu-id="fa56a-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="fa56a-127">Total enrolled device count.</span></span> <span data-ttu-id="fa56a-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="fa56a-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="fa56a-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="fa56a-129">mdmEnrolledCount</span></span>|<span data-ttu-id="fa56a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="fa56a-130">Int32</span></span>|<span data-ttu-id="fa56a-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="fa56a-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="fa56a-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="fa56a-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="fa56a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="fa56a-133">Int32</span></span>|<span data-ttu-id="fa56a-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="fa56a-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="fa56a-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="fa56a-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="fa56a-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="fa56a-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="fa56a-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="fa56a-137">Device operating system summary.</span></span>|
|<span data-ttu-id="fa56a-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa56a-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="fa56a-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="fa56a-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="fa56a-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="fa56a-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="fa56a-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="fa56a-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="fa56a-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="fa56a-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="fa56a-143">Модели и производство в учетной записи для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="fa56a-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="fa56a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa56a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="fa56a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa56a-145">DateTimeOffset</span></span>|<span data-ttu-id="fa56a-146">Обзор даты последнего изменения устройства</span><span class="sxs-lookup"><span data-stu-id="fa56a-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa56a-147">Связи</span><span class="sxs-lookup"><span data-stu-id="fa56a-147">Relationships</span></span>
<span data-ttu-id="fa56a-148">Нет</span><span class="sxs-lookup"><span data-stu-id="fa56a-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa56a-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa56a-149">JSON Representation</span></span>
<span data-ttu-id="fa56a-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa56a-150">Here is a JSON representation of the resource.</span></span>
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
    "aospUserAssociatedCount": 1024
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




