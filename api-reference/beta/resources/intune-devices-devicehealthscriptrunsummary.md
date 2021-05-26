---
title: тип ресурса deviceHealthScriptRunSummary
description: Содержит свойства для сводки запуска скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b1c1b31413c19436c7dceb34a2055a238fe5881a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665233"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a><span data-ttu-id="a4c09-103">тип ресурса deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="a4c09-103">deviceHealthScriptRunSummary resource type</span></span>

<span data-ttu-id="a4c09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4c09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4c09-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4c09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4c09-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4c09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4c09-107">Содержит свойства для сводки запуска скрипта управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="a4c09-107">Contains properties for the run summary of a device management script.</span></span>

## <a name="methods"></a><span data-ttu-id="a4c09-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a4c09-108">Methods</span></span>
|<span data-ttu-id="a4c09-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a4c09-109">Method</span></span>|<span data-ttu-id="a4c09-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a4c09-110">Return Type</span></span>|<span data-ttu-id="a4c09-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4c09-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a4c09-112">Get deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="a4c09-112">Get deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[<span data-ttu-id="a4c09-113">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="a4c09-113">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="a4c09-114">Чтение свойств и связей [объекта deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4c09-114">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|
|[<span data-ttu-id="a4c09-115">Обновление устройстваHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="a4c09-115">Update deviceHealthScriptRunSummary</span></span>](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[<span data-ttu-id="a4c09-116">deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="a4c09-116">deviceHealthScriptRunSummary</span></span>](../resources/intune-devices-devicehealthscriptrunsummary.md)|<span data-ttu-id="a4c09-117">Обновление свойств объекта [deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="a4c09-117">Update the properties of a [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4c09-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4c09-118">Properties</span></span>
|<span data-ttu-id="a4c09-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4c09-119">Property</span></span>|<span data-ttu-id="a4c09-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a4c09-120">Type</span></span>|<span data-ttu-id="a4c09-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a4c09-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4c09-122">id</span><span class="sxs-lookup"><span data-stu-id="a4c09-122">id</span></span>|<span data-ttu-id="a4c09-123">Строка</span><span class="sxs-lookup"><span data-stu-id="a4c09-123">String</span></span>|<span data-ttu-id="a4c09-124">Ключ скрипта для службы службы устройств запустите объект сводки.</span><span class="sxs-lookup"><span data-stu-id="a4c09-124">Key of the device health script run summary entity.</span></span> <span data-ttu-id="a4c09-125">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4c09-125">This property is read-only.</span></span>|
|<span data-ttu-id="a4c09-126">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-126">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="a4c09-127">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-127">Int32</span></span>|<span data-ttu-id="a4c09-128">Количество устройств, для которых сценарий обнаружения не нашел проблемы и устройство является здоровым</span><span class="sxs-lookup"><span data-stu-id="a4c09-128">Number of devices for which the detection script did not find an issue and the device is healthy</span></span>|
|<span data-ttu-id="a4c09-129">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-129">issueDetectedDeviceCount</span></span>|<span data-ttu-id="a4c09-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-130">Int32</span></span>|<span data-ttu-id="a4c09-131">Количество устройств, для которых скрипт обнаружения обнаружил проблему</span><span class="sxs-lookup"><span data-stu-id="a4c09-131">Number of devices for which the detection script found an issue</span></span>|
|<span data-ttu-id="a4c09-132">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-132">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="a4c09-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-133">Int32</span></span>|<span data-ttu-id="a4c09-134">Количество устройств, на которых при выполнении скрипта обнаружения произошла ошибка и не была завершена</span><span class="sxs-lookup"><span data-stu-id="a4c09-134">Number of devices on which the detection script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="a4c09-135">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-135">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="a4c09-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-136">Int32</span></span>|<span data-ttu-id="a4c09-137">Количество устройств, которые еще не запускают последнюю версию скрипта здоровья устройств</span><span class="sxs-lookup"><span data-stu-id="a4c09-137">Number of devices which have not yet run the latest version of the device health script</span></span>|
|<span data-ttu-id="a4c09-138">detectionScriptNotApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-138">detectionScriptNotApplicableDeviceCount</span></span>|<span data-ttu-id="a4c09-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-139">Int32</span></span>|<span data-ttu-id="a4c09-140">Количество устройств, для которых сценарий обнаружения не был применим</span><span class="sxs-lookup"><span data-stu-id="a4c09-140">Number of devices for which the detection script was not applicable</span></span>|
|<span data-ttu-id="a4c09-141">issueRemediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-141">issueRemediatedDeviceCount</span></span>|<span data-ttu-id="a4c09-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-142">Int32</span></span>|<span data-ttu-id="a4c09-143">Количество устройств, для которых сценарий восстановления смог устранить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="a4c09-143">Number of devices for which the remediation script was able to resolve the detected issue</span></span>|
|<span data-ttu-id="a4c09-144">remediationSkippedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-144">remediationSkippedDeviceCount</span></span>|<span data-ttu-id="a4c09-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-145">Int32</span></span>|<span data-ttu-id="a4c09-146">Количество устройств, для которых было пропущено исправление</span><span class="sxs-lookup"><span data-stu-id="a4c09-146">Number of devices for which remediation was skipped</span></span>|
|<span data-ttu-id="a4c09-147">issueReoccurredDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-147">issueReoccurredDeviceCount</span></span>|<span data-ttu-id="a4c09-148">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-148">Int32</span></span>|<span data-ttu-id="a4c09-149">Количество устройств, для которых успешно выполнен сценарий восстановления, но не удалось устранить обнаруженную проблему</span><span class="sxs-lookup"><span data-stu-id="a4c09-149">Number of devices for which the remediation script executed successfully but failed to resolve the detected issue</span></span>|
|<span data-ttu-id="a4c09-150">remediationScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-150">remediationScriptErrorDeviceCount</span></span>|<span data-ttu-id="a4c09-151">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-151">Int32</span></span>|<span data-ttu-id="a4c09-152">Количество устройств, для которых при выполнении сценария восстановления произошла ошибка и не была завершена</span><span class="sxs-lookup"><span data-stu-id="a4c09-152">Number of devices for which the remediation script execution encountered an error and did not complete</span></span>|
|<span data-ttu-id="a4c09-153">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="a4c09-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="a4c09-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4c09-154">DateTimeOffset</span></span>|<span data-ttu-id="a4c09-155">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="a4c09-155">Last run time for the script across all devices</span></span>|
|<span data-ttu-id="a4c09-156">issueRemediatedCumulativeDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a4c09-156">issueRemediatedCumulativeDeviceCount</span></span>|<span data-ttu-id="a4c09-157">Int32</span><span class="sxs-lookup"><span data-stu-id="a4c09-157">Int32</span></span>|<span data-ttu-id="a4c09-158">Количество устройств, которые были исправлены за последние 30 дней</span><span class="sxs-lookup"><span data-stu-id="a4c09-158">Number of devices that were remediated over the last 30 days</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4c09-159">Связи</span><span class="sxs-lookup"><span data-stu-id="a4c09-159">Relationships</span></span>
<span data-ttu-id="a4c09-160">Нет</span><span class="sxs-lookup"><span data-stu-id="a4c09-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4c09-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4c09-161">JSON Representation</span></span>
<span data-ttu-id="a4c09-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4c09-162">Here is a JSON representation of the resource.</span></span>
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
  "detectionScriptNotApplicableDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```




