---
title: Тип ресурса deviceProtectionOverview
description: Сведения об оборудовании данного устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 12066877e380c022a1cd1ec49322ab51b8e59d65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811531"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="bf38b-103">Тип ресурса deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="bf38b-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="bf38b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf38b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf38b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf38b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf38b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf38b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf38b-107">Сведения об оборудовании данного устройства.</span><span class="sxs-lookup"><span data-stu-id="bf38b-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="bf38b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf38b-108">Properties</span></span>
|<span data-ttu-id="bf38b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf38b-109">Property</span></span>|<span data-ttu-id="bf38b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bf38b-110">Type</span></span>|<span data-ttu-id="bf38b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf38b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf38b-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="bf38b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-113">Int32</span></span>|<span data-ttu-id="bf38b-114">Счетчик общее устройства.</span><span class="sxs-lookup"><span data-stu-id="bf38b-114">Total device count.</span></span>|
|<span data-ttu-id="bf38b-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="bf38b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-116">Int32</span></span>|<span data-ttu-id="bf38b-117">Устройства со счетчиком агента неактивных угроз</span><span class="sxs-lookup"><span data-stu-id="bf38b-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="bf38b-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="bf38b-119">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-119">Int32</span></span>|<span data-ttu-id="bf38b-120">Устройство с состоянием агента угроз, как число неизвестно.</span><span class="sxs-lookup"><span data-stu-id="bf38b-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="bf38b-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="bf38b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-122">Int32</span></span>|<span data-ttu-id="bf38b-123">Устройство со старой счетчиком подписи.</span><span class="sxs-lookup"><span data-stu-id="bf38b-123">Device with old signature count.</span></span>|
|<span data-ttu-id="bf38b-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-124">cleanDeviceCount</span></span>|<span data-ttu-id="bf38b-125">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-125">Int32</span></span>|<span data-ttu-id="bf38b-126">Счетчик чистой устройства.</span><span class="sxs-lookup"><span data-stu-id="bf38b-126">Clean device count.</span></span>|
|<span data-ttu-id="bf38b-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="bf38b-128">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-128">Int32</span></span>|<span data-ttu-id="bf38b-129">Счетчик устройства ожидающие полную проверку.</span><span class="sxs-lookup"><span data-stu-id="bf38b-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="bf38b-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="bf38b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-131">Int32</span></span>|<span data-ttu-id="bf38b-132">Счетчик отложенная перезагрузка устройства.</span><span class="sxs-lookup"><span data-stu-id="bf38b-132">Pending restart device count.</span></span>|
|<span data-ttu-id="bf38b-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="bf38b-134">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-134">Int32</span></span>|<span data-ttu-id="bf38b-135">Счетчик устройства ожидающие ручные операции.</span><span class="sxs-lookup"><span data-stu-id="bf38b-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="bf38b-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="bf38b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-137">Int32</span></span>|<span data-ttu-id="bf38b-138">Число ожидающих автономной проверки устройства.</span><span class="sxs-lookup"><span data-stu-id="bf38b-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="bf38b-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bf38b-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="bf38b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="bf38b-140">Int32</span></span>|<span data-ttu-id="bf38b-141">Счетчик устройства критические ошибки.</span><span class="sxs-lookup"><span data-stu-id="bf38b-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf38b-142">Связи</span><span class="sxs-lookup"><span data-stu-id="bf38b-142">Relationships</span></span>
<span data-ttu-id="bf38b-143">Нет</span><span class="sxs-lookup"><span data-stu-id="bf38b-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf38b-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf38b-144">JSON Representation</span></span>
<span data-ttu-id="bf38b-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf38b-145">Here is a JSON representation of the resource.</span></span>
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





