---
title: Тип ресурса Девицехеалсскриптрунсуммари
description: Содержит свойства сводки по запуску сценария управления устройствами.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1be7c470bb2776b16f74f352dc93e1f56163abf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784939"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="c92fe-103">Тип ресурса Девицехеалсскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="c92fe-103">deviceHealthScriptRunSummary resource type</span></span>

> <span data-ttu-id="c92fe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c92fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c92fe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c92fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c92fe-106">Содержит свойства сводки по запуску сценария управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="c92fe-106">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="c92fe-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c92fe-107">Methods</span></span>
|<span data-ttu-id="c92fe-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c92fe-108">Method</span></span>|<span data-ttu-id="c92fe-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c92fe-109">Return Type</span></span>|<span data-ttu-id="c92fe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c92fe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c92fe-111">Получение Девицехеалсскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="c92fe-111">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="c92fe-112">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c92fe-112">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="c92fe-113">Чтение свойств и связей объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c92fe-113">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="c92fe-114">Обновление Девицехеалсскриптрунсуммари</span><span class="sxs-lookup"><span data-stu-id="c92fe-114">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="c92fe-115">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="c92fe-115">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="c92fe-116">Обновление свойств объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="c92fe-116">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c92fe-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c92fe-117">Properties</span></span>
|<span data-ttu-id="c92fe-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c92fe-118">Property</span></span>|<span data-ttu-id="c92fe-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c92fe-119">Type</span></span>|<span data-ttu-id="c92fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c92fe-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c92fe-121">id</span><span class="sxs-lookup"><span data-stu-id="c92fe-121">id</span></span>|<span data-ttu-id="c92fe-122">String</span><span class="sxs-lookup"><span data-stu-id="c92fe-122">String</span></span>|<span data-ttu-id="c92fe-123">Ключевой объект сводки запуска сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="c92fe-123">Key of the device health script run summary entity.</span></span> <span data-ttu-id="c92fe-124">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c92fe-124">This property is read-only.</span></span>|
|<span data-ttu-id="c92fe-125">ноиссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-125">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="c92fe-126">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-126">Int32</span></span>|<span data-ttu-id="c92fe-127">Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии.</span><span class="sxs-lookup"><span data-stu-id="c92fe-127">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="c92fe-128">иссуедетектеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-128">issueDetectedDeviceCount</span></span>|<span data-ttu-id="c92fe-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-129">Int32</span></span>|<span data-ttu-id="c92fe-130">Количество устройств, для которых обнаружена ошибка сценария обнаружения</span><span class="sxs-lookup"><span data-stu-id="c92fe-130">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="c92fe-131">детектионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-131">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="c92fe-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-132">Int32</span></span>|<span data-ttu-id="c92fe-133">Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен</span><span class="sxs-lookup"><span data-stu-id="c92fe-133">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="c92fe-134">детектионскриптпендингдевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-134">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="c92fe-135">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-135">Int32</span></span>|<span data-ttu-id="c92fe-136">Количество устройств, на которых еще не выполнялась последняя версия сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="c92fe-136">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="c92fe-137">иссуеремедиатеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-137">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="c92fe-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-138">Int32</span></span>|<span data-ttu-id="c92fe-139">Количество устройств, для которых сценарий исправления мог разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="c92fe-139">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="c92fe-140">ремедиатионскиппеддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-140">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="c92fe-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-141">Int32</span></span>|<span data-ttu-id="c92fe-142">Количество устройств, для которых было пропущено исправление</span><span class="sxs-lookup"><span data-stu-id="c92fe-142">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="c92fe-143">иссуереоккурреддевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-143">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="c92fe-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-144">Int32</span></span>|<span data-ttu-id="c92fe-145">Количество устройств, для которых сценарий исправления успешно выполнен, но не удалось разрешить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="c92fe-145">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="c92fe-146">ремедиатионскриптеррордевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-146">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="c92fe-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-147">Int32</span></span>|<span data-ttu-id="c92fe-148">Количество устройств, для которых при выполнении сценария исправления возникла ошибка и оно не было завершено</span><span class="sxs-lookup"><span data-stu-id="c92fe-148">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="c92fe-149">ластскриптрундатетиме</span><span class="sxs-lookup"><span data-stu-id="c92fe-149">lastScriptRunDateTime</span></span>|<span data-ttu-id="c92fe-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c92fe-150">DateTimeOffset</span></span>|<span data-ttu-id="c92fe-151">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="c92fe-151">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="c92fe-152">иссуеремедиатедкумулативедевицекаунт</span><span class="sxs-lookup"><span data-stu-id="c92fe-152">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="c92fe-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c92fe-153">Int32</span></span>|<span data-ttu-id="c92fe-154">Количество устройств, которые были исправлены за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="c92fe-154">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="c92fe-155">Связи</span><span class="sxs-lookup"><span data-stu-id="c92fe-155">Relationships</span></span>
<span data-ttu-id="c92fe-156">Нет</span><span class="sxs-lookup"><span data-stu-id="c92fe-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c92fe-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c92fe-157">JSON Representation</span></span>
<span data-ttu-id="c92fe-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c92fe-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```



