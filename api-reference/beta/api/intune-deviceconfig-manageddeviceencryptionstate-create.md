---
title: Создание Манажеддевицеенкриптионстате
description: Создание нового объекта Манажеддевицеенкриптионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff5908b41972dfb0d68f4b1e3eb1da68b2b82361
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448608"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="00756-103">Создание Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="00756-103">Create managedDeviceEncryptionState</span></span>

<span data-ttu-id="00756-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="00756-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00756-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00756-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00756-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00756-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00756-107">Создание нового объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="00756-107">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00756-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00756-108">Prerequisites</span></span>
<span data-ttu-id="00756-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00756-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00756-111">Permission type</span></span>|<span data-ttu-id="00756-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00756-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00756-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00756-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00756-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00756-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00756-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00756-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00756-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00756-116">Not supported.</span></span>|
|<span data-ttu-id="00756-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00756-117">Application</span></span>|<span data-ttu-id="00756-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00756-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00756-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00756-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="00756-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00756-120">Request headers</span></span>
|<span data-ttu-id="00756-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00756-121">Header</span></span>|<span data-ttu-id="00756-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00756-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00756-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00756-123">Authorization</span></span>|<span data-ttu-id="00756-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00756-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00756-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00756-125">Accept</span></span>|<span data-ttu-id="00756-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00756-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00756-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00756-127">Request body</span></span>
<span data-ttu-id="00756-128">В тексте запроса добавьте представление объекта Манажеддевицеенкриптионстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00756-128">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="00756-129">В следующей таблице приведены свойства, необходимые при создании Манажеддевицеенкриптионстате.</span><span class="sxs-lookup"><span data-stu-id="00756-129">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="00756-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00756-130">Property</span></span>|<span data-ttu-id="00756-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00756-131">Type</span></span>|<span data-ttu-id="00756-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00756-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00756-133">id</span><span class="sxs-lookup"><span data-stu-id="00756-133">id</span></span>|<span data-ttu-id="00756-134">Строка</span><span class="sxs-lookup"><span data-stu-id="00756-134">String</span></span>|<span data-ttu-id="00756-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="00756-135">Key of the entity.</span></span>|
|<span data-ttu-id="00756-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00756-136">userPrincipalName</span></span>|<span data-ttu-id="00756-137">String</span><span class="sxs-lookup"><span data-stu-id="00756-137">String</span></span>|<span data-ttu-id="00756-138">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="00756-138">User name</span></span>|
|<span data-ttu-id="00756-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="00756-139">deviceType</span></span>|[<span data-ttu-id="00756-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="00756-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="00756-141">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="00756-141">Platform of the device.</span></span> <span data-ttu-id="00756-142">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `iSocConsumer` `unknown`,,,,,,,,,,,,,,,,,,,,,,,,. `winEmbedded` `iPhone` `iPad` `iPod` `android`</span><span class="sxs-lookup"><span data-stu-id="00756-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="00756-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="00756-143">osVersion</span></span>|<span data-ttu-id="00756-144">String</span><span class="sxs-lookup"><span data-stu-id="00756-144">String</span></span>|<span data-ttu-id="00756-145">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="00756-145">Operating system version of the device</span></span>|
|<span data-ttu-id="00756-146">тпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="00756-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="00756-147">String</span><span class="sxs-lookup"><span data-stu-id="00756-147">String</span></span>|<span data-ttu-id="00756-148">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="00756-148">Device TPM Version</span></span>|
|<span data-ttu-id="00756-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="00756-149">deviceName</span></span>|<span data-ttu-id="00756-150">String</span><span class="sxs-lookup"><span data-stu-id="00756-150">String</span></span>|<span data-ttu-id="00756-151">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="00756-151">Device name</span></span>|
|<span data-ttu-id="00756-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="00756-152">encryptionReadinessState</span></span>|[<span data-ttu-id="00756-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="00756-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="00756-154">Состояние готовности к шифрованию.</span><span class="sxs-lookup"><span data-stu-id="00756-154">Encryption readiness state.</span></span> <span data-ttu-id="00756-155">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="00756-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="00756-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="00756-156">encryptionState</span></span>|[<span data-ttu-id="00756-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="00756-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="00756-158">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="00756-158">Device encryption state.</span></span> <span data-ttu-id="00756-159">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="00756-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="00756-160">енкриптионполицисеттингстате</span><span class="sxs-lookup"><span data-stu-id="00756-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="00756-161">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="00756-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="00756-162">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="00756-162">Encryption policy setting state.</span></span> <span data-ttu-id="00756-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="00756-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="00756-164">адванцедбитлоккерстатес</span><span class="sxs-lookup"><span data-stu-id="00756-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="00756-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="00756-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="00756-166">Расширенное состояние BitLocker.</span><span class="sxs-lookup"><span data-stu-id="00756-166">Advanced BitLocker State.</span></span> <span data-ttu-id="00756-167">Возможные значения: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`,. `networkError`</span><span class="sxs-lookup"><span data-stu-id="00756-167">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="00756-168">филеваултстатес</span><span class="sxs-lookup"><span data-stu-id="00756-168">fileVaultStates</span></span>|[<span data-ttu-id="00756-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="00756-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="00756-170">Состояние Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="00756-170">FileVault State.</span></span> <span data-ttu-id="00756-171">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="00756-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="00756-172">полицидетаилс</span><span class="sxs-lookup"><span data-stu-id="00756-172">policyDetails</span></span>|<span data-ttu-id="00756-173">Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="00756-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="00756-174">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="00756-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="00756-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="00756-175">Response</span></span>
<span data-ttu-id="00756-176">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00756-176">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00756-177">Пример</span><span class="sxs-lookup"><span data-stu-id="00756-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="00756-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="00756-178">Request</span></span>
<span data-ttu-id="00756-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00756-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
Content-type: application/json
Content-length: 704

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="00756-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="00756-180">Response</span></span>
<span data-ttu-id="00756-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00756-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
  "userPrincipalName": "User Principal Name value",
  "deviceType": "windowsRT",
  "osVersion": "Os Version value",
  "tpmSpecificationVersion": "Tpm Specification Version value",
  "deviceName": "Device Name value",
  "encryptionReadinessState": "ready",
  "encryptionState": "encrypted",
  "encryptionPolicySettingState": "notApplicable",
  "advancedBitLockerStates": "noUserConsent",
  "fileVaultStates": "driveEncryptedByUser",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```





