---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: db5cebe36850971c871f673d07f18b8d5121cb1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422238"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="87836-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="87836-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="87836-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="87836-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87836-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87836-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87836-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87836-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87836-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="87836-107">Summary data for managed devices</span></span>

## <a name="methods"></a><span data-ttu-id="87836-108">Методы</span><span class="sxs-lookup"><span data-stu-id="87836-108">Methods</span></span>
|<span data-ttu-id="87836-109">Метод</span><span class="sxs-lookup"><span data-stu-id="87836-109">Method</span></span>|<span data-ttu-id="87836-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="87836-110">Return Type</span></span>|<span data-ttu-id="87836-111">Описание</span><span class="sxs-lookup"><span data-stu-id="87836-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87836-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="87836-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="87836-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="87836-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="87836-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="87836-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="87836-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="87836-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="87836-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="87836-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="87836-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="87836-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87836-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="87836-118">Properties</span></span>
|<span data-ttu-id="87836-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="87836-119">Property</span></span>|<span data-ttu-id="87836-120">Тип</span><span class="sxs-lookup"><span data-stu-id="87836-120">Type</span></span>|<span data-ttu-id="87836-121">Описание</span><span class="sxs-lookup"><span data-stu-id="87836-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87836-122">id</span><span class="sxs-lookup"><span data-stu-id="87836-122">id</span></span>|<span data-ttu-id="87836-123">String</span><span class="sxs-lookup"><span data-stu-id="87836-123">String</span></span>|<span data-ttu-id="87836-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="87836-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="87836-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="87836-125">enrolledDeviceCount</span></span>|<span data-ttu-id="87836-126">Int32</span><span class="sxs-lookup"><span data-stu-id="87836-126">Int32</span></span>|<span data-ttu-id="87836-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="87836-127">Total enrolled device count.</span></span> <span data-ttu-id="87836-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="87836-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="87836-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="87836-129">mdmEnrolledCount</span></span>|<span data-ttu-id="87836-130">Int32</span><span class="sxs-lookup"><span data-stu-id="87836-130">Int32</span></span>|<span data-ttu-id="87836-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="87836-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="87836-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="87836-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="87836-133">Int32</span><span class="sxs-lookup"><span data-stu-id="87836-133">Int32</span></span>|<span data-ttu-id="87836-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="87836-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="87836-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="87836-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="87836-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="87836-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="87836-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="87836-137">Device operating system summary.</span></span>|
|<span data-ttu-id="87836-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="87836-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="87836-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="87836-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="87836-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="87836-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="87836-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="87836-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="87836-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="87836-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="87836-143">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="87836-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="87836-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87836-144">lastModifiedDateTime</span></span>|<span data-ttu-id="87836-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87836-145">DateTimeOffset</span></span>|<span data-ttu-id="87836-146">Время последнего изменения Обзор устройства</span><span class="sxs-lookup"><span data-stu-id="87836-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="87836-147">Отношения</span><span class="sxs-lookup"><span data-stu-id="87836-147">Relationships</span></span>
<span data-ttu-id="87836-148">Нет</span><span class="sxs-lookup"><span data-stu-id="87836-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87836-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87836-149">JSON Representation</span></span>
<span data-ttu-id="87836-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87836-150">Here is a JSON representation of the resource.</span></span>
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




