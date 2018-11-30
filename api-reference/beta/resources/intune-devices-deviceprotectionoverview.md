---
title: Тип ресурса deviceProtectionOverview
description: Сведения об оборудовании данного устройства.
ms.openlocfilehash: 81252fdf60c1de129a615b075968e0e6f1eca943
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080150"
---
# <a name="deviceprotectionoverview-resource-type"></a><span data-ttu-id="1db4c-103">Тип ресурса deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="1db4c-103">deviceProtectionOverview resource type</span></span>

> <span data-ttu-id="1db4c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1db4c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1db4c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1db4c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1db4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1db4c-107">Сведения об оборудовании данного устройства.</span><span class="sxs-lookup"><span data-stu-id="1db4c-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="1db4c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1db4c-108">Properties</span></span>
|<span data-ttu-id="1db4c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1db4c-109">Property</span></span>|<span data-ttu-id="1db4c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1db4c-110">Type</span></span>|<span data-ttu-id="1db4c-111">Description</span><span class="sxs-lookup"><span data-stu-id="1db4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1db4c-112">totalReportedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-112">totalReportedDeviceCount</span></span>|<span data-ttu-id="1db4c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-113">Int32</span></span>|<span data-ttu-id="1db4c-114">Счетчик общее устройства.</span><span class="sxs-lookup"><span data-stu-id="1db4c-114">Total device count.</span></span>|
|<span data-ttu-id="1db4c-115">inactiveThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-115">inactiveThreatAgentDeviceCount</span></span>|<span data-ttu-id="1db4c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-116">Int32</span></span>|<span data-ttu-id="1db4c-117">Устройства со счетчиком агента неактивных угроз</span><span class="sxs-lookup"><span data-stu-id="1db4c-117">Device with inactive threat agent count</span></span>|
|<span data-ttu-id="1db4c-118">unknownStateThreatAgentDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-118">unknownStateThreatAgentDeviceCount</span></span>|<span data-ttu-id="1db4c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-119">Int32</span></span>|<span data-ttu-id="1db4c-120">Устройство с состоянием агента угроз, как число неизвестно.</span><span class="sxs-lookup"><span data-stu-id="1db4c-120">Device with threat agent state as unknown count.</span></span>|
|<span data-ttu-id="1db4c-121">pendingSignatureUpdateDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-121">pendingSignatureUpdateDeviceCount</span></span>|<span data-ttu-id="1db4c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-122">Int32</span></span>|<span data-ttu-id="1db4c-123">Устройство со старой счетчиком подписи.</span><span class="sxs-lookup"><span data-stu-id="1db4c-123">Device with old signature count.</span></span>|
|<span data-ttu-id="1db4c-124">cleanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-124">cleanDeviceCount</span></span>|<span data-ttu-id="1db4c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-125">Int32</span></span>|<span data-ttu-id="1db4c-126">Счетчик чистой устройства.</span><span class="sxs-lookup"><span data-stu-id="1db4c-126">Clean device count.</span></span>|
|<span data-ttu-id="1db4c-127">pendingFullScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-127">pendingFullScanDeviceCount</span></span>|<span data-ttu-id="1db4c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-128">Int32</span></span>|<span data-ttu-id="1db4c-129">Счетчик устройства ожидающие полную проверку.</span><span class="sxs-lookup"><span data-stu-id="1db4c-129">Pending full scan device count.</span></span>|
|<span data-ttu-id="1db4c-130">pendingRestartDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-130">pendingRestartDeviceCount</span></span>|<span data-ttu-id="1db4c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-131">Int32</span></span>|<span data-ttu-id="1db4c-132">Счетчик отложенная перезагрузка устройства.</span><span class="sxs-lookup"><span data-stu-id="1db4c-132">Pending restart device count.</span></span>|
|<span data-ttu-id="1db4c-133">pendingManualStepsDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-133">pendingManualStepsDeviceCount</span></span>|<span data-ttu-id="1db4c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-134">Int32</span></span>|<span data-ttu-id="1db4c-135">Счетчик устройства ожидающие ручные операции.</span><span class="sxs-lookup"><span data-stu-id="1db4c-135">Pending manual steps device count.</span></span>|
|<span data-ttu-id="1db4c-136">pendingOfflineScanDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-136">pendingOfflineScanDeviceCount</span></span>|<span data-ttu-id="1db4c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-137">Int32</span></span>|<span data-ttu-id="1db4c-138">Число ожидающих автономной проверки устройства.</span><span class="sxs-lookup"><span data-stu-id="1db4c-138">Pending offline scan device count.</span></span>|
|<span data-ttu-id="1db4c-139">criticalFailuresDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1db4c-139">criticalFailuresDeviceCount</span></span>|<span data-ttu-id="1db4c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1db4c-140">Int32</span></span>|<span data-ttu-id="1db4c-141">Счетчик устройства критические ошибки.</span><span class="sxs-lookup"><span data-stu-id="1db4c-141">Critical failures device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1db4c-142">Связи</span><span class="sxs-lookup"><span data-stu-id="1db4c-142">Relationships</span></span>
<span data-ttu-id="1db4c-143">Нет</span><span class="sxs-lookup"><span data-stu-id="1db4c-143">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1db4c-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1db4c-144">JSON Representation</span></span>
<span data-ttu-id="1db4c-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1db4c-145">Here is a JSON representation of the resource.</span></span>
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





