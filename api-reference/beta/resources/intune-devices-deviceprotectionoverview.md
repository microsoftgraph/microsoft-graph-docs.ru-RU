---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a815dbd43f8b47f872b51ecb3eee8791b622d505
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691367"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="e277d-103">Тип ресурса Девицепротектионовервиев</span><span class="sxs-lookup"><span data-stu-id="e277d-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="e277d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e277d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e277d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e277d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e277d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e277d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e277d-107">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="e277d-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e277d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e277d-108">Properties</span></span>
|<span data-ttu-id="e277d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e277d-109">Property</span></span>|<span data-ttu-id="e277d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e277d-110">Type</span></span>|<span data-ttu-id="e277d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e277d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e277d-112">тоталрепортеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="e277d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-113">Int32</span></span>|<span data-ttu-id="e277d-114">Общее количество устройств.</span><span class="sxs-lookup"><span data-stu-id="e277d-114">Total device count.</span></span>|
|<span data-ttu-id="e277d-115">инактивесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="e277d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-116">Int32</span></span>|<span data-ttu-id="e277d-117">Устройство с неактивным числом агентов угроз</span><span class="sxs-lookup"><span data-stu-id="e277d-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="e277d-118">ункновнстатесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="e277d-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-119">Int32</span></span>|<span data-ttu-id="e277d-120">Устройство с состоянием агента угроз "неизвестное количество".</span><span class="sxs-lookup"><span data-stu-id="e277d-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="e277d-121">пендингсигнатуреупдатедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="e277d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-122">Int32</span></span>|<span data-ttu-id="e277d-123">Устройство со старым количеством подписей.</span><span class="sxs-lookup"><span data-stu-id="e277d-123">Device with old signature count.</span></span>|
|<span data-ttu-id="e277d-124">клеандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-124">cleanDeviceCount</span></span>|<span data-ttu-id="e277d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-125">Int32</span></span>|<span data-ttu-id="e277d-126">Очистка числа устройств.</span><span class="sxs-lookup"><span data-stu-id="e277d-126">Clean device count.</span></span>|
|<span data-ttu-id="e277d-127">пендингфуллскандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="e277d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-128">Int32</span></span>|<span data-ttu-id="e277d-129">Количество устройств, ожидающих полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="e277d-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="e277d-130">пендингрестартдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="e277d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-131">Int32</span></span>|<span data-ttu-id="e277d-132">Количество устройств, ожидающих перезапуска.</span><span class="sxs-lookup"><span data-stu-id="e277d-132">Pending restart device count.</span></span>|
|<span data-ttu-id="e277d-133">пендингмануалстепсдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="e277d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-134">Int32</span></span>|<span data-ttu-id="e277d-135">Количество устройств, ожидающих действий, выполняемых вручную.</span><span class="sxs-lookup"><span data-stu-id="e277d-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="e277d-136">пендингоффлинескандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="e277d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-137">Int32</span></span>|<span data-ttu-id="e277d-138">Количество устройств, ожидающих автономной проверки.</span><span class="sxs-lookup"><span data-stu-id="e277d-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="e277d-139">критикалфаилуресдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="e277d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-140">Int32</span></span>|<span data-ttu-id="e277d-141">Количество устройств критических сбоев.</span><span class="sxs-lookup"><span data-stu-id="e277d-141">Critical failures device count.</span></span>|
|<span data-ttu-id="e277d-142">пендингкуиккскандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="e277d-142">pendingQuickScanDeviceCount</span></span>|<span data-ttu-id="e277d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e277d-143">Int32</span></span>|<span data-ttu-id="e277d-144">Число ожидающих устройств быстрого сканирования.</span><span class="sxs-lookup"><span data-stu-id="e277d-144">Pending quick scan device count.</span></span> <span data-ttu-id="e277d-145">Допустимые значения: от 2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e277d-145">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="e277d-146">Связи</span><span class="sxs-lookup"><span data-stu-id="e277d-146">Relationships</span></span>
<span data-ttu-id="e277d-147">Нет</span><span class="sxs-lookup"><span data-stu-id="e277d-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e277d-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e277d-148">JSON Representation</span></span>
<span data-ttu-id="e277d-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e277d-149">Here is a JSON representation of the resource.</span></span>
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
  "criticalFailuresDeviceCount": 1024,
  "pendingQuickScanDeviceCount": 1024
}
```





