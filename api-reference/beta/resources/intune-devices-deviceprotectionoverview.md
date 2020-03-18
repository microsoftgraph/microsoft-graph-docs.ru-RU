---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e9bdadb7cef003a8d22653660d516afe8357d59
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784142"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="33675-103">Тип ресурса Девицепротектионовервиев</span><span class="sxs-lookup"><span data-stu-id="33675-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="33675-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33675-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33675-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33675-106">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="33675-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="33675-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="33675-107">Properties</span></span>
|<span data-ttu-id="33675-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="33675-108">Property</span></span>|<span data-ttu-id="33675-109">Тип</span><span class="sxs-lookup"><span data-stu-id="33675-109">Type</span></span>|<span data-ttu-id="33675-110">Описание</span><span class="sxs-lookup"><span data-stu-id="33675-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33675-111">тоталрепортеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="33675-112">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-112">Int32</span></span>|<span data-ttu-id="33675-113">Общее количество устройств.</span><span class="sxs-lookup"><span data-stu-id="33675-113">Total device count.</span></span>|
|<span data-ttu-id="33675-114">инактивесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="33675-115">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-115">Int32</span></span>|<span data-ttu-id="33675-116">Устройство с неактивным числом агентов угроз</span><span class="sxs-lookup"><span data-stu-id="33675-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="33675-117">ункновнстатесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="33675-118">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-118">Int32</span></span>|<span data-ttu-id="33675-119">Устройство с состоянием агента угроз "неизвестное количество".</span><span class="sxs-lookup"><span data-stu-id="33675-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="33675-120">пендингсигнатуреупдатедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="33675-121">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-121">Int32</span></span>|<span data-ttu-id="33675-122">Устройство со старым количеством подписей.</span><span class="sxs-lookup"><span data-stu-id="33675-122">Device with old signature count.</span></span>|
|<span data-ttu-id="33675-123">клеандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-123">cleanDeviceCount</span></span>|<span data-ttu-id="33675-124">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-124">Int32</span></span>|<span data-ttu-id="33675-125">Очистка числа устройств.</span><span class="sxs-lookup"><span data-stu-id="33675-125">Clean device count.</span></span>|
|<span data-ttu-id="33675-126">пендингфуллскандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="33675-127">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-127">Int32</span></span>|<span data-ttu-id="33675-128">Количество устройств, ожидающих полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="33675-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="33675-129">пендингрестартдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="33675-130">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-130">Int32</span></span>|<span data-ttu-id="33675-131">Количество устройств, ожидающих перезапуска.</span><span class="sxs-lookup"><span data-stu-id="33675-131">Pending restart device count.</span></span>|
|<span data-ttu-id="33675-132">пендингмануалстепсдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="33675-133">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-133">Int32</span></span>|<span data-ttu-id="33675-134">Количество устройств, ожидающих действий, выполняемых вручную.</span><span class="sxs-lookup"><span data-stu-id="33675-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="33675-135">пендингоффлинескандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="33675-136">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-136">Int32</span></span>|<span data-ttu-id="33675-137">Количество устройств, ожидающих автономной проверки.</span><span class="sxs-lookup"><span data-stu-id="33675-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="33675-138">критикалфаилуресдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="33675-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="33675-139">Int32</span><span class="sxs-lookup"><span data-stu-id="33675-139">Int32</span></span>|<span data-ttu-id="33675-140">Количество устройств критических сбоев.</span><span class="sxs-lookup"><span data-stu-id="33675-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33675-141">Связи</span><span class="sxs-lookup"><span data-stu-id="33675-141">Relationships</span></span>
<span data-ttu-id="33675-142">Нет</span><span class="sxs-lookup"><span data-stu-id="33675-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33675-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33675-143">JSON Representation</span></span>
<span data-ttu-id="33675-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33675-144">Here is a JSON representation of the resource.</span></span>
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



