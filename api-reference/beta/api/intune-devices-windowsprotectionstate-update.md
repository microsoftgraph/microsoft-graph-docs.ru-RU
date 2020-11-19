---
title: Обновление windowsProtectionState
description: Обновление свойств объекта windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c5317326018404986a63243678455c59302683f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49212694"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="37f46-103">Обновление windowsProtectionState</span><span class="sxs-lookup"><span data-stu-id="37f46-103">Update windowsProtectionState</span></span>

<span data-ttu-id="37f46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37f46-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37f46-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37f46-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37f46-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37f46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37f46-107">Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="37f46-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37f46-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="37f46-108">Prerequisites</span></span>
<span data-ttu-id="37f46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f46-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37f46-111">Permission type</span></span>|<span data-ttu-id="37f46-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="37f46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37f46-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37f46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37f46-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f46-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="37f46-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37f46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37f46-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37f46-116">Not supported.</span></span>|
|<span data-ttu-id="37f46-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="37f46-117">Application</span></span>|<span data-ttu-id="37f46-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f46-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37f46-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37f46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="37f46-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="37f46-120">Request headers</span></span>
|<span data-ttu-id="37f46-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="37f46-121">Header</span></span>|<span data-ttu-id="37f46-122">Значение</span><span class="sxs-lookup"><span data-stu-id="37f46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37f46-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37f46-123">Authorization</span></span>|<span data-ttu-id="37f46-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37f46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37f46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="37f46-125">Accept</span></span>|<span data-ttu-id="37f46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37f46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f46-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37f46-127">Request body</span></span>
<span data-ttu-id="37f46-128">В тексте запроса добавьте представление объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37f46-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="37f46-129">В следующей таблице приведены свойства, необходимые при создании [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span><span class="sxs-lookup"><span data-stu-id="37f46-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="37f46-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="37f46-130">Property</span></span>|<span data-ttu-id="37f46-131">Тип</span><span class="sxs-lookup"><span data-stu-id="37f46-131">Type</span></span>|<span data-ttu-id="37f46-132">Описание</span><span class="sxs-lookup"><span data-stu-id="37f46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37f46-133">id</span><span class="sxs-lookup"><span data-stu-id="37f46-133">id</span></span>|<span data-ttu-id="37f46-134">String</span><span class="sxs-lookup"><span data-stu-id="37f46-134">String</span></span>|<span data-ttu-id="37f46-135">Уникальный идентификатор для объекта состояния защиты устройства.</span><span class="sxs-lookup"><span data-stu-id="37f46-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="37f46-136">Это идентификатор устройства для устройства.</span><span class="sxs-lookup"><span data-stu-id="37f46-136">This is device id of the device</span></span>|
|<span data-ttu-id="37f46-137">малварепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="37f46-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="37f46-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-138">Boolean</span></span>|<span data-ttu-id="37f46-139">Защита от вредоносных программ включена или нет</span><span class="sxs-lookup"><span data-stu-id="37f46-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="37f46-140">девицестате</span><span class="sxs-lookup"><span data-stu-id="37f46-140">deviceState</span></span>|[<span data-ttu-id="37f46-141">виндовсдевицехеалсстате</span><span class="sxs-lookup"><span data-stu-id="37f46-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="37f46-142">Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.).</span><span class="sxs-lookup"><span data-stu-id="37f46-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="37f46-143">Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span><span class="sxs-lookup"><span data-stu-id="37f46-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="37f46-144">реалтимепротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="37f46-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="37f46-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-145">Boolean</span></span>|<span data-ttu-id="37f46-146">Защита в режиме реального времени включена или нет?</span><span class="sxs-lookup"><span data-stu-id="37f46-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="37f46-147">нетворкинспектионсистеменаблед</span><span class="sxs-lookup"><span data-stu-id="37f46-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="37f46-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-148">Boolean</span></span>|<span data-ttu-id="37f46-149">Система проверки сети включена или нет?</span><span class="sxs-lookup"><span data-stu-id="37f46-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="37f46-150">куиккскановердуе</span><span class="sxs-lookup"><span data-stu-id="37f46-150">quickScanOverdue</span></span>|<span data-ttu-id="37f46-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-151">Boolean</span></span>|<span data-ttu-id="37f46-152">Быстрая проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="37f46-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="37f46-153">фуллскановердуе</span><span class="sxs-lookup"><span data-stu-id="37f46-153">fullScanOverdue</span></span>|<span data-ttu-id="37f46-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-154">Boolean</span></span>|<span data-ttu-id="37f46-155">Полная проверка просрочена или нет?</span><span class="sxs-lookup"><span data-stu-id="37f46-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="37f46-156">сигнатуреупдатеовердуе</span><span class="sxs-lookup"><span data-stu-id="37f46-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="37f46-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-157">Boolean</span></span>|<span data-ttu-id="37f46-158">Подпись устарела или нет?</span><span class="sxs-lookup"><span data-stu-id="37f46-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="37f46-159">ребутрекуиред</span><span class="sxs-lookup"><span data-stu-id="37f46-159">rebootRequired</span></span>|<span data-ttu-id="37f46-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-160">Boolean</span></span>|<span data-ttu-id="37f46-161">Требуется перезагрузка или нет?</span><span class="sxs-lookup"><span data-stu-id="37f46-161">Reboot required or not?</span></span>|
|<span data-ttu-id="37f46-162">фуллсканрекуиред</span><span class="sxs-lookup"><span data-stu-id="37f46-162">fullScanRequired</span></span>|<span data-ttu-id="37f46-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-163">Boolean</span></span>|<span data-ttu-id="37f46-164">Необходима полная проверка или нет?</span><span class="sxs-lookup"><span data-stu-id="37f46-164">Full scan required or not?</span></span>|
|<span data-ttu-id="37f46-165">енгиневерсион</span><span class="sxs-lookup"><span data-stu-id="37f46-165">engineVersion</span></span>|<span data-ttu-id="37f46-166">String</span><span class="sxs-lookup"><span data-stu-id="37f46-166">String</span></span>|<span data-ttu-id="37f46-167">Текущая версия модуля Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="37f46-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="37f46-168">сигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="37f46-168">signatureVersion</span></span>|<span data-ttu-id="37f46-169">String</span><span class="sxs-lookup"><span data-stu-id="37f46-169">String</span></span>|<span data-ttu-id="37f46-170">Текущая версия определений вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="37f46-170">Current malware definitions version</span></span>|
|<span data-ttu-id="37f46-171">антималвареверсион</span><span class="sxs-lookup"><span data-stu-id="37f46-171">antiMalwareVersion</span></span>|<span data-ttu-id="37f46-172">String</span><span class="sxs-lookup"><span data-stu-id="37f46-172">String</span></span>|<span data-ttu-id="37f46-173">Текущая версия защиты от вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="37f46-173">Current anti malware version</span></span>|
|<span data-ttu-id="37f46-174">ласткуиккскандатетиме</span><span class="sxs-lookup"><span data-stu-id="37f46-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="37f46-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37f46-175">DateTimeOffset</span></span>|<span data-ttu-id="37f46-176">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="37f46-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="37f46-177">ластфуллскандатетиме</span><span class="sxs-lookup"><span data-stu-id="37f46-177">lastFullScanDateTime</span></span>|<span data-ttu-id="37f46-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37f46-178">DateTimeOffset</span></span>|<span data-ttu-id="37f46-179">Дата и время последнего быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="37f46-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="37f46-180">ласткуиккскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="37f46-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="37f46-181">String</span><span class="sxs-lookup"><span data-stu-id="37f46-181">String</span></span>|<span data-ttu-id="37f46-182">Последняя версия подписи быстрого сканирования</span><span class="sxs-lookup"><span data-stu-id="37f46-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="37f46-183">ластфуллскансигнатуреверсион</span><span class="sxs-lookup"><span data-stu-id="37f46-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="37f46-184">String</span><span class="sxs-lookup"><span data-stu-id="37f46-184">String</span></span>|<span data-ttu-id="37f46-185">Версия последней полной проверки подписи</span><span class="sxs-lookup"><span data-stu-id="37f46-185">Last full scan signature version</span></span>|
|<span data-ttu-id="37f46-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="37f46-186">lastReportedDateTime</span></span>|<span data-ttu-id="37f46-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37f46-187">DateTimeOffset</span></span>|<span data-ttu-id="37f46-188">Последнее состояние работоспособности устройства в отчете о времени</span><span class="sxs-lookup"><span data-stu-id="37f46-188">Last device health status reported time</span></span>|
|<span data-ttu-id="37f46-189">продуктстатус</span><span class="sxs-lookup"><span data-stu-id="37f46-189">productStatus</span></span>|[<span data-ttu-id="37f46-190">виндовсдефендерпродуктстатус</span><span class="sxs-lookup"><span data-stu-id="37f46-190">windowsDefenderProductStatus</span></span>](../resources/intune-devices-windowsdefenderproductstatus.md)|<span data-ttu-id="37f46-191">Состояние продукта антивирусной программы "Защитник Windows".</span><span class="sxs-lookup"><span data-stu-id="37f46-191">Product Status of Windows Defender Antivirus.</span></span> <span data-ttu-id="37f46-192">Возможные значения:,,,,,,,,,,, `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` ,,,,,,, `systemInitiatedCleanInProgress` `samplesPendingSubmission` , `productRunningInEvaluationMode` , `productRunningInNonGenuineMode` , `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` ,,,,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="37f46-192">Possible values are: `noStatus`, `serviceNotRunning`, `serviceStartedWithoutMalwareProtection`, `pendingFullScanDueToThreatAction`, `pendingRebootDueToThreatAction`, `pendingManualStepsDueToThreatAction`, `avSignaturesOutOfDate`, `asSignaturesOutOfDate`, `noQuickScanHappenedForSpecifiedPeriod`, `noFullScanHappenedForSpecifiedPeriod`, `systemInitiatedScanInProgress`, `systemInitiatedCleanInProgress`, `samplesPendingSubmission`, `productRunningInEvaluationMode`, `productRunningInNonGenuineMode`, `productExpired`, `offlineScanRequired`, `serviceShutdownAsPartOfSystemShutdown`, `threatRemediationFailedCritically`, `threatRemediationFailedNonCritically`, `noStatusFlagsSet`, `platformOutOfDate`, `platformUpdateInProgress`, `platformAboutToBeOutdated`, `signatureOrPlatformEndOfLifeIsPastOrIsImpending`, `windowsSModeSignaturesInUseOnNonWin10SInstall`.</span></span>|
|<span data-ttu-id="37f46-193">исвиртуалмачине</span><span class="sxs-lookup"><span data-stu-id="37f46-193">isVirtualMachine</span></span>|<span data-ttu-id="37f46-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-194">Boolean</span></span>|<span data-ttu-id="37f46-195">Указывает, является ли устройство виртуальной машиной.</span><span class="sxs-lookup"><span data-stu-id="37f46-195">Indicates whether the device is a virtual machine.</span></span>|
|<span data-ttu-id="37f46-196">тамперпротектионенаблед</span><span class="sxs-lookup"><span data-stu-id="37f46-196">tamperProtectionEnabled</span></span>|<span data-ttu-id="37f46-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f46-197">Boolean</span></span>|<span data-ttu-id="37f46-198">Указывает, включена ли функция защиты от несанкционированного защитника Windows.</span><span class="sxs-lookup"><span data-stu-id="37f46-198">Indicates whether the Windows Defender tamper protection feature is enabled.</span></span>|



## <a name="response"></a><span data-ttu-id="37f46-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="37f46-199">Response</span></span>
<span data-ttu-id="37f46-200">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37f46-200">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37f46-201">Пример</span><span class="sxs-lookup"><span data-stu-id="37f46-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="37f46-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="37f46-202">Request</span></span>
<span data-ttu-id="37f46-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37f46-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37f46-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="37f46-204">Response</span></span>
<span data-ttu-id="37f46-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37f46-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




