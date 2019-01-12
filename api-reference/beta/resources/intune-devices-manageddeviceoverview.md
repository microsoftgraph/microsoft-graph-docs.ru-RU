---
title: Тип ресурса managedDeviceOverview
description: Сводные данные для управляемых устройств
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 091871ed88903f4fcb3a3ad8be86e7b997f173b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932518"
---
# <a name="manageddeviceoverview-resource-type"></a><span data-ttu-id="a91d7-103">Тип ресурса managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a91d7-103">managedDeviceOverview resource type</span></span>

> <span data-ttu-id="a91d7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a91d7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a91d7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a91d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a91d7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a91d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a91d7-107">Сводные данные для управляемых устройств</span><span class="sxs-lookup"><span data-stu-id="a91d7-107">Summary data for managed devices</span></span>
## <a name="methods"></a><span data-ttu-id="a91d7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a91d7-108">Methods</span></span>
|<span data-ttu-id="a91d7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a91d7-109">Method</span></span>|<span data-ttu-id="a91d7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a91d7-110">Return Type</span></span>|<span data-ttu-id="a91d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a91d7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a91d7-112">Получение объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a91d7-112">Get managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-get.md)|[<span data-ttu-id="a91d7-113">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a91d7-113">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="a91d7-114">Чтение свойств и связей объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="a91d7-114">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|
|[<span data-ttu-id="a91d7-115">Обновление объекта managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a91d7-115">Update managedDeviceOverview</span></span>](../api/intune-devices-manageddeviceoverview-update.md)|[<span data-ttu-id="a91d7-116">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a91d7-116">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="a91d7-117">Обновление свойств объекта [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="a91d7-117">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a91d7-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a91d7-118">Properties</span></span>
|<span data-ttu-id="a91d7-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a91d7-119">Property</span></span>|<span data-ttu-id="a91d7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a91d7-120">Type</span></span>|<span data-ttu-id="a91d7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a91d7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a91d7-122">id</span><span class="sxs-lookup"><span data-stu-id="a91d7-122">id</span></span>|<span data-ttu-id="a91d7-123">String</span><span class="sxs-lookup"><span data-stu-id="a91d7-123">String</span></span>|<span data-ttu-id="a91d7-124">Уникальный идентификатор сводки.</span><span class="sxs-lookup"><span data-stu-id="a91d7-124">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="a91d7-125">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a91d7-125">enrolledDeviceCount</span></span>|<span data-ttu-id="a91d7-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a91d7-126">Int32</span></span>|<span data-ttu-id="a91d7-127">Общее количество зарегистрированных устройств.</span><span class="sxs-lookup"><span data-stu-id="a91d7-127">Total enrolled device count.</span></span> <span data-ttu-id="a91d7-128">Не включает устройства ПК, которыми управляет агент Intune для ПК.</span><span class="sxs-lookup"><span data-stu-id="a91d7-128">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="a91d7-129">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="a91d7-129">mdmEnrolledCount</span></span>|<span data-ttu-id="a91d7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a91d7-130">Int32</span></span>|<span data-ttu-id="a91d7-131">Количество устройств, зарегистрированных в MDM.</span><span class="sxs-lookup"><span data-stu-id="a91d7-131">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="a91d7-132">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a91d7-132">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="a91d7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a91d7-133">Int32</span></span>|<span data-ttu-id="a91d7-134">Количество устройств, зарегистрированных как в MDM, так и в EAS.</span><span class="sxs-lookup"><span data-stu-id="a91d7-134">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="a91d7-135">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a91d7-135">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="a91d7-136">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a91d7-136">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="a91d7-137">Общие сведения об операционной системе устройства.</span><span class="sxs-lookup"><span data-stu-id="a91d7-137">Device operating system summary.</span></span>|
|<span data-ttu-id="a91d7-138">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="a91d7-138">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="a91d7-139">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="a91d7-139">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="a91d7-140">Распределение состояния доступа к Exchange в Intune.</span><span class="sxs-lookup"><span data-stu-id="a91d7-140">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="a91d7-141">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="a91d7-141">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="a91d7-142">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="a91d7-142">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="a91d7-143">Модели и производители meatadata для управляемых устройств в учетной записи</span><span class="sxs-lookup"><span data-stu-id="a91d7-143">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="a91d7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a91d7-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a91d7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a91d7-145">DateTimeOffset</span></span>|<span data-ttu-id="a91d7-146">Время последнего изменения Обзор устройства</span><span class="sxs-lookup"><span data-stu-id="a91d7-146">Last modified date time of device overview</span></span>|

## <a name="relationships"></a><span data-ttu-id="a91d7-147">Связи</span><span class="sxs-lookup"><span data-stu-id="a91d7-147">Relationships</span></span>
<span data-ttu-id="a91d7-148">Нет</span><span class="sxs-lookup"><span data-stu-id="a91d7-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a91d7-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a91d7-149">JSON Representation</span></span>
<span data-ttu-id="a91d7-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a91d7-150">Here is a JSON representation of the resource.</span></span>
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





