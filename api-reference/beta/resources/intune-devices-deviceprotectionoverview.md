---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86f941be55d2871f22900c69ec7f1c209df6737d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942026"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="a7edd-103">Тип ресурса Девицепротектионовервиев</span><span class="sxs-lookup"><span data-stu-id="a7edd-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="a7edd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7edd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7edd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7edd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7edd-106">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="a7edd-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="a7edd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7edd-107">Properties</span></span>
|<span data-ttu-id="a7edd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7edd-108">Property</span></span>|<span data-ttu-id="a7edd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a7edd-109">Type</span></span>|<span data-ttu-id="a7edd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a7edd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7edd-111">Тоталрепортеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="a7edd-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-112">Int32</span></span>|<span data-ttu-id="a7edd-113">Общее количество устройств.</span><span class="sxs-lookup"><span data-stu-id="a7edd-113">Total device count.</span></span>|
|<span data-ttu-id="a7edd-114">Инактивесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="a7edd-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-115">Int32</span></span>|<span data-ttu-id="a7edd-116">Устройство с неактивным числом агентов угроз</span><span class="sxs-lookup"><span data-stu-id="a7edd-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="a7edd-117">Ункновнстатесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="a7edd-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-118">Int32</span></span>|<span data-ttu-id="a7edd-119">Устройство с состоянием агента угроз "неизвестное количество".</span><span class="sxs-lookup"><span data-stu-id="a7edd-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="a7edd-120">Пендингсигнатуреупдатедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="a7edd-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-121">Int32</span></span>|<span data-ttu-id="a7edd-122">Устройство со старым количеством подписей.</span><span class="sxs-lookup"><span data-stu-id="a7edd-122">Device with old signature count.</span></span>|
|<span data-ttu-id="a7edd-123">Клеандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-123">cleanDeviceCount</span></span>|<span data-ttu-id="a7edd-124">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-124">Int32</span></span>|<span data-ttu-id="a7edd-125">Очистка числа устройств.</span><span class="sxs-lookup"><span data-stu-id="a7edd-125">Clean device count.</span></span>|
|<span data-ttu-id="a7edd-126">Пендингфуллскандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="a7edd-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-127">Int32</span></span>|<span data-ttu-id="a7edd-128">Количество устройств, ожидающих полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="a7edd-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="a7edd-129">Пендингрестартдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="a7edd-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-130">Int32</span></span>|<span data-ttu-id="a7edd-131">Количество устройств, ожидающих перезапуска.</span><span class="sxs-lookup"><span data-stu-id="a7edd-131">Pending restart device count.</span></span>|
|<span data-ttu-id="a7edd-132">Пендингмануалстепсдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="a7edd-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-133">Int32</span></span>|<span data-ttu-id="a7edd-134">Количество устройств, ожидающих действий, выполняемых вручную.</span><span class="sxs-lookup"><span data-stu-id="a7edd-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="a7edd-135">Пендингоффлинескандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="a7edd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-136">Int32</span></span>|<span data-ttu-id="a7edd-137">Количество устройств, ожидающих автономной проверки.</span><span class="sxs-lookup"><span data-stu-id="a7edd-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="a7edd-138">Критикалфаилуресдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="a7edd-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="a7edd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a7edd-139">Int32</span></span>|<span data-ttu-id="a7edd-140">Количество устройств критических сбоев.</span><span class="sxs-lookup"><span data-stu-id="a7edd-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7edd-141">Связи</span><span class="sxs-lookup"><span data-stu-id="a7edd-141">Relationships</span></span>
<span data-ttu-id="a7edd-142">Нет</span><span class="sxs-lookup"><span data-stu-id="a7edd-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7edd-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7edd-143">JSON Representation</span></span>
<span data-ttu-id="a7edd-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7edd-144">Here is a JSON representation of the resource.</span></span>
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




