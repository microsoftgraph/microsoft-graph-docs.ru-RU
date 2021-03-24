---
title: Обновление windowsProtectionState
description: Обновление свойств объекта WindowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a500c5f1510a28638e58be0ef32d328cc598776
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135833"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="f3620-103">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="f3620-103">Update windowsProtectionState</span></span>

<span data-ttu-id="f3620-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3620-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3620-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3620-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3620-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3620-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3620-107">Обновление свойств объекта [WindowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="f3620-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3620-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3620-108">Prerequisites</span></span>
<span data-ttu-id="f3620-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3620-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3620-111">Permission type</span></span>|<span data-ttu-id="f3620-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3620-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3620-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3620-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3620-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3620-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3620-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3620-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3620-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3620-116">Not supported.</span></span>|
|<span data-ttu-id="f3620-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f3620-117">Application</span></span>|<span data-ttu-id="f3620-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3620-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3620-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3620-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="f3620-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3620-120">Request headers</span></span>
|<span data-ttu-id="f3620-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3620-121">Header</span></span>|<span data-ttu-id="f3620-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3620-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3620-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3620-123">Authorization</span></span>|<span data-ttu-id="f3620-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3620-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3620-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3620-125">Accept</span></span>|<span data-ttu-id="f3620-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3620-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3620-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3620-127">Request body</span></span>
<span data-ttu-id="f3620-128">В теле запроса подарйте представление JSON для [объекта WindowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="f3620-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="f3620-129">В следующей таблице показаны свойства, необходимые при создании [windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)</span><span class="sxs-lookup"><span data-stu-id="f3620-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="f3620-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3620-130">Property</span></span>|<span data-ttu-id="f3620-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3620-131">Type</span></span>|<span data-ttu-id="f3620-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3620-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3620-133">id</span><span class="sxs-lookup"><span data-stu-id="f3620-133">id</span></span>|<span data-ttu-id="f3620-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f3620-134">String</span></span>|<span data-ttu-id="f3620-135">Уникальный идентификатор для объекта защиты от устройства.</span><span class="sxs-lookup"><span data-stu-id="f3620-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="f3620-136">Это id устройства</span><span class="sxs-lookup"><span data-stu-id="f3620-136">This is device id of the device</span></span>|
|<span data-ttu-id="f3620-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f3620-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="f3620-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-138">Boolean</span></span>|<span data-ttu-id="f3620-139">Включено или не включено вредоносное ПО</span><span class="sxs-lookup"><span data-stu-id="f3620-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="f3620-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="f3620-140">deviceState</span></span>|[<span data-ttu-id="f3620-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="f3620-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="f3620-142">Состояние компьютера (например, очистка или ожидание полного сканирования или ожидающих перезагрузки и т.д.).</span><span class="sxs-lookup"><span data-stu-id="f3620-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="f3620-143">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="f3620-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="f3620-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f3620-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="f3620-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-145">Boolean</span></span>|<span data-ttu-id="f3620-146">Включена защита в режиме реального времени или нет?</span><span class="sxs-lookup"><span data-stu-id="f3620-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="f3620-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="f3620-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="f3620-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-148">Boolean</span></span>|<span data-ttu-id="f3620-149">Включена или нет включена система сетевого контроля?</span><span class="sxs-lookup"><span data-stu-id="f3620-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="f3620-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f3620-150">quickScanOverdue</span></span>|<span data-ttu-id="f3620-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-151">Boolean</span></span>|<span data-ttu-id="f3620-152">Быстрое сканирование просрочено или нет?</span><span class="sxs-lookup"><span data-stu-id="f3620-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="f3620-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="f3620-153">fullScanOverdue</span></span>|<span data-ttu-id="f3620-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-154">Boolean</span></span>|<span data-ttu-id="f3620-155">Полная просроченная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="f3620-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="f3620-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="f3620-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="f3620-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-157">Boolean</span></span>|<span data-ttu-id="f3620-158">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="f3620-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="f3620-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="f3620-159">rebootRequired</span></span>|<span data-ttu-id="f3620-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-160">Boolean</span></span>|<span data-ttu-id="f3620-161">Перезагрузка требуется или нет?</span><span class="sxs-lookup"><span data-stu-id="f3620-161">Reboot required or not?</span></span>|
|<span data-ttu-id="f3620-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="f3620-162">fullScanRequired</span></span>|<span data-ttu-id="f3620-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-163">Boolean</span></span>|<span data-ttu-id="f3620-164">Полное сканирование требуется или нет?</span><span class="sxs-lookup"><span data-stu-id="f3620-164">Full scan required or not?</span></span>|
|<span data-ttu-id="f3620-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="f3620-165">engineVersion</span></span>|<span data-ttu-id="f3620-166">Строка</span><span class="sxs-lookup"><span data-stu-id="f3620-166">String</span></span>|<span data-ttu-id="f3620-167">Версия двигателя защиты конечной точки</span><span class="sxs-lookup"><span data-stu-id="f3620-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="f3620-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="f3620-168">signatureVersion</span></span>|<span data-ttu-id="f3620-169">Строка</span><span class="sxs-lookup"><span data-stu-id="f3620-169">String</span></span>|<span data-ttu-id="f3620-170">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="f3620-170">Current malware definitions version</span></span>|
|<span data-ttu-id="f3620-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="f3620-171">antiMalwareVersion</span></span>|<span data-ttu-id="f3620-172">Строка</span><span class="sxs-lookup"><span data-stu-id="f3620-172">String</span></span>|<span data-ttu-id="f3620-173">Текущая версия антивирусных программ</span><span class="sxs-lookup"><span data-stu-id="f3620-173">Current anti malware version</span></span>|
|<span data-ttu-id="f3620-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f3620-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="f3620-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3620-175">DateTimeOffset</span></span>|<span data-ttu-id="f3620-176">Дата последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="f3620-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="f3620-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="f3620-177">lastFullScanDateTime</span></span>|<span data-ttu-id="f3620-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3620-178">DateTimeOffset</span></span>|<span data-ttu-id="f3620-179">Дата последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="f3620-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="f3620-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f3620-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="f3620-181">Строка</span><span class="sxs-lookup"><span data-stu-id="f3620-181">String</span></span>|<span data-ttu-id="f3620-182">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="f3620-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="f3620-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="f3620-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="f3620-184">Строка</span><span class="sxs-lookup"><span data-stu-id="f3620-184">String</span></span>|<span data-ttu-id="f3620-185">Последняя версия подписи полного сканирования</span><span class="sxs-lookup"><span data-stu-id="f3620-185">Last full scan signature version</span></span>|
|<span data-ttu-id="f3620-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3620-186">lastReportedDateTime</span></span>|<span data-ttu-id="f3620-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3620-187">DateTimeOffset</span></span>|<span data-ttu-id="f3620-188">Время последнего состояния состояния устройства</span><span class="sxs-lookup"><span data-stu-id="f3620-188">Last device health status reported time</span></span>|
|<span data-ttu-id="f3620-189">productStatus</span><span class="sxs-lookup"><span data-stu-id="f3620-189">productStatus</span></span>|[<span data-ttu-id="f3620-190">windowsDefenderProductStatus</span><span class="sxs-lookup"><span data-stu-id="f3620-190">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="f3620-191">Состояние продукта Защитник Windows антивируса.</span><span class="sxs-lookup"><span data-stu-id="f3620-191">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="f3620-192">Возможные значения: `noStatus` `serviceNotRunning` , `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` . `windowsSModeSignaturesInUseOnNonWin10SInstall`</span><span class="sxs-lookup"><span data-stu-id="f3620-192">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="f3620-193">isVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="f3620-193">isVirtualMachine</span></span>|<span data-ttu-id="f3620-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-194">Boolean</span></span>|<span data-ttu-id="f3620-195">Указывает, является ли устройство виртуальной машиной.</span><span class="sxs-lookup"><span data-stu-id="f3620-195">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="f3620-196">tamperProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="f3620-196">tamperProtectionEnabled</span></span>|<span data-ttu-id="f3620-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3620-197">Boolean</span></span>|<span data-ttu-id="f3620-198">Указывает, включена ли Защитник Windows защита от взлома.</span><span class="sxs-lookup"><span data-stu-id="f3620-198">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|



## <a name="response"></a><span data-ttu-id="f3620-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3620-199">Response</span></span>
<span data-ttu-id="f3620-200">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f3620-200">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3620-201">Пример</span><span class="sxs-lookup"><span data-stu-id="f3620-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3620-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3620-202">Request</span></span>
<span data-ttu-id="f3620-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3620-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
Content-type: application/json
Content-length: 971

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="f3620-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3620-204">Response</span></span>
<span data-ttu-id="f3620-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3620-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1020

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




