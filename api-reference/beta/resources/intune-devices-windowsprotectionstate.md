---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2651aa9fad173654d8fff554bdf89f7ab36da14
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207563"
---
# <a name="windowsprotectionstate-resource-type"></a><span data-ttu-id="c3716-103">Тип ресурса windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c3716-103">windowsProtectionState resource type</span></span>

<span data-ttu-id="c3716-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3716-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3716-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3716-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3716-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3716-107">Объект состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="c3716-107">Device protection status entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c3716-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c3716-108">Methods</span></span>
|<span data-ttu-id="c3716-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c3716-109">Method</span></span>|<span data-ttu-id="c3716-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3716-110">Return Type</span></span>|<span data-ttu-id="c3716-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3716-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3716-112">Получение windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c3716-112">Get windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-get.md)|[<span data-ttu-id="c3716-113">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c3716-113">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="c3716-114">Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c3716-114">Read properties and relationships of the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|
|[<span data-ttu-id="c3716-115">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c3716-115">Update windowsProtectionState</span></span>](../api/intune-devices-windowsprotectionstate-update.md)|[<span data-ttu-id="c3716-116">windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="c3716-116">windowsProtectionState</span></span>](../resources/intune-devices-windowsprotectionstate.md)|<span data-ttu-id="c3716-117">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="c3716-117">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3716-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3716-118">Properties</span></span>
|<span data-ttu-id="c3716-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3716-119">Property</span></span>|<span data-ttu-id="c3716-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c3716-120">Type</span></span>|<span data-ttu-id="c3716-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3716-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3716-122">id</span><span class="sxs-lookup"><span data-stu-id="c3716-122">id</span></span>|<span data-ttu-id="c3716-123">String</span><span class="sxs-lookup"><span data-stu-id="c3716-123">String</span></span>|<span data-ttu-id="c3716-124">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="c3716-124">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="c3716-125">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="c3716-125">This is device id of the device</span></span>|
|<span data-ttu-id="c3716-126">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="c3716-126">malwareProtectionEnabled</span></span>|<span data-ttu-id="c3716-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-127">Boolean</span></span>|<span data-ttu-id="c3716-128">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="c3716-128">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="c3716-129">девицестате</span><span class="sxs-lookup"><span data-stu-id="c3716-129">deviceState</span></span>|[<span data-ttu-id="c3716-130">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="c3716-130">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="c3716-131">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="c3716-131">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="c3716-132">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="c3716-132">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="c3716-133">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="c3716-133">realTimeProtectionEnabled</span></span>|<span data-ttu-id="c3716-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-134">Boolean</span></span>|<span data-ttu-id="c3716-135">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="c3716-135">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="c3716-136">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="c3716-136">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="c3716-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-137">Boolean</span></span>|<span data-ttu-id="c3716-138">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="c3716-138">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="c3716-139">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="c3716-139">quickScanOverdue</span></span>|<span data-ttu-id="c3716-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-140">Boolean</span></span>|<span data-ttu-id="c3716-141">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="c3716-141">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="c3716-142">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="c3716-142">fullScanOverdue</span></span>|<span data-ttu-id="c3716-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-143">Boolean</span></span>|<span data-ttu-id="c3716-144">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="c3716-144">Full scan overdue or not?</span></span>|
|<span data-ttu-id="c3716-145">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="c3716-145">signatureUpdateOverdue</span></span>|<span data-ttu-id="c3716-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-146">Boolean</span></span>|<span data-ttu-id="c3716-147">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="c3716-147">Signature out of date or not?</span></span>|
|<span data-ttu-id="c3716-148">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="c3716-148">rebootRequired</span></span>|<span data-ttu-id="c3716-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-149">Boolean</span></span>|<span data-ttu-id="c3716-150">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="c3716-150">Reboot required or not?</span></span>|
|<span data-ttu-id="c3716-151">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="c3716-151">fullScanRequired</span></span>|<span data-ttu-id="c3716-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-152">Boolean</span></span>|<span data-ttu-id="c3716-153">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="c3716-153">Full scan required or not?</span></span>|
|<span data-ttu-id="c3716-154">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="c3716-154">engineVersion</span></span>|<span data-ttu-id="c3716-155">String</span><span class="sxs-lookup"><span data-stu-id="c3716-155">String</span></span>|<span data-ttu-id="c3716-156">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="c3716-156">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="c3716-157">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="c3716-157">signatureVersion</span></span>|<span data-ttu-id="c3716-158">String</span><span class="sxs-lookup"><span data-stu-id="c3716-158">String</span></span>|<span data-ttu-id="c3716-159">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="c3716-159">Current malware definitions version</span></span>|
|<span data-ttu-id="c3716-160">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="c3716-160">antiMalwareVersion</span></span>|<span data-ttu-id="c3716-161">String</span><span class="sxs-lookup"><span data-stu-id="c3716-161">String</span></span>|<span data-ttu-id="c3716-162">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="c3716-162">Current anti malware version</span></span>|
|<span data-ttu-id="c3716-163">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="c3716-163">lastQuickScanDateTime</span></span>|<span data-ttu-id="c3716-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3716-164">DateTimeOffset</span></span>|<span data-ttu-id="c3716-165">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="c3716-165">Last quick scan datetime</span></span>|
|<span data-ttu-id="c3716-166">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="c3716-166">lastFullScanDateTime</span></span>|<span data-ttu-id="c3716-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3716-167">DateTimeOffset</span></span>|<span data-ttu-id="c3716-168">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="c3716-168">Last quick scan datetime</span></span>|
|<span data-ttu-id="c3716-169">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="c3716-169">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="c3716-170">String</span><span class="sxs-lookup"><span data-stu-id="c3716-170">String</span></span>|<span data-ttu-id="c3716-171">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="c3716-171">Last quick scan signature version</span></span>|
|<span data-ttu-id="c3716-172">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="c3716-172">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="c3716-173">String</span><span class="sxs-lookup"><span data-stu-id="c3716-173">String</span></span>|<span data-ttu-id="c3716-174">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="c3716-174">Last full scan signature version</span></span>|
|<span data-ttu-id="c3716-175">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3716-175">lastReportedDateTime</span></span>|<span data-ttu-id="c3716-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3716-176">DateTimeOffset</span></span>|<span data-ttu-id="c3716-177">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="c3716-177">Last device health status reported time</span></span>|
|<span data-ttu-id="c3716-178">продуктстатус</span><span class="sxs-lookup"><span data-stu-id="c3716-178">productStatus</span></span>|[<span data-ttu-id="c3716-179">виндовсдефендерпродуктстатус</span><span class="sxs-lookup"><span data-stu-id="c3716-179">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="c3716-180">Состояние продукта антивирусной программы "Защитник Windows".</span><span class="sxs-lookup"><span data-stu-id="c3716-180">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="c3716-181">Возможные значения:,,,,,,,,,,, `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` ,,,,,,, `systemInitiatedCleanInProgress` `samplesPendingSubmission` , `productRunningInEvaluationMode` , `productRunningInNonGenuineMode` , `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` ,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="c3716-181">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="c3716-182">исвиртуалмачине</span><span class="sxs-lookup"><span data-stu-id="c3716-182">isVirtualMachine</span></span>|<span data-ttu-id="c3716-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-183">Boolean</span></span>|<span data-ttu-id="c3716-184">Указывает, является ли устройство виртуальной машиной.</span><span class="sxs-lookup"><span data-stu-id="c3716-184">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="c3716-185">тамперпротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="c3716-185">tamperProtectionEnabled</span></span>|<span data-ttu-id="c3716-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3716-186">Boolean</span></span>|<span data-ttu-id="c3716-187">Указывает, включена ли функция защиты от несанкционированного защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="c3716-187">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3716-188">Связи</span><span class="sxs-lookup"><span data-stu-id="c3716-188">Relationships</span></span>
|<span data-ttu-id="c3716-189">Связь</span><span class="sxs-lookup"><span data-stu-id="c3716-189">Relationship</span></span>|<span data-ttu-id="c3716-190">Тип</span><span class="sxs-lookup"><span data-stu-id="c3716-190">Type</span></span>|<span data-ttu-id="c3716-191">Описание</span><span class="sxs-lookup"><span data-stu-id="c3716-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3716-192">детектедмалварестате</span><span class="sxs-lookup"><span data-stu-id="c3716-192">detectedMalwareState</span></span>|<span data-ttu-id="c3716-193">Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)</span><span class="sxs-lookup"><span data-stu-id="c3716-193">[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) collection</span></span>|<span data-ttu-id="c3716-194">Список вредоносных программ для устройств</span><span class="sxs-lookup"><span data-stu-id="c3716-194">Device malware list</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3716-195">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3716-195">JSON Representation</span></span>
<span data-ttu-id="c3716-196">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3716-196">Here is a JSON representation of the resource.</span></span>
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
  "lastReportedDateTime": "String (timestamp)",
  "productStatus": "String",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




