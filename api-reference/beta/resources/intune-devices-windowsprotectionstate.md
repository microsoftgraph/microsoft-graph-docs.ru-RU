---
title: Тип ресурса windowsProtectionState
description: Устройство защиты состояния сущности.
ms.openlocfilehash: dfdfb5f79f696e2f6f577f59b7597f16c89a5d56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081581"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="f2d6b-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="f2d6b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2d6b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2d6b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d6b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2d6b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f2d6b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2d6b-107">Устройство защиты состояния сущности.</span><span class="sxs-lookup"><span data-stu-id="f2d6b-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="f2d6b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="f2d6b-108">Methods</span></span>
|<span data-ttu-id="f2d6b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="f2d6b-109">Method</span></span>|<span data-ttu-id="f2d6b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2d6b-110">Return Type</span></span>|<span data-ttu-id="f2d6b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f2d6b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2d6b-112">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="f2d6b-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="f2d6b-114">Чтение свойства и связи объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="f2d6b-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="f2d6b-115">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="f2d6b-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="f2d6b-117">Обновление свойства объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="f2d6b-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2d6b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2d6b-118">Properties</span></span>
|<span data-ttu-id="f2d6b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2d6b-119">Property</span></span>|<span data-ttu-id="f2d6b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f2d6b-120">Type</span></span>|<span data-ttu-id="f2d6b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f2d6b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2d6b-122">id</span><span class="sxs-lookup"><span data-stu-id="f2d6b-122">id</span></span>|<span data-ttu-id="f2d6b-123">String</span><span class="sxs-lookup"><span data-stu-id="f2d6b-123">String</span></span>|<span data-ttu-id="f2d6b-124">Уникальный идентификатор для объекта состояния защиты устройств.</span><span class="sxs-lookup"><span data-stu-id="f2d6b-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="f2d6b-125">— Идентификатор устройства, устройства</span><span class="sxs-lookup"><span data-stu-id="f2d6b-125">This is device id of the device</span></span>|
|<span data-ttu-id="f2d6b-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f2d6b-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="f2d6b-127">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-127">Boolean</span></span>|<span data-ttu-id="f2d6b-128">Защита от вредоносных программ включен или не</span><span class="sxs-lookup"><span data-stu-id="f2d6b-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="f2d6b-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-129">deviceState</span></span>|[<span data-ttu-id="f2d6b-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="f2d6b-131">Состояние компьютера (например, очистить или Ожидание полного сканирования или помещенных в очередь перезагрузки и т.).</span><span class="sxs-lookup"><span data-stu-id="f2d6b-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="f2d6b-132">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="f2d6b-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="f2d6b-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f2d6b-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="f2d6b-134">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-134">Boolean</span></span>|<span data-ttu-id="f2d6b-135">Защита в режиме реального времени включено или нет?</span><span class="sxs-lookup"><span data-stu-id="f2d6b-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="f2d6b-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="f2d6b-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="f2d6b-137">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-137">Boolean</span></span>|<span data-ttu-id="f2d6b-138">Система проверки сети включено или нет?</span><span class="sxs-lookup"><span data-stu-id="f2d6b-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="f2d6b-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f2d6b-139">quickScanOverdue</span></span>|<span data-ttu-id="f2d6b-140">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-140">Boolean</span></span>|<span data-ttu-id="f2d6b-141">Быстрое сканирование просроченные или не?</span><span class="sxs-lookup"><span data-stu-id="f2d6b-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="f2d6b-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f2d6b-142">fullScanOverdue</span></span>|<span data-ttu-id="f2d6b-143">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-143">Boolean</span></span>|<span data-ttu-id="f2d6b-144">Полное сканирование просроченные или нет?</span><span class="sxs-lookup"><span data-stu-id="f2d6b-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="f2d6b-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="f2d6b-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="f2d6b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-146">Boolean</span></span>|<span data-ttu-id="f2d6b-147">Устаревший подписи или нет?</span><span class="sxs-lookup"><span data-stu-id="f2d6b-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="f2d6b-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="f2d6b-148">rebootRequired</span></span>|<span data-ttu-id="f2d6b-149">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-149">Boolean</span></span>|<span data-ttu-id="f2d6b-150">Требуется ли перезагрузка?</span><span class="sxs-lookup"><span data-stu-id="f2d6b-150">Reboot required or not?</span></span>|
|<span data-ttu-id="f2d6b-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="f2d6b-151">fullScanRequired</span></span>|<span data-ttu-id="f2d6b-152">Логический</span><span class="sxs-lookup"><span data-stu-id="f2d6b-152">Boolean</span></span>|<span data-ttu-id="f2d6b-153">Полная проверка, требуется или нет?</span><span class="sxs-lookup"><span data-stu-id="f2d6b-153">Full scan required or not?</span></span>|
|<span data-ttu-id="f2d6b-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="f2d6b-154">engineVersion</span></span>|<span data-ttu-id="f2d6b-155">String</span><span class="sxs-lookup"><span data-stu-id="f2d6b-155">String</span></span>|<span data-ttu-id="f2d6b-156">Версия текущей конечной точки защиты ядра</span><span class="sxs-lookup"><span data-stu-id="f2d6b-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="f2d6b-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="f2d6b-157">signatureVersion</span></span>|<span data-ttu-id="f2d6b-158">String</span><span class="sxs-lookup"><span data-stu-id="f2d6b-158">String</span></span>|<span data-ttu-id="f2d6b-159">Текущая версия определения вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="f2d6b-159">Current malware definitions version</span></span>|
|<span data-ttu-id="f2d6b-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="f2d6b-160">antiMalwareVersion</span></span>|<span data-ttu-id="f2d6b-161">String</span><span class="sxs-lookup"><span data-stu-id="f2d6b-161">String</span></span>|<span data-ttu-id="f2d6b-162">Текущая платформа защита от вредоносных программ версии</span><span class="sxs-lookup"><span data-stu-id="f2d6b-162">Current anti malware version</span></span>|
|<span data-ttu-id="f2d6b-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f2d6b-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="f2d6b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2d6b-164">DateTimeOffset</span></span>|<span data-ttu-id="f2d6b-165">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="f2d6b-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="f2d6b-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f2d6b-166">lastFullScanDateTime</span></span>|<span data-ttu-id="f2d6b-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2d6b-167">DateTimeOffset</span></span>|<span data-ttu-id="f2d6b-168">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="f2d6b-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="f2d6b-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f2d6b-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="f2d6b-170">String</span><span class="sxs-lookup"><span data-stu-id="f2d6b-170">String</span></span>|<span data-ttu-id="f2d6b-171">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="f2d6b-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="f2d6b-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f2d6b-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="f2d6b-173">String</span><span class="sxs-lookup"><span data-stu-id="f2d6b-173">String</span></span>|<span data-ttu-id="f2d6b-174">Последняя версия полная проверка подписи</span><span class="sxs-lookup"><span data-stu-id="f2d6b-174">Last full scan signature version</span></span>|
|<span data-ttu-id="f2d6b-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2d6b-175">lastReportedDateTime</span></span>|<span data-ttu-id="f2d6b-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2d6b-176">DateTimeOffset</span></span>|<span data-ttu-id="f2d6b-177">Последнее состояние работоспособности устройства, обнаруженных времени</span><span class="sxs-lookup"><span data-stu-id="f2d6b-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2d6b-178">Связи</span><span class="sxs-lookup"><span data-stu-id="f2d6b-178">Relationships</span></span>
|<span data-ttu-id="f2d6b-179">Связь</span><span class="sxs-lookup"><span data-stu-id="f2d6b-179">Relationship</span></span>|<span data-ttu-id="f2d6b-180">Тип</span><span class="sxs-lookup"><span data-stu-id="f2d6b-180">Type</span></span>|<span data-ttu-id="f2d6b-181">Description</span><span class="sxs-lookup"><span data-stu-id="f2d6b-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2d6b-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="f2d6b-182">detectedMalwareState</span></span>|<span data-ttu-id="f2d6b-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f2d6b-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="f2d6b-184">Список устройств вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="f2d6b-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2d6b-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2d6b-185">JSON Representation</span></span>
<span data-ttu-id="f2d6b-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2d6b-186">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





