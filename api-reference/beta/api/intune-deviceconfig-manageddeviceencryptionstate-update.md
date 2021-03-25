---
title: Обновление managedDeviceEncryptionState
description: Обновление свойств объекта managedDeviceEncryptionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8dd4c44cf373b5aa5ac20208308394ede5fe2d05
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155136"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="eda58-103">Обновление managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="eda58-103">Update managedDeviceEncryptionState</span></span>

<span data-ttu-id="eda58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eda58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eda58-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eda58-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eda58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eda58-107">Обновление свойств объекта [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="eda58-107">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eda58-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eda58-108">Prerequisites</span></span>
<span data-ttu-id="eda58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eda58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eda58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eda58-111">Permission type</span></span>|<span data-ttu-id="eda58-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eda58-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eda58-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eda58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eda58-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda58-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eda58-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eda58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eda58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eda58-116">Not supported.</span></span>|
|<span data-ttu-id="eda58-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="eda58-117">Application</span></span>|<span data-ttu-id="eda58-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eda58-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eda58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eda58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="eda58-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eda58-120">Request headers</span></span>
|<span data-ttu-id="eda58-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eda58-121">Header</span></span>|<span data-ttu-id="eda58-122">Значение</span><span class="sxs-lookup"><span data-stu-id="eda58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eda58-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eda58-123">Authorization</span></span>|<span data-ttu-id="eda58-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eda58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eda58-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eda58-125">Accept</span></span>|<span data-ttu-id="eda58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eda58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eda58-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eda58-127">Request body</span></span>
<span data-ttu-id="eda58-128">В теле запроса укажи представление JSON для [объекта managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="eda58-128">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="eda58-129">В следующей таблице показаны свойства, необходимые при создании [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="eda58-129">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="eda58-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="eda58-130">Property</span></span>|<span data-ttu-id="eda58-131">Тип</span><span class="sxs-lookup"><span data-stu-id="eda58-131">Type</span></span>|<span data-ttu-id="eda58-132">Описание</span><span class="sxs-lookup"><span data-stu-id="eda58-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eda58-133">id</span><span class="sxs-lookup"><span data-stu-id="eda58-133">id</span></span>|<span data-ttu-id="eda58-134">Строка</span><span class="sxs-lookup"><span data-stu-id="eda58-134">String</span></span>|<span data-ttu-id="eda58-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eda58-135">Key of the entity.</span></span>|
|<span data-ttu-id="eda58-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eda58-136">userPrincipalName</span></span>|<span data-ttu-id="eda58-137">String</span><span class="sxs-lookup"><span data-stu-id="eda58-137">String</span></span>|<span data-ttu-id="eda58-138">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="eda58-138">User name</span></span>|
|<span data-ttu-id="eda58-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="eda58-139">deviceType</span></span>|[<span data-ttu-id="eda58-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="eda58-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="eda58-141">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="eda58-141">Platform of the device.</span></span> <span data-ttu-id="eda58-142">Возможные значения: `desktop` `windowsRT` , , , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="eda58-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="eda58-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="eda58-143">osVersion</span></span>|<span data-ttu-id="eda58-144">String</span><span class="sxs-lookup"><span data-stu-id="eda58-144">String</span></span>|<span data-ttu-id="eda58-145">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="eda58-145">Operating system version of the device</span></span>|
|<span data-ttu-id="eda58-146">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="eda58-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="eda58-147">Строка</span><span class="sxs-lookup"><span data-stu-id="eda58-147">String</span></span>|<span data-ttu-id="eda58-148">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="eda58-148">Device TPM Version</span></span>|
|<span data-ttu-id="eda58-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="eda58-149">deviceName</span></span>|<span data-ttu-id="eda58-150">String</span><span class="sxs-lookup"><span data-stu-id="eda58-150">String</span></span>|<span data-ttu-id="eda58-151">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="eda58-151">Device name</span></span>|
|<span data-ttu-id="eda58-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="eda58-152">encryptionReadinessState</span></span>|[<span data-ttu-id="eda58-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="eda58-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="eda58-154">Состояние готовности шифрования.</span><span class="sxs-lookup"><span data-stu-id="eda58-154">Encryption readiness state.</span></span> <span data-ttu-id="eda58-155">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="eda58-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="eda58-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="eda58-156">encryptionState</span></span>|[<span data-ttu-id="eda58-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="eda58-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="eda58-158">Состояние шифрования устройств.</span><span class="sxs-lookup"><span data-stu-id="eda58-158">Device encryption state.</span></span> <span data-ttu-id="eda58-159">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="eda58-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="eda58-160">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="eda58-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="eda58-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="eda58-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="eda58-162">Состояние настройки политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="eda58-162">Encryption policy setting state.</span></span> <span data-ttu-id="eda58-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="eda58-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="eda58-164">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="eda58-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="eda58-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="eda58-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="eda58-166">Состояние Advanced BitLocker.</span><span class="sxs-lookup"><span data-stu-id="eda58-166">Advanced BitLocker State.</span></span> <span data-ttu-id="eda58-167">Возможные значения: `success` `noUserConsent` , , , , , `osVolumeUnprotected` , , `osVolumeTpmRequired` , `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` .</span><span class="sxs-lookup"><span data-stu-id="eda58-167">Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="eda58-168">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="eda58-168">fileVaultStates</span></span>|[<span data-ttu-id="eda58-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="eda58-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="eda58-170">Состояние FileVault.</span><span class="sxs-lookup"><span data-stu-id="eda58-170">FileVault State.</span></span> <span data-ttu-id="eda58-171">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="eda58-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="eda58-172">policyDetails</span><span class="sxs-lookup"><span data-stu-id="eda58-172">policyDetails</span></span>|<span data-ttu-id="eda58-173">[коллекция encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="eda58-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="eda58-174">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="eda58-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="eda58-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda58-175">Response</span></span>
<span data-ttu-id="eda58-176">В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="eda58-176">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eda58-177">Пример</span><span class="sxs-lookup"><span data-stu-id="eda58-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="eda58-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="eda58-178">Request</span></span>
<span data-ttu-id="eda58-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eda58-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
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

### <a name="response"></a><span data-ttu-id="eda58-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="eda58-180">Response</span></span>
<span data-ttu-id="eda58-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eda58-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




