---
title: Создание managedDeviceEncryptionState
description: Создайте новый объект managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c81fca916669c46e853c788d147cdbb69f027ed
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131178"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="a9f45-103">Создание managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="a9f45-103">Create managedDeviceEncryptionState</span></span>

<span data-ttu-id="a9f45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9f45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9f45-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9f45-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9f45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9f45-107">Создайте новый [объект managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="a9f45-107">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9f45-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a9f45-108">Prerequisites</span></span>
<span data-ttu-id="a9f45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9f45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9f45-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9f45-111">Permission type</span></span>|<span data-ttu-id="a9f45-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9f45-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9f45-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9f45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9f45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9f45-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9f45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9f45-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9f45-116">Not supported.</span></span>|
|<span data-ttu-id="a9f45-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a9f45-117">Application</span></span>|<span data-ttu-id="a9f45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9f45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9f45-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9f45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="a9f45-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a9f45-120">Request headers</span></span>
|<span data-ttu-id="a9f45-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9f45-121">Header</span></span>|<span data-ttu-id="a9f45-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a9f45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9f45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9f45-123">Authorization</span></span>|<span data-ttu-id="a9f45-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9f45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9f45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9f45-125">Accept</span></span>|<span data-ttu-id="a9f45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9f45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9f45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9f45-127">Request body</span></span>
<span data-ttu-id="a9f45-128">В теле запроса укажи представление JSON для объекта managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="a9f45-128">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="a9f45-129">В следующей таблице показаны свойства, необходимые при создании managedDeviceEncryptionState.</span><span class="sxs-lookup"><span data-stu-id="a9f45-129">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="a9f45-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9f45-130">Property</span></span>|<span data-ttu-id="a9f45-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a9f45-131">Type</span></span>|<span data-ttu-id="a9f45-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a9f45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9f45-133">id</span><span class="sxs-lookup"><span data-stu-id="a9f45-133">id</span></span>|<span data-ttu-id="a9f45-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a9f45-134">String</span></span>|<span data-ttu-id="a9f45-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a9f45-135">Key of the entity.</span></span>|
|<span data-ttu-id="a9f45-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9f45-136">userPrincipalName</span></span>|<span data-ttu-id="a9f45-137">String</span><span class="sxs-lookup"><span data-stu-id="a9f45-137">String</span></span>|<span data-ttu-id="a9f45-138">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="a9f45-138">User name</span></span>|
|<span data-ttu-id="a9f45-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="a9f45-139">deviceType</span></span>|[<span data-ttu-id="a9f45-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="a9f45-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="a9f45-141">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="a9f45-141">Platform of the device.</span></span> <span data-ttu-id="a9f45-142">Возможные значения: `desktop` `windowsRT` , , , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="a9f45-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a9f45-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="a9f45-143">osVersion</span></span>|<span data-ttu-id="a9f45-144">String</span><span class="sxs-lookup"><span data-stu-id="a9f45-144">String</span></span>|<span data-ttu-id="a9f45-145">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="a9f45-145">Operating system version of the device</span></span>|
|<span data-ttu-id="a9f45-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="a9f45-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="a9f45-147">Строка</span><span class="sxs-lookup"><span data-stu-id="a9f45-147">String</span></span>|<span data-ttu-id="a9f45-148">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="a9f45-148">Device TPM Version</span></span>|
|<span data-ttu-id="a9f45-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="a9f45-149">deviceName</span></span>|<span data-ttu-id="a9f45-150">String</span><span class="sxs-lookup"><span data-stu-id="a9f45-150">String</span></span>|<span data-ttu-id="a9f45-151">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="a9f45-151">Device name</span></span>|
|<span data-ttu-id="a9f45-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="a9f45-152">encryptionReadinessState</span></span>|[<span data-ttu-id="a9f45-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="a9f45-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="a9f45-154">Состояние готовности шифрования.</span><span class="sxs-lookup"><span data-stu-id="a9f45-154">Encryption readiness state.</span></span> <span data-ttu-id="a9f45-155">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="a9f45-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="a9f45-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="a9f45-156">encryptionState</span></span>|[<span data-ttu-id="a9f45-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="a9f45-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="a9f45-158">Состояние шифрования устройств.</span><span class="sxs-lookup"><span data-stu-id="a9f45-158">Device encryption state.</span></span> <span data-ttu-id="a9f45-159">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="a9f45-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="a9f45-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="a9f45-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="a9f45-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a9f45-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a9f45-162">Состояние настройки политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="a9f45-162">Encryption policy setting state.</span></span> <span data-ttu-id="a9f45-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a9f45-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a9f45-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="a9f45-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="a9f45-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="a9f45-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="a9f45-166">Состояние Advanced BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a9f45-166">Advanced BitLocker State.</span></span> <span data-ttu-id="a9f45-167">Возможные значения: `success` `noUserConsent` , , , , , `osVolumeUnprotected` , , `osVolumeTpmRequired` , `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` .</span><span class="sxs-lookup"><span data-stu-id="a9f45-167">Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="a9f45-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="a9f45-168">fileVaultStates</span></span>|[<span data-ttu-id="a9f45-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="a9f45-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="a9f45-170">Состояние FileVault.</span><span class="sxs-lookup"><span data-stu-id="a9f45-170">FileVault State.</span></span> <span data-ttu-id="a9f45-171">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="a9f45-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="a9f45-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="a9f45-172">policyDetails</span></span>|<span data-ttu-id="a9f45-173">[коллекция encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="a9f45-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="a9f45-174">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="a9f45-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="a9f45-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9f45-175">Response</span></span>
<span data-ttu-id="a9f45-176">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a9f45-176">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9f45-177">Пример</span><span class="sxs-lookup"><span data-stu-id="a9f45-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9f45-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9f45-178">Request</span></span>
<span data-ttu-id="a9f45-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9f45-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a9f45-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9f45-180">Response</span></span>
<span data-ttu-id="a9f45-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9f45-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




