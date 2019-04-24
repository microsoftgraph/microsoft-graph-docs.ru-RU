---
title: Тип ресурса Девицепротектионовервиев
description: Сведения об оборудовании для данного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f76918b5a959a6621fb7f5c6480a7a2513afead
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522400"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="cafc6-103">Тип ресурса Девицепротектионовервиев</span><span class="sxs-lookup"><span data-stu-id="cafc6-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="cafc6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cafc6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cafc6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cafc6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cafc6-106">Сведения об оборудовании для данного устройства.</span><span class="sxs-lookup"><span data-stu-id="cafc6-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="cafc6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cafc6-107">Properties</span></span>
|<span data-ttu-id="cafc6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cafc6-108">Property</span></span>|<span data-ttu-id="cafc6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cafc6-109">Type</span></span>|<span data-ttu-id="cafc6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cafc6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cafc6-111">Тоталрепортеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-111">totalReportedDeviceCount</span></span>|<span data-ttu-id="cafc6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-112">Int32</span></span>|<span data-ttu-id="cafc6-113">Общее количество устройств.</span><span class="sxs-lookup"><span data-stu-id="cafc6-113">Total device count.</span></span>|
|<span data-ttu-id="cafc6-114">Инактивесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-114">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="cafc6-115">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-115">Int32</span></span>|<span data-ttu-id="cafc6-116">Устройство с неактивным числом агентов угроз</span><span class="sxs-lookup"><span data-stu-id="cafc6-116">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="cafc6-117">Ункновнстатесреатажентдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-117">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="cafc6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-118">Int32</span></span>|<span data-ttu-id="cafc6-119">Устройство с состоянием агента угроз "неизвестное количество".</span><span class="sxs-lookup"><span data-stu-id="cafc6-119">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="cafc6-120">Пендингсигнатуреупдатедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-120">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="cafc6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-121">Int32</span></span>|<span data-ttu-id="cafc6-122">Устройство со старым количеством подписей.</span><span class="sxs-lookup"><span data-stu-id="cafc6-122">Device with old signature count.</span></span>|
|<span data-ttu-id="cafc6-123">Клеандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-123">cleanDeviceCount</span></span>|<span data-ttu-id="cafc6-124">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-124">Int32</span></span>|<span data-ttu-id="cafc6-125">Очистка числа устройств.</span><span class="sxs-lookup"><span data-stu-id="cafc6-125">Clean device count.</span></span>|
|<span data-ttu-id="cafc6-126">Пендингфуллскандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-126">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="cafc6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-127">Int32</span></span>|<span data-ttu-id="cafc6-128">Количество устройств, ожидающих полного сканирования.</span><span class="sxs-lookup"><span data-stu-id="cafc6-128">Pending full scan device count.</span></span>|
|<span data-ttu-id="cafc6-129">Пендингрестартдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-129">pendingRestartDeviceCount</span></span>|<span data-ttu-id="cafc6-130">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-130">Int32</span></span>|<span data-ttu-id="cafc6-131">Количество устройств, ожидающих перезапуска.</span><span class="sxs-lookup"><span data-stu-id="cafc6-131">Pending restart device count.</span></span>|
|<span data-ttu-id="cafc6-132">Пендингмануалстепсдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-132">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="cafc6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-133">Int32</span></span>|<span data-ttu-id="cafc6-134">Количество устройств, ожидающих действий, выполняемых вручную.</span><span class="sxs-lookup"><span data-stu-id="cafc6-134">Pending manual steps device count.</span></span>|
|<span data-ttu-id="cafc6-135">Пендингоффлинескандевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-135">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="cafc6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-136">Int32</span></span>|<span data-ttu-id="cafc6-137">Количество устройств, ожидающих автономной проверки.</span><span class="sxs-lookup"><span data-stu-id="cafc6-137">Pending offline scan device count.</span></span>|
|<span data-ttu-id="cafc6-138">Критикалфаилуресдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="cafc6-138">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="cafc6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cafc6-139">Int32</span></span>|<span data-ttu-id="cafc6-140">Количество устройств критических сбоев.</span><span class="sxs-lookup"><span data-stu-id="cafc6-140">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cafc6-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="cafc6-141">Relationships</span></span>
<span data-ttu-id="cafc6-142">Нет</span><span class="sxs-lookup"><span data-stu-id="cafc6-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cafc6-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cafc6-143">JSON Representation</span></span>
<span data-ttu-id="cafc6-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cafc6-144">Here is a JSON representation of the resource.</span></span>
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





