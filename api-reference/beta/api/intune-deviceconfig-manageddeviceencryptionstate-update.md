---
title: Обновление Манажеддевицеенкриптионстате
description: Обновление свойств объекта Манажеддевицеенкриптионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: def987033cc6a1ea34159f5de9038d0f2c0ceefb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946615"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="32083-103">Обновление Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="32083-103">Update managedDeviceEncryptionState</span></span>

> <span data-ttu-id="32083-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32083-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32083-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32083-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32083-106">Обновление свойств объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="32083-106">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32083-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="32083-107">Prerequisites</span></span>
<span data-ttu-id="32083-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32083-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32083-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32083-110">Permission type</span></span>|<span data-ttu-id="32083-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32083-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32083-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32083-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32083-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32083-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32083-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32083-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32083-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32083-115">Not supported.</span></span>|
|<span data-ttu-id="32083-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32083-116">Application</span></span>|<span data-ttu-id="32083-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32083-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32083-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32083-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="32083-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32083-119">Request headers</span></span>
|<span data-ttu-id="32083-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32083-120">Header</span></span>|<span data-ttu-id="32083-121">Значение</span><span class="sxs-lookup"><span data-stu-id="32083-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32083-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32083-122">Authorization</span></span>|<span data-ttu-id="32083-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32083-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32083-124">Accept</span><span class="sxs-lookup"><span data-stu-id="32083-124">Accept</span></span>|<span data-ttu-id="32083-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32083-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32083-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32083-126">Request body</span></span>
<span data-ttu-id="32083-127">В тексте запроса добавьте представление объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32083-127">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="32083-128">В следующей таблице приведены свойства, необходимые при создании [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span><span class="sxs-lookup"><span data-stu-id="32083-128">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="32083-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="32083-129">Property</span></span>|<span data-ttu-id="32083-130">Тип</span><span class="sxs-lookup"><span data-stu-id="32083-130">Type</span></span>|<span data-ttu-id="32083-131">Описание</span><span class="sxs-lookup"><span data-stu-id="32083-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32083-132">id</span><span class="sxs-lookup"><span data-stu-id="32083-132">id</span></span>|<span data-ttu-id="32083-133">Строка</span><span class="sxs-lookup"><span data-stu-id="32083-133">String</span></span>|<span data-ttu-id="32083-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="32083-134">Key of the entity.</span></span>|
|<span data-ttu-id="32083-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="32083-135">userPrincipalName</span></span>|<span data-ttu-id="32083-136">String</span><span class="sxs-lookup"><span data-stu-id="32083-136">String</span></span>|<span data-ttu-id="32083-137">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="32083-137">User name</span></span>|
|<span data-ttu-id="32083-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="32083-138">deviceType</span></span>|[<span data-ttu-id="32083-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="32083-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="32083-140">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="32083-140">Platform of the device.</span></span> <span data-ttu-id="32083-141">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="32083-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="32083-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="32083-142">osVersion</span></span>|<span data-ttu-id="32083-143">String</span><span class="sxs-lookup"><span data-stu-id="32083-143">String</span></span>|<span data-ttu-id="32083-144">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="32083-144">Operating system version of the device</span></span>|
|<span data-ttu-id="32083-145">ТпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="32083-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="32083-146">String</span><span class="sxs-lookup"><span data-stu-id="32083-146">String</span></span>|<span data-ttu-id="32083-147">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="32083-147">Device TPM Version</span></span>|
|<span data-ttu-id="32083-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="32083-148">deviceName</span></span>|<span data-ttu-id="32083-149">String</span><span class="sxs-lookup"><span data-stu-id="32083-149">String</span></span>|<span data-ttu-id="32083-150">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="32083-150">Device name</span></span>|
|<span data-ttu-id="32083-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="32083-151">encryptionReadinessState</span></span>|[<span data-ttu-id="32083-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="32083-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="32083-153">Состояние готовности к шифрованию.</span><span class="sxs-lookup"><span data-stu-id="32083-153">Encryption readiness state.</span></span> <span data-ttu-id="32083-154">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="32083-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="32083-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="32083-155">encryptionState</span></span>|[<span data-ttu-id="32083-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="32083-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="32083-157">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="32083-157">Device encryption state.</span></span> <span data-ttu-id="32083-158">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="32083-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="32083-159">Енкриптионполицисеттингстате</span><span class="sxs-lookup"><span data-stu-id="32083-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="32083-160">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="32083-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="32083-161">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="32083-161">Encryption policy setting state.</span></span> <span data-ttu-id="32083-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="32083-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="32083-163">Адванцедбитлоккерстатес</span><span class="sxs-lookup"><span data-stu-id="32083-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="32083-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="32083-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="32083-165">Расширенное состояние BitLocker.</span><span class="sxs-lookup"><span data-stu-id="32083-165">Advanced BitLocker State.</span></span> <span data-ttu-id="32083-166">Возможные значения: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`,. `networkError`</span><span class="sxs-lookup"><span data-stu-id="32083-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="32083-167">Филеваултстатес</span><span class="sxs-lookup"><span data-stu-id="32083-167">fileVaultStates</span></span>|[<span data-ttu-id="32083-168">Филеваултстате</span><span class="sxs-lookup"><span data-stu-id="32083-168">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="32083-169">Состояние Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="32083-169">FileVault State.</span></span> <span data-ttu-id="32083-170">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="32083-170">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="32083-171">Полицидетаилс</span><span class="sxs-lookup"><span data-stu-id="32083-171">policyDetails</span></span>|<span data-ttu-id="32083-172">Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="32083-172">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="32083-173">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="32083-173">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="32083-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="32083-174">Response</span></span>
<span data-ttu-id="32083-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32083-175">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32083-176">Пример</span><span class="sxs-lookup"><span data-stu-id="32083-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="32083-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="32083-177">Request</span></span>
<span data-ttu-id="32083-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32083-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32083-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="32083-179">Response</span></span>
<span data-ttu-id="32083-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32083-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





