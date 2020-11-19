---
title: Создание Манажеддевицеенкриптионстате
description: Создание нового объекта Манажеддевицеенкриптионстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dd3da3b52746bc9f1c5cc48b7a73b4384b9214b4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287279"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="837fc-103">Создание Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="837fc-103">Create managedDeviceEncryptionState</span></span>

<span data-ttu-id="837fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="837fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="837fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="837fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="837fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="837fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="837fc-107">Создание нового объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="837fc-107">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="837fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="837fc-108">Prerequisites</span></span>
<span data-ttu-id="837fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="837fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="837fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="837fc-111">Permission type</span></span>|<span data-ttu-id="837fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="837fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="837fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="837fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="837fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="837fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="837fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="837fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="837fc-116">Not supported.</span></span>|
|<span data-ttu-id="837fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="837fc-117">Application</span></span>|<span data-ttu-id="837fc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837fc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="837fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="837fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="837fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="837fc-120">Request headers</span></span>
|<span data-ttu-id="837fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="837fc-121">Header</span></span>|<span data-ttu-id="837fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="837fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="837fc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="837fc-123">Authorization</span></span>|<span data-ttu-id="837fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="837fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="837fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="837fc-125">Accept</span></span>|<span data-ttu-id="837fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="837fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="837fc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="837fc-127">Request body</span></span>
<span data-ttu-id="837fc-128">В тексте запроса добавьте представление объекта Манажеддевицеенкриптионстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="837fc-128">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="837fc-129">В следующей таблице приведены свойства, необходимые при создании Манажеддевицеенкриптионстате.</span><span class="sxs-lookup"><span data-stu-id="837fc-129">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="837fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="837fc-130">Property</span></span>|<span data-ttu-id="837fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="837fc-131">Type</span></span>|<span data-ttu-id="837fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="837fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="837fc-133">id</span><span class="sxs-lookup"><span data-stu-id="837fc-133">id</span></span>|<span data-ttu-id="837fc-134">String</span><span class="sxs-lookup"><span data-stu-id="837fc-134">String</span></span>|<span data-ttu-id="837fc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="837fc-135">Key of the entity.</span></span>|
|<span data-ttu-id="837fc-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="837fc-136">userPrincipalName</span></span>|<span data-ttu-id="837fc-137">String</span><span class="sxs-lookup"><span data-stu-id="837fc-137">String</span></span>|<span data-ttu-id="837fc-138">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="837fc-138">User name</span></span>|
|<span data-ttu-id="837fc-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="837fc-139">deviceType</span></span>|[<span data-ttu-id="837fc-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="837fc-140">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="837fc-141">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="837fc-141">Platform of the device.</span></span> <span data-ttu-id="837fc-142">Возможные значения: `desktop` ,,,,,,,,,,,,,,,,,,,,,,,,,,, `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="837fc-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="837fc-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="837fc-143">osVersion</span></span>|<span data-ttu-id="837fc-144">String</span><span class="sxs-lookup"><span data-stu-id="837fc-144">String</span></span>|<span data-ttu-id="837fc-145">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="837fc-145">Operating system version of the device</span></span>|
|<span data-ttu-id="837fc-146">тпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="837fc-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="837fc-147">String</span><span class="sxs-lookup"><span data-stu-id="837fc-147">String</span></span>|<span data-ttu-id="837fc-148">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="837fc-148">Device TPM Version</span></span>|
|<span data-ttu-id="837fc-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="837fc-149">deviceName</span></span>|<span data-ttu-id="837fc-150">String</span><span class="sxs-lookup"><span data-stu-id="837fc-150">String</span></span>|<span data-ttu-id="837fc-151">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="837fc-151">Device name</span></span>|
|<span data-ttu-id="837fc-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="837fc-152">encryptionReadinessState</span></span>|[<span data-ttu-id="837fc-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="837fc-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="837fc-154">Состояние готовности к шифрованию.</span><span class="sxs-lookup"><span data-stu-id="837fc-154">Encryption readiness state.</span></span> <span data-ttu-id="837fc-155">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="837fc-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="837fc-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="837fc-156">encryptionState</span></span>|[<span data-ttu-id="837fc-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="837fc-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="837fc-158">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="837fc-158">Device encryption state.</span></span> <span data-ttu-id="837fc-159">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="837fc-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="837fc-160">енкриптионполицисеттингстате</span><span class="sxs-lookup"><span data-stu-id="837fc-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="837fc-161">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="837fc-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="837fc-162">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="837fc-162">Encryption policy setting state.</span></span> <span data-ttu-id="837fc-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="837fc-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="837fc-164">адванцедбитлоккерстатес</span><span class="sxs-lookup"><span data-stu-id="837fc-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="837fc-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="837fc-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="837fc-166">Расширенное состояние BitLocker.</span><span class="sxs-lookup"><span data-stu-id="837fc-166">Advanced BitLocker State.</span></span> <span data-ttu-id="837fc-167">Возможные значения: `success` , `noUserConsent` ,,,,, `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` ,,, `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` ,,, `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` , `windowsRecoveryEnvironmentNotConfigured` , `tpmNotAvailable` , `tpmNotReady` , `networkError` .</span><span class="sxs-lookup"><span data-stu-id="837fc-167">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="837fc-168">филеваултстатес</span><span class="sxs-lookup"><span data-stu-id="837fc-168">fileVaultStates</span></span>|[<span data-ttu-id="837fc-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="837fc-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="837fc-170">Состояние Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="837fc-170">FileVault State.</span></span> <span data-ttu-id="837fc-171">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="837fc-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="837fc-172">полицидетаилс</span><span class="sxs-lookup"><span data-stu-id="837fc-172">policyDetails</span></span>|<span data-ttu-id="837fc-173">Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="837fc-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="837fc-174">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="837fc-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="837fc-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="837fc-175">Response</span></span>
<span data-ttu-id="837fc-176">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="837fc-176">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="837fc-177">Пример</span><span class="sxs-lookup"><span data-stu-id="837fc-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="837fc-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="837fc-178">Request</span></span>
<span data-ttu-id="837fc-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="837fc-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="837fc-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="837fc-180">Response</span></span>
<span data-ttu-id="837fc-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="837fc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




