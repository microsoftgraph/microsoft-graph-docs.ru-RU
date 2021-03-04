---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e519f3fd5653e1e3512da8ee58d369df03cc69c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444191"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="0c769-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0c769-103">managedDeviceOverview resource type</span></span>

<span data-ttu-id="0c769-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c769-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c769-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c769-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c769-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c769-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c769-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="0c769-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="0c769-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0c769-108">Methods</span></span>
|<span data-ttu-id="0c769-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0c769-109">Method</span></span>|<span data-ttu-id="0c769-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c769-110">Return Type</span></span>|<span data-ttu-id="0c769-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c769-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c769-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0c769-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="0c769-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0c769-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="0c769-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0c769-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="0c769-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0c769-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="0c769-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0c769-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="0c769-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="0c769-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c769-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c769-118">Properties</span></span>
|<span data-ttu-id="0c769-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c769-119">Property</span></span>|<span data-ttu-id="0c769-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0c769-120">Type</span></span>|<span data-ttu-id="0c769-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0c769-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c769-122">id</span><span class="sxs-lookup"><span data-stu-id="0c769-122">id</span></span>|<span data-ttu-id="0c769-123">String</span><span class="sxs-lookup"><span data-stu-id="0c769-123">String</span></span>|<span data-ttu-id="0c769-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="0c769-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="0c769-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0c769-125">enrolledDeviceCount</span></span>|<span data-ttu-id="0c769-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0c769-126">Int32</span></span>|<span data-ttu-id="0c769-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="0c769-127">Total enrolled device count.</span></span> <span data-ttu-id="0c769-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="0c769-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="0c769-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="0c769-129">mdmEnrolledCount</span></span>|<span data-ttu-id="0c769-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0c769-130">Int32</span></span>|<span data-ttu-id="0c769-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="0c769-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="0c769-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0c769-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="0c769-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0c769-133">Int32</span></span>|<span data-ttu-id="0c769-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="0c769-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="0c769-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="0c769-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="0c769-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="0c769-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="0c769-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="0c769-137">Device operating system summary.</span></span>|
|<span data-ttu-id="0c769-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="0c769-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="0c769-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="0c769-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="0c769-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="0c769-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="0c769-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="0c769-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="0c769-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="0c769-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="0c769-143">Модели и производство meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="0c769-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="0c769-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c769-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0c769-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c769-145">DateTimeOffset</span></span>|<span data-ttu-id="0c769-146">Последнее измененное время даты обзора устройства</span><span class="sxs-lookup"><span data-stu-id="0c769-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c769-147">Связи</span><span class="sxs-lookup"><span data-stu-id="0c769-147">Relationships</span></span>
<span data-ttu-id="0c769-148">Нет</span><span class="sxs-lookup"><span data-stu-id="0c769-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c769-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c769-149">JSON Representation</span></span>
<span data-ttu-id="0c769-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c769-150">Here is a JSON representation of the resource.</span></span>
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
    "linuxCount": 1024
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




