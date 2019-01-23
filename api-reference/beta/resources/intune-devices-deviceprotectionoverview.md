---
title: Тип ресурса deviceProtectionOverview
description: Сведения об оборудовании данного устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418990"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="21d66-103">Тип ресурса deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="21d66-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="21d66-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21d66-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21d66-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21d66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21d66-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21d66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d66-107">Сведения об оборудовании данного устройства.</span><span class="sxs-lookup"><span data-stu-id="21d66-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="21d66-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21d66-108">Properties</span></span>
|<span data-ttu-id="21d66-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21d66-109">Property</span></span>|<span data-ttu-id="21d66-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21d66-110">Type</span></span>|<span data-ttu-id="21d66-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21d66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d66-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="21d66-113">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-113">Int32</span></span>|<span data-ttu-id="21d66-114">Счетчик общее устройства.</span><span class="sxs-lookup"><span data-stu-id="21d66-114">Total device count.</span></span>|
|<span data-ttu-id="21d66-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="21d66-116">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-116">Int32</span></span>|<span data-ttu-id="21d66-117">Устройства со счетчиком агента неактивных угроз</span><span class="sxs-lookup"><span data-stu-id="21d66-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="21d66-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="21d66-119">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-119">Int32</span></span>|<span data-ttu-id="21d66-120">Устройство с состоянием агента угроз, как число неизвестно.</span><span class="sxs-lookup"><span data-stu-id="21d66-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="21d66-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="21d66-122">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-122">Int32</span></span>|<span data-ttu-id="21d66-123">Устройство со старой счетчиком подписи.</span><span class="sxs-lookup"><span data-stu-id="21d66-123">Device with old signature count.</span></span>|
|<span data-ttu-id="21d66-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-124">cleanDeviceCount</span></span>|<span data-ttu-id="21d66-125">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-125">Int32</span></span>|<span data-ttu-id="21d66-126">Счетчик чистой устройства.</span><span class="sxs-lookup"><span data-stu-id="21d66-126">Clean device count.</span></span>|
|<span data-ttu-id="21d66-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="21d66-128">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-128">Int32</span></span>|<span data-ttu-id="21d66-129">Счетчик устройства ожидающие полную проверку.</span><span class="sxs-lookup"><span data-stu-id="21d66-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="21d66-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="21d66-131">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-131">Int32</span></span>|<span data-ttu-id="21d66-132">Счетчик отложенная перезагрузка устройства.</span><span class="sxs-lookup"><span data-stu-id="21d66-132">Pending restart device count.</span></span>|
|<span data-ttu-id="21d66-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="21d66-134">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-134">Int32</span></span>|<span data-ttu-id="21d66-135">Счетчик устройства ожидающие ручные операции.</span><span class="sxs-lookup"><span data-stu-id="21d66-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="21d66-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="21d66-137">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-137">Int32</span></span>|<span data-ttu-id="21d66-138">Число ожидающих автономной проверки устройства.</span><span class="sxs-lookup"><span data-stu-id="21d66-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="21d66-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21d66-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="21d66-140">Int32</span><span class="sxs-lookup"><span data-stu-id="21d66-140">Int32</span></span>|<span data-ttu-id="21d66-141">Счетчик устройства критические ошибки.</span><span class="sxs-lookup"><span data-stu-id="21d66-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21d66-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="21d66-142">Relationships</span></span>
<span data-ttu-id="21d66-143">Нет</span><span class="sxs-lookup"><span data-stu-id="21d66-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21d66-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21d66-144">JSON Representation</span></span>
<span data-ttu-id="21d66-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21d66-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




