---
title: Тип ресурса windowsProtectionState
description: Устройство защиты состояния сущности.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a21cc27039f3119836e0027b2558cadadab1b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884107"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="1651e-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1651e-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="1651e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1651e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1651e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1651e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1651e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1651e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1651e-107">Устройство защиты состояния сущности.</span><span class="sxs-lookup"><span data-stu-id="1651e-107">Device protection status entity.</span></span>
## <a name="methods"></a><span data-ttu-id="1651e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1651e-108">Methods</span></span>
|<span data-ttu-id="1651e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1651e-109">Method</span></span>|<span data-ttu-id="1651e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1651e-110">Return Type</span></span>|<span data-ttu-id="1651e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1651e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1651e-112">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1651e-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="1651e-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1651e-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="1651e-114">Чтение свойства и связи объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="1651e-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="1651e-115">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1651e-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="1651e-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="1651e-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="1651e-117">Обновление свойства объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="1651e-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1651e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="1651e-118">Properties</span></span>
|<span data-ttu-id="1651e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="1651e-119">Property</span></span>|<span data-ttu-id="1651e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1651e-120">Type</span></span>|<span data-ttu-id="1651e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1651e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1651e-122">id</span><span class="sxs-lookup"><span data-stu-id="1651e-122">id</span></span>|<span data-ttu-id="1651e-123">Строка</span><span class="sxs-lookup"><span data-stu-id="1651e-123">String</span></span>|<span data-ttu-id="1651e-124">Уникальный идентификатор для объекта состояния защиты устройств.</span><span class="sxs-lookup"><span data-stu-id="1651e-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="1651e-125">— Идентификатор устройства, устройства</span><span class="sxs-lookup"><span data-stu-id="1651e-125">This is device id of the device</span></span>|
|<span data-ttu-id="1651e-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1651e-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="1651e-127">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-127">Boolean</span></span>|<span data-ttu-id="1651e-128">Защита от вредоносных программ включен или не</span><span class="sxs-lookup"><span data-stu-id="1651e-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="1651e-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="1651e-129">deviceState</span></span>|[<span data-ttu-id="1651e-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="1651e-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="1651e-131">Состояние компьютера (например, очистить или Ожидание полного сканирования или помещенных в очередь перезагрузки и т.).</span><span class="sxs-lookup"><span data-stu-id="1651e-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="1651e-132">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="1651e-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="1651e-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="1651e-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="1651e-134">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-134">Boolean</span></span>|<span data-ttu-id="1651e-135">Защита в режиме реального времени включено или нет?</span><span class="sxs-lookup"><span data-stu-id="1651e-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="1651e-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="1651e-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="1651e-137">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-137">Boolean</span></span>|<span data-ttu-id="1651e-138">Система проверки сети включено или нет?</span><span class="sxs-lookup"><span data-stu-id="1651e-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="1651e-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="1651e-139">quickScanOverdue</span></span>|<span data-ttu-id="1651e-140">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-140">Boolean</span></span>|<span data-ttu-id="1651e-141">Быстрое сканирование просроченные или не?</span><span class="sxs-lookup"><span data-stu-id="1651e-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="1651e-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="1651e-142">fullScanOverdue</span></span>|<span data-ttu-id="1651e-143">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-143">Boolean</span></span>|<span data-ttu-id="1651e-144">Полное сканирование просроченные или нет?</span><span class="sxs-lookup"><span data-stu-id="1651e-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="1651e-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="1651e-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="1651e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-146">Boolean</span></span>|<span data-ttu-id="1651e-147">Устаревший подписи или нет?</span><span class="sxs-lookup"><span data-stu-id="1651e-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="1651e-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="1651e-148">rebootRequired</span></span>|<span data-ttu-id="1651e-149">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-149">Boolean</span></span>|<span data-ttu-id="1651e-150">Требуется ли перезагрузка?</span><span class="sxs-lookup"><span data-stu-id="1651e-150">Reboot required or not?</span></span>|
|<span data-ttu-id="1651e-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="1651e-151">fullScanRequired</span></span>|<span data-ttu-id="1651e-152">Логический</span><span class="sxs-lookup"><span data-stu-id="1651e-152">Boolean</span></span>|<span data-ttu-id="1651e-153">Полная проверка, требуется или нет?</span><span class="sxs-lookup"><span data-stu-id="1651e-153">Full scan required or not?</span></span>|
|<span data-ttu-id="1651e-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="1651e-154">engineVersion</span></span>|<span data-ttu-id="1651e-155">Строка</span><span class="sxs-lookup"><span data-stu-id="1651e-155">String</span></span>|<span data-ttu-id="1651e-156">Версия текущей конечной точки защиты ядра</span><span class="sxs-lookup"><span data-stu-id="1651e-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="1651e-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="1651e-157">signatureVersion</span></span>|<span data-ttu-id="1651e-158">Строка</span><span class="sxs-lookup"><span data-stu-id="1651e-158">String</span></span>|<span data-ttu-id="1651e-159">Текущая версия определения вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="1651e-159">Current malware definitions version</span></span>|
|<span data-ttu-id="1651e-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="1651e-160">antiMalwareVersion</span></span>|<span data-ttu-id="1651e-161">Строка</span><span class="sxs-lookup"><span data-stu-id="1651e-161">String</span></span>|<span data-ttu-id="1651e-162">Текущая платформа защита от вредоносных программ версии</span><span class="sxs-lookup"><span data-stu-id="1651e-162">Current anti malware version</span></span>|
|<span data-ttu-id="1651e-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="1651e-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="1651e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1651e-164">DateTimeOffset</span></span>|<span data-ttu-id="1651e-165">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="1651e-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="1651e-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="1651e-166">lastFullScanDateTime</span></span>|<span data-ttu-id="1651e-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1651e-167">DateTimeOffset</span></span>|<span data-ttu-id="1651e-168">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="1651e-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="1651e-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="1651e-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="1651e-170">Строка</span><span class="sxs-lookup"><span data-stu-id="1651e-170">String</span></span>|<span data-ttu-id="1651e-171">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="1651e-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="1651e-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="1651e-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="1651e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1651e-173">String</span></span>|<span data-ttu-id="1651e-174">Последняя версия полная проверка подписи</span><span class="sxs-lookup"><span data-stu-id="1651e-174">Last full scan signature version</span></span>|
|<span data-ttu-id="1651e-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1651e-175">lastReportedDateTime</span></span>|<span data-ttu-id="1651e-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1651e-176">DateTimeOffset</span></span>|<span data-ttu-id="1651e-177">Последнее состояние работоспособности устройства, обнаруженных времени</span><span class="sxs-lookup"><span data-stu-id="1651e-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="1651e-178">Связи</span><span class="sxs-lookup"><span data-stu-id="1651e-178">Relationships</span></span>
|<span data-ttu-id="1651e-179">Связь</span><span class="sxs-lookup"><span data-stu-id="1651e-179">Relationship</span></span>|<span data-ttu-id="1651e-180">Тип</span><span class="sxs-lookup"><span data-stu-id="1651e-180">Type</span></span>|<span data-ttu-id="1651e-181">Описание</span><span class="sxs-lookup"><span data-stu-id="1651e-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1651e-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="1651e-182">detectedMalwareState</span></span>|<span data-ttu-id="1651e-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1651e-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="1651e-184">Список устройств вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="1651e-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1651e-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1651e-185">JSON Representation</span></span>
<span data-ttu-id="1651e-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1651e-186">Here is a JSON representation of the resource.</span></span>
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





