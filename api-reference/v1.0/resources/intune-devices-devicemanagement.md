---
title: Тип ресурса deviceManagement
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bff42d331ac2fe67bdca2193a4ab8ad230b36113
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755437"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="ff2c4-103">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ff2c4-103">deviceManagement resource type</span></span>

<span data-ttu-id="ff2c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff2c4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff2c4-106">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="ff2c4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ff2c4-107">Methods</span></span>
|<span data-ttu-id="ff2c4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ff2c4-108">Method</span></span>|<span data-ttu-id="ff2c4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff2c4-109">Return Type</span></span>|<span data-ttu-id="ff2c4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2c4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff2c4-111">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ff2c4-111">Get deviceManagement</span></span>](../api/intune-devices-devicemanagement-get.md)|[<span data-ttu-id="ff2c4-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ff2c4-112">deviceManagement</span></span>](../resources/intune-devices-devicemanagement.md)|<span data-ttu-id="ff2c4-113">Чтение свойств и связей объекта [deviceManagement](../resources/intune-devices-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ff2c4-113">Read properties and relationships of the [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="ff2c4-114">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ff2c4-114">Update deviceManagement</span></span>](../api/intune-devices-devicemanagement-update.md)|[<span data-ttu-id="ff2c4-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="ff2c4-115">deviceManagement</span></span>](../resources/intune-devices-devicemanagement.md)|<span data-ttu-id="ff2c4-116">Обновление свойств объекта [deviceManagement](../resources/intune-devices-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ff2c4-116">Update the properties of a [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff2c4-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff2c4-117">Properties</span></span>
|<span data-ttu-id="ff2c4-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff2c4-118">Property</span></span>|<span data-ttu-id="ff2c4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ff2c4-119">Type</span></span>|<span data-ttu-id="ff2c4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2c4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2c4-121">id</span><span class="sxs-lookup"><span data-stu-id="ff2c4-121">id</span></span>|<span data-ttu-id="ff2c4-122">String</span><span class="sxs-lookup"><span data-stu-id="ff2c4-122">String</span></span>|<span data-ttu-id="ff2c4-123">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-123">Unique Identifier for the device</span></span>|
|<span data-ttu-id="ff2c4-124">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="ff2c4-124">subscriptionState</span></span>|[<span data-ttu-id="ff2c4-125">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="ff2c4-125">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="ff2c4-126">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-126">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="ff2c4-127">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-127">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff2c4-128">Связи</span><span class="sxs-lookup"><span data-stu-id="ff2c4-128">Relationships</span></span>
|<span data-ttu-id="ff2c4-129">Связь</span><span class="sxs-lookup"><span data-stu-id="ff2c4-129">Relationship</span></span>|<span data-ttu-id="ff2c4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ff2c4-130">Type</span></span>|<span data-ttu-id="ff2c4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2c4-132">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ff2c4-132">applePushNotificationCertificate</span></span>|[<span data-ttu-id="ff2c4-133">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ff2c4-133">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="ff2c4-134">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="ff2c4-134">Apple push notification certificate.</span></span>|
|<span data-ttu-id="ff2c4-135">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff2c4-135">managedDeviceOverview</span></span>|[<span data-ttu-id="ff2c4-136">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ff2c4-136">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="ff2c4-137">Обзор устройств</span><span class="sxs-lookup"><span data-stu-id="ff2c4-137">Device overview</span></span>|
|<span data-ttu-id="ff2c4-138">detectedApps</span><span class="sxs-lookup"><span data-stu-id="ff2c4-138">detectedApps</span></span>|<span data-ttu-id="ff2c4-139">Коллекция [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c4-139">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="ff2c4-140">Список обнаруженных приложений, связанных с устройством.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-140">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="ff2c4-141">managedDevices</span><span class="sxs-lookup"><span data-stu-id="ff2c4-141">managedDevices</span></span>|<span data-ttu-id="ff2c4-142">Коллекция [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c4-142">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="ff2c4-143">Список управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-143">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff2c4-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff2c4-144">JSON Representation</span></span>
<span data-ttu-id="ff2c4-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff2c4-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```




