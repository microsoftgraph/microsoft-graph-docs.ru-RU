---
title: Обновление Манажеддевицеенкриптионстате
description: Обновление свойств объекта Манажеддевицеенкриптионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bfe9b0c0f6d92bd1dfba454811c8bf021a3aa774
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314961"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="fd5ab-103">Обновление Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="fd5ab-103">Update managedDeviceEncryptionState</span></span>

> <span data-ttu-id="fd5ab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd5ab-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd5ab-106">Обновление свойств объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="fd5ab-106">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fd5ab-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fd5ab-107">Prerequisites</span></span>
<span data-ttu-id="fd5ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd5ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd5ab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd5ab-110">Permission type</span></span>|<span data-ttu-id="fd5ab-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd5ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd5ab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd5ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fd5ab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd5ab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fd5ab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd5ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd5ab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-115">Not supported.</span></span>|
|<span data-ttu-id="fd5ab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd5ab-116">Application</span></span>|<span data-ttu-id="fd5ab-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd5ab-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd5ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd5ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="fd5ab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd5ab-119">Request headers</span></span>
|<span data-ttu-id="fd5ab-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd5ab-120">Header</span></span>|<span data-ttu-id="fd5ab-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fd5ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd5ab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd5ab-122">Authorization</span></span>|<span data-ttu-id="fd5ab-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd5ab-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fd5ab-124">Accept</span></span>|<span data-ttu-id="fd5ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fd5ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd5ab-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd5ab-126">Request body</span></span>
<span data-ttu-id="fd5ab-127">В тексте запроса добавьте представление объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-127">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="fd5ab-128">В следующей таблице приведены свойства, необходимые при создании [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span><span class="sxs-lookup"><span data-stu-id="fd5ab-128">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="fd5ab-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd5ab-129">Property</span></span>|<span data-ttu-id="fd5ab-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fd5ab-130">Type</span></span>|<span data-ttu-id="fd5ab-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fd5ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd5ab-132">id</span><span class="sxs-lookup"><span data-stu-id="fd5ab-132">id</span></span>|<span data-ttu-id="fd5ab-133">Строка</span><span class="sxs-lookup"><span data-stu-id="fd5ab-133">String</span></span>|<span data-ttu-id="fd5ab-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-134">Key of the entity.</span></span>|
|<span data-ttu-id="fd5ab-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd5ab-135">userPrincipalName</span></span>|<span data-ttu-id="fd5ab-136">String</span><span class="sxs-lookup"><span data-stu-id="fd5ab-136">String</span></span>|<span data-ttu-id="fd5ab-137">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="fd5ab-137">User name</span></span>|
|<span data-ttu-id="fd5ab-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="fd5ab-138">deviceType</span></span>|[<span data-ttu-id="fd5ab-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="fd5ab-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="fd5ab-140">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-140">Platform of the device.</span></span> <span data-ttu-id="fd5ab-141">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="fd5ab-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="fd5ab-142">osVersion</span></span>|<span data-ttu-id="fd5ab-143">String</span><span class="sxs-lookup"><span data-stu-id="fd5ab-143">String</span></span>|<span data-ttu-id="fd5ab-144">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="fd5ab-144">Operating system version of the device</span></span>|
|<span data-ttu-id="fd5ab-145">тпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="fd5ab-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="fd5ab-146">String</span><span class="sxs-lookup"><span data-stu-id="fd5ab-146">String</span></span>|<span data-ttu-id="fd5ab-147">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="fd5ab-147">Device TPM Version</span></span>|
|<span data-ttu-id="fd5ab-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="fd5ab-148">deviceName</span></span>|<span data-ttu-id="fd5ab-149">String</span><span class="sxs-lookup"><span data-stu-id="fd5ab-149">String</span></span>|<span data-ttu-id="fd5ab-150">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="fd5ab-150">Device name</span></span>|
|<span data-ttu-id="fd5ab-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="fd5ab-151">encryptionReadinessState</span></span>|[<span data-ttu-id="fd5ab-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="fd5ab-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="fd5ab-153">Состояние готовности к шифрованию.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-153">Encryption readiness state.</span></span> <span data-ttu-id="fd5ab-154">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="fd5ab-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="fd5ab-155">encryptionState</span></span>|[<span data-ttu-id="fd5ab-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="fd5ab-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="fd5ab-157">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-157">Device encryption state.</span></span> <span data-ttu-id="fd5ab-158">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="fd5ab-159">енкриптионполицисеттингстате</span><span class="sxs-lookup"><span data-stu-id="fd5ab-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="fd5ab-160">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="fd5ab-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fd5ab-161">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-161">Encryption policy setting state.</span></span> <span data-ttu-id="fd5ab-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fd5ab-163">адванцедбитлоккерстатес</span><span class="sxs-lookup"><span data-stu-id="fd5ab-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="fd5ab-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="fd5ab-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="fd5ab-165">Расширенное состояние BitLocker.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-165">Advanced BitLocker State.</span></span> <span data-ttu-id="fd5ab-166">Возможные значения: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`,. `networkError`</span><span class="sxs-lookup"><span data-stu-id="fd5ab-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="fd5ab-167">филеваултстатес</span><span class="sxs-lookup"><span data-stu-id="fd5ab-167">fileVaultStates</span></span>|[<span data-ttu-id="fd5ab-168">филеваултстате</span><span class="sxs-lookup"><span data-stu-id="fd5ab-168">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="fd5ab-169">Состояние Филеваулт.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-169">FileVault State.</span></span> <span data-ttu-id="fd5ab-170">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-170">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="fd5ab-171">полицидетаилс</span><span class="sxs-lookup"><span data-stu-id="fd5ab-171">policyDetails</span></span>|<span data-ttu-id="fd5ab-172">Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="fd5ab-172">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="fd5ab-173">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="fd5ab-173">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="fd5ab-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd5ab-174">Response</span></span>
<span data-ttu-id="fd5ab-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-175">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd5ab-176">Пример</span><span class="sxs-lookup"><span data-stu-id="fd5ab-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="fd5ab-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd5ab-177">Request</span></span>
<span data-ttu-id="fd5ab-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fd5ab-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd5ab-179">Response</span></span>
<span data-ttu-id="fd5ab-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd5ab-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






