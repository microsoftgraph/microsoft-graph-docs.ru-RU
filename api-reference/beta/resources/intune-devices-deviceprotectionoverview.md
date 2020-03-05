---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fcdcbe69c1c5d94a00ec50e7e7b29b11a471441f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528596"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="c0546-103">Тип ресурса Девицепротектионовервиев</span><span class="sxs-lookup"><span data-stu-id="c0546-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="c0546-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c0546-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0546-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0546-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0546-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0546-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0546-107">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="c0546-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="c0546-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0546-108">Properties</span></span>
|<span data-ttu-id="c0546-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0546-109">Property</span></span>|<span data-ttu-id="c0546-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c0546-110">Type</span></span>|<span data-ttu-id="c0546-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c0546-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0546-112">тоталрепортеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="c0546-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-113">Int32</span></span>|<span data-ttu-id="c0546-114">Общее количество устройств.</span><span class="sxs-lookup"><span data-stu-id="c0546-114">Total device count.</span></span>|
|<span data-ttu-id="c0546-115">инактивесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="c0546-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-116">Int32</span></span>|<span data-ttu-id="c0546-117">Устройство с неактивным числом агентов угроз</span><span class="sxs-lookup"><span data-stu-id="c0546-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="c0546-118">ункновнстатесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="c0546-119">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-119">Int32</span></span>|<span data-ttu-id="c0546-120">Устройство с состоянием агента угроз "неизвестное количество".</span><span class="sxs-lookup"><span data-stu-id="c0546-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="c0546-121">пендингсигнатуреупдатедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="c0546-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-122">Int32</span></span>|<span data-ttu-id="c0546-123">Устройство со старым количеством подписей.</span><span class="sxs-lookup"><span data-stu-id="c0546-123">Device with old signature count.</span></span>|
|<span data-ttu-id="c0546-124">клеандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-124">cleanDeviceCount</span></span>|<span data-ttu-id="c0546-125">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-125">Int32</span></span>|<span data-ttu-id="c0546-126">Очистка числа устройств.</span><span class="sxs-lookup"><span data-stu-id="c0546-126">Clean device count.</span></span>|
|<span data-ttu-id="c0546-127">пендингфуллскандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="c0546-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-128">Int32</span></span>|<span data-ttu-id="c0546-129">Количество устройств, ожидающих полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="c0546-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="c0546-130">пендингрестартдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="c0546-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-131">Int32</span></span>|<span data-ttu-id="c0546-132">Количество устройств, ожидающих перезапуска.</span><span class="sxs-lookup"><span data-stu-id="c0546-132">Pending restart device count.</span></span>|
|<span data-ttu-id="c0546-133">пендингмануалстепсдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="c0546-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-134">Int32</span></span>|<span data-ttu-id="c0546-135">Количество устройств, ожидающих действий, выполняемых вручную.</span><span class="sxs-lookup"><span data-stu-id="c0546-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="c0546-136">пендингоффлинескандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="c0546-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-137">Int32</span></span>|<span data-ttu-id="c0546-138">Количество устройств, ожидающих автономной проверки.</span><span class="sxs-lookup"><span data-stu-id="c0546-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="c0546-139">критикалфаилуресдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c0546-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="c0546-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c0546-140">Int32</span></span>|<span data-ttu-id="c0546-141">Количество устройств критических сбоев.</span><span class="sxs-lookup"><span data-stu-id="c0546-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0546-142">Связи</span><span class="sxs-lookup"><span data-stu-id="c0546-142">Relationships</span></span>
<span data-ttu-id="c0546-143">Нет</span><span class="sxs-lookup"><span data-stu-id="c0546-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0546-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0546-144">JSON Representation</span></span>
<span data-ttu-id="c0546-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0546-145">Here is a JSON representation of the resource.</span></span>
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



