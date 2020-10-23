---
title: Обновление Манажеддевицеенкриптионстате
description: Обновление свойств объекта Манажеддевицеенкриптионстате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab37f8168982025d2c4dc4e2f9ead4ed96b6dcfd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704289"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="900bf-103">Обновление Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="900bf-103">Update managedDeviceEncryptionState</span></span>

<span data-ttu-id="900bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="900bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="900bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="900bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="900bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="900bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="900bf-107">Обновление свойств объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="900bf-107">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="900bf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="900bf-108">Prerequisites</span></span>
<span data-ttu-id="900bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="900bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="900bf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="900bf-111">Permission type</span></span>|<span data-ttu-id="900bf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="900bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="900bf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="900bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="900bf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="900bf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="900bf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="900bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="900bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="900bf-116">Not supported.</span></span>|
|<span data-ttu-id="900bf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="900bf-117">Application</span></span>|<span data-ttu-id="900bf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="900bf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="900bf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="900bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="900bf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="900bf-120">Request headers</span></span>
|<span data-ttu-id="900bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="900bf-121">Header</span></span>|<span data-ttu-id="900bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="900bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="900bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="900bf-123">Authorization</span></span>|<span data-ttu-id="900bf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="900bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="900bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="900bf-125">Accept</span></span>|<span data-ttu-id="900bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="900bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="900bf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="900bf-127">Request body</span></span>
<span data-ttu-id="900bf-128">В тексте запроса добавьте представление объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="900bf-128">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="900bf-129">В следующей таблице приведены свойства, необходимые при создании [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span><span class="sxs-lookup"><span data-stu-id="900bf-129">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="900bf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="900bf-130">Property</span></span>|<span data-ttu-id="900bf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="900bf-131">Type</span></span>|<span data-ttu-id="900bf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="900bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="900bf-133">id</span><span class="sxs-lookup"><span data-stu-id="900bf-133">id</span></span>|<span data-ttu-id="900bf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="900bf-134">String</span></span>|<span data-ttu-id="900bf-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="900bf-135">Key of the entity.</span></span>|
|<span data-ttu-id="900bf-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="900bf-136">userPrincipalName</span></span>|<span data-ttu-id="900bf-137">String</span><span class="sxs-lookup"><span data-stu-id="900bf-137">String</span></span>|<span data-ttu-id="900bf-138">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="900bf-138">User name</span></span>|
|<span data-ttu-id="900bf-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="900bf-139">deviceType</span></span>|[<span data-ttu-id="900bf-140">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="900bf-140">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="900bf-141">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="900bf-141">Platform of the device.</span></span> <span data-ttu-id="900bf-142">Возможные значения: `desktop` ,,,,,,,,,,,,,,,,,,,,,,,,,,, `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="900bf-142">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="900bf-143">osVersion</span><span class="sxs-lookup"><span data-stu-id="900bf-143">osVersion</span></span>|<span data-ttu-id="900bf-144">String</span><span class="sxs-lookup"><span data-stu-id="900bf-144">String</span></span>|<span data-ttu-id="900bf-145">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="900bf-145">Operating system version of the device</span></span>|
|<span data-ttu-id="900bf-146">тпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="900bf-146">tpmSpecificationVersion</span></span>|<span data-ttu-id="900bf-147">Строка</span><span class="sxs-lookup"><span data-stu-id="900bf-147">String</span></span>|<span data-ttu-id="900bf-148">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="900bf-148">Device TPM Version</span></span>|
|<span data-ttu-id="900bf-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="900bf-149">deviceName</span></span>|<span data-ttu-id="900bf-150">String</span><span class="sxs-lookup"><span data-stu-id="900bf-150">String</span></span>|<span data-ttu-id="900bf-151">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="900bf-151">Device name</span></span>|
|<span data-ttu-id="900bf-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="900bf-152">encryptionReadinessState</span></span>|[<span data-ttu-id="900bf-153">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="900bf-153">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="900bf-154">Состояние готовности к шифрованию.</span><span class="sxs-lookup"><span data-stu-id="900bf-154">Encryption readiness state.</span></span> <span data-ttu-id="900bf-155">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="900bf-155">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="900bf-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="900bf-156">encryptionState</span></span>|[<span data-ttu-id="900bf-157">encryptionState</span><span class="sxs-lookup"><span data-stu-id="900bf-157">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="900bf-158">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="900bf-158">Device encryption state.</span></span> <span data-ttu-id="900bf-159">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="900bf-159">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="900bf-160">енкриптионполицисеттингстате</span><span class="sxs-lookup"><span data-stu-id="900bf-160">encryptionPolicySettingState</span></span>|[<span data-ttu-id="900bf-161">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="900bf-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="900bf-162">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="900bf-162">Encryption policy setting state.</span></span> <span data-ttu-id="900bf-163">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="900bf-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="900bf-164">адванцедбитлоккерстатес</span><span class="sxs-lookup"><span data-stu-id="900bf-164">advancedBitLockerStates</span></span>|[<span data-ttu-id="900bf-165">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="900bf-165">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="900bf-166">Расширенное состояние BitLocker.</span><span class="sxs-lookup"><span data-stu-id="900bf-166">Advanced BitLocker State.</span></span> <span data-ttu-id="900bf-167">Возможные значения: `success` , `noUserConsent` ,,,,, `osVolumeEncryptionMethodMismatch` `osVolumeTpmRequired` `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` ,,, `osVolumeTpmPinStartupKeyRequired` `osVolumeUnprotected` `recoveryKeyBackupFailed` ,,, `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` , `windowsRecoveryEnvironmentNotConfigured` , `tpmNotAvailable` , `tpmNotReady` , `networkError` .</span><span class="sxs-lookup"><span data-stu-id="900bf-167">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="900bf-168">филеваултстатес</span><span class="sxs-lookup"><span data-stu-id="900bf-168">fileVaultStates</span></span>|[<span data-ttu-id="900bf-169">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="900bf-169">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="900bf-170">Состояние Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="900bf-170">FileVault State.</span></span> <span data-ttu-id="900bf-171">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="900bf-171">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="900bf-172">полицидетаилс</span><span class="sxs-lookup"><span data-stu-id="900bf-172">policyDetails</span></span>|<span data-ttu-id="900bf-173">Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="900bf-173">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="900bf-174">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="900bf-174">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="900bf-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="900bf-175">Response</span></span>
<span data-ttu-id="900bf-176">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="900bf-176">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="900bf-177">Пример</span><span class="sxs-lookup"><span data-stu-id="900bf-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="900bf-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="900bf-178">Request</span></span>
<span data-ttu-id="900bf-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="900bf-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="900bf-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="900bf-180">Response</span></span>
<span data-ttu-id="900bf-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="900bf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





