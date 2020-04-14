---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e6f949cae0ae293c713ba52480d23c44ea093b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470727"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="f7ab8-103">Тип ресурса Девицепротектионовервиев</span><span class="sxs-lookup"><span data-stu-id="f7ab8-103">deviceProtectionOverview resource type</span></span>

<span data-ttu-id="f7ab8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ab8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7ab8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7ab8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ab8-107">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="f7ab8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7ab8-108">Properties</span></span>
|<span data-ttu-id="f7ab8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7ab8-109">Property</span></span>|<span data-ttu-id="f7ab8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f7ab8-110">Type</span></span>|<span data-ttu-id="f7ab8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f7ab8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ab8-112">тоталрепортеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="f7ab8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-113">Int32</span></span>|<span data-ttu-id="f7ab8-114">Общее количество устройств.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-114">Total device count.</span></span>|
|<span data-ttu-id="f7ab8-115">инактивесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="f7ab8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-116">Int32</span></span>|<span data-ttu-id="f7ab8-117">Устройство с неактивным числом агентов угроз</span><span class="sxs-lookup"><span data-stu-id="f7ab8-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="f7ab8-118">ункновнстатесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="f7ab8-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-119">Int32</span></span>|<span data-ttu-id="f7ab8-120">Устройство с состоянием агента угроз "неизвестное количество".</span><span class="sxs-lookup"><span data-stu-id="f7ab8-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="f7ab8-121">пендингсигнатуреупдатедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="f7ab8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-122">Int32</span></span>|<span data-ttu-id="f7ab8-123">Устройство со старым количеством подписей.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-123">Device with old signature count.</span></span>|
|<span data-ttu-id="f7ab8-124">клеандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-124">cleanDeviceCount</span></span>|<span data-ttu-id="f7ab8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-125">Int32</span></span>|<span data-ttu-id="f7ab8-126">Очистка числа устройств.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-126">Clean device count.</span></span>|
|<span data-ttu-id="f7ab8-127">пендингфуллскандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="f7ab8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-128">Int32</span></span>|<span data-ttu-id="f7ab8-129">Количество устройств, ожидающих полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="f7ab8-130">пендингрестартдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="f7ab8-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-131">Int32</span></span>|<span data-ttu-id="f7ab8-132">Количество устройств, ожидающих перезапуска.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-132">Pending restart device count.</span></span>|
|<span data-ttu-id="f7ab8-133">пендингмануалстепсдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="f7ab8-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-134">Int32</span></span>|<span data-ttu-id="f7ab8-135">Количество устройств, ожидающих действий, выполняемых вручную.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="f7ab8-136">пендингоффлинескандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="f7ab8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-137">Int32</span></span>|<span data-ttu-id="f7ab8-138">Количество устройств, ожидающих автономной проверки.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="f7ab8-139">критикалфаилуресдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="f7ab8-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="f7ab8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f7ab8-140">Int32</span></span>|<span data-ttu-id="f7ab8-141">Количество устройств критических сбоев.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7ab8-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="f7ab8-142">Relationships</span></span>
<span data-ttu-id="f7ab8-143">Нет</span><span class="sxs-lookup"><span data-stu-id="f7ab8-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7ab8-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7ab8-144">JSON Representation</span></span>
<span data-ttu-id="f7ab8-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7ab8-145">Here is a JSON representation of the resource.</span></span>
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



