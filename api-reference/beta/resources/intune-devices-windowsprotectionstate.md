---
title: Тип ресурса windowsProtectionState
description: Устройство защиты состояния сущности.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1ef6c86983475abc687055ac2322ba02fae27ecd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423589"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="2cbf2-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-103">windowsProtectionState resource type</span></span>

> <span data-ttu-id="2cbf2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2cbf2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cbf2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cbf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cbf2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cbf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cbf2-107">Устройство защиты состояния сущности.</span><span class="sxs-lookup"><span data-stu-id="2cbf2-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="2cbf2-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2cbf2-108">Methods</span></span>
|<span data-ttu-id="2cbf2-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2cbf2-109">Method</span></span>|<span data-ttu-id="2cbf2-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2cbf2-110">Return Type</span></span>|<span data-ttu-id="2cbf2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2cbf2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2cbf2-112">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="2cbf2-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="2cbf2-114">Чтение свойства и связи объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="2cbf2-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="2cbf2-115">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="2cbf2-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="2cbf2-117">Обновление свойства объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="2cbf2-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2cbf2-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cbf2-118">Properties</span></span>
|<span data-ttu-id="2cbf2-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cbf2-119">Property</span></span>|<span data-ttu-id="2cbf2-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2cbf2-120">Type</span></span>|<span data-ttu-id="2cbf2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2cbf2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cbf2-122">id</span><span class="sxs-lookup"><span data-stu-id="2cbf2-122">id</span></span>|<span data-ttu-id="2cbf2-123">String</span><span class="sxs-lookup"><span data-stu-id="2cbf2-123">String</span></span>|<span data-ttu-id="2cbf2-124">Уникальный идентификатор для объекта состояния защиты устройств.</span><span class="sxs-lookup"><span data-stu-id="2cbf2-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="2cbf2-125">— Идентификатор устройства, устройства</span><span class="sxs-lookup"><span data-stu-id="2cbf2-125">This is device id of the device</span></span>|
|<span data-ttu-id="2cbf2-126">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2cbf2-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="2cbf2-127">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-127">Boolean</span></span>|<span data-ttu-id="2cbf2-128">Защита от вредоносных программ включен или не</span><span class="sxs-lookup"><span data-stu-id="2cbf2-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="2cbf2-129">deviceState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-129">deviceState</span></span>|[<span data-ttu-id="2cbf2-130">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="2cbf2-131">Состояние компьютера (например, очистить или Ожидание полного сканирования или помещенных в очередь перезагрузки и т.).</span><span class="sxs-lookup"><span data-stu-id="2cbf2-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="2cbf2-132">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="2cbf2-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="2cbf2-133">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="2cbf2-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="2cbf2-134">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-134">Boolean</span></span>|<span data-ttu-id="2cbf2-135">Защита в режиме реального времени включено или нет?</span><span class="sxs-lookup"><span data-stu-id="2cbf2-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="2cbf2-136">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="2cbf2-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="2cbf2-137">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-137">Boolean</span></span>|<span data-ttu-id="2cbf2-138">Система проверки сети включено или нет?</span><span class="sxs-lookup"><span data-stu-id="2cbf2-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="2cbf2-139">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="2cbf2-139">quickScanOverdue</span></span>|<span data-ttu-id="2cbf2-140">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-140">Boolean</span></span>|<span data-ttu-id="2cbf2-141">Быстрое сканирование просроченные или не?</span><span class="sxs-lookup"><span data-stu-id="2cbf2-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="2cbf2-142">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="2cbf2-142">fullScanOverdue</span></span>|<span data-ttu-id="2cbf2-143">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-143">Boolean</span></span>|<span data-ttu-id="2cbf2-144">Полное сканирование просроченные или нет?</span><span class="sxs-lookup"><span data-stu-id="2cbf2-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="2cbf2-145">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="2cbf2-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="2cbf2-146">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-146">Boolean</span></span>|<span data-ttu-id="2cbf2-147">Устаревший подписи или нет?</span><span class="sxs-lookup"><span data-stu-id="2cbf2-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="2cbf2-148">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="2cbf2-148">rebootRequired</span></span>|<span data-ttu-id="2cbf2-149">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-149">Boolean</span></span>|<span data-ttu-id="2cbf2-150">Требуется ли перезагрузка?</span><span class="sxs-lookup"><span data-stu-id="2cbf2-150">Reboot required or not?</span></span>|
|<span data-ttu-id="2cbf2-151">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="2cbf2-151">fullScanRequired</span></span>|<span data-ttu-id="2cbf2-152">Логический</span><span class="sxs-lookup"><span data-stu-id="2cbf2-152">Boolean</span></span>|<span data-ttu-id="2cbf2-153">Полная проверка, требуется или нет?</span><span class="sxs-lookup"><span data-stu-id="2cbf2-153">Full scan required or not?</span></span>|
|<span data-ttu-id="2cbf2-154">engineVersion</span><span class="sxs-lookup"><span data-stu-id="2cbf2-154">engineVersion</span></span>|<span data-ttu-id="2cbf2-155">String</span><span class="sxs-lookup"><span data-stu-id="2cbf2-155">String</span></span>|<span data-ttu-id="2cbf2-156">Версия текущей конечной точки защиты ядра</span><span class="sxs-lookup"><span data-stu-id="2cbf2-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="2cbf2-157">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="2cbf2-157">signatureVersion</span></span>|<span data-ttu-id="2cbf2-158">String</span><span class="sxs-lookup"><span data-stu-id="2cbf2-158">String</span></span>|<span data-ttu-id="2cbf2-159">Текущая версия определения вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="2cbf2-159">Current malware definitions version</span></span>|
|<span data-ttu-id="2cbf2-160">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="2cbf2-160">antiMalwareVersion</span></span>|<span data-ttu-id="2cbf2-161">String</span><span class="sxs-lookup"><span data-stu-id="2cbf2-161">String</span></span>|<span data-ttu-id="2cbf2-162">Текущая платформа защита от вредоносных программ версии</span><span class="sxs-lookup"><span data-stu-id="2cbf2-162">Current anti malware version</span></span>|
|<span data-ttu-id="2cbf2-163">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="2cbf2-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="2cbf2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cbf2-164">DateTimeOffset</span></span>|<span data-ttu-id="2cbf2-165">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="2cbf2-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="2cbf2-166">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="2cbf2-166">lastFullScanDateTime</span></span>|<span data-ttu-id="2cbf2-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cbf2-167">DateTimeOffset</span></span>|<span data-ttu-id="2cbf2-168">Даты и времени последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="2cbf2-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="2cbf2-169">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="2cbf2-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="2cbf2-170">String</span><span class="sxs-lookup"><span data-stu-id="2cbf2-170">String</span></span>|<span data-ttu-id="2cbf2-171">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="2cbf2-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="2cbf2-172">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="2cbf2-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="2cbf2-173">String</span><span class="sxs-lookup"><span data-stu-id="2cbf2-173">String</span></span>|<span data-ttu-id="2cbf2-174">Последняя версия полная проверка подписи</span><span class="sxs-lookup"><span data-stu-id="2cbf2-174">Last full scan signature version</span></span>|
|<span data-ttu-id="2cbf2-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cbf2-175">lastReportedDateTime</span></span>|<span data-ttu-id="2cbf2-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cbf2-176">DateTimeOffset</span></span>|<span data-ttu-id="2cbf2-177">Последнее состояние работоспособности устройства, обнаруженных времени</span><span class="sxs-lookup"><span data-stu-id="2cbf2-177">Last device health status reported time</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cbf2-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="2cbf2-178">Relationships</span></span>
|<span data-ttu-id="2cbf2-179">Связь</span><span class="sxs-lookup"><span data-stu-id="2cbf2-179">Relationship</span></span>|<span data-ttu-id="2cbf2-180">Тип</span><span class="sxs-lookup"><span data-stu-id="2cbf2-180">Type</span></span>|<span data-ttu-id="2cbf2-181">Описание</span><span class="sxs-lookup"><span data-stu-id="2cbf2-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cbf2-182">detectedMalwareState</span><span class="sxs-lookup"><span data-stu-id="2cbf2-182">detectedMalwareState</span></span>|<span data-ttu-id="2cbf2-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2cbf2-183">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="2cbf2-184">Список устройств вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="2cbf2-184">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2cbf2-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cbf2-185">JSON Representation</span></span>
<span data-ttu-id="2cbf2-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cbf2-186">Here is a JSON representation of the resource.</span></span>
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




