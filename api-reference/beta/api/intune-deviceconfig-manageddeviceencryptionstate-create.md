---
title: Создание Манажеддевицеенкриптионстате
description: Создание нового объекта Манажеддевицеенкриптионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c5fa1846c7f3541e4ea7e3a7cc0186fe01f8290
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962990"
---
# <a name="create-manageddeviceencryptionstate"></a><span data-ttu-id="e8f5d-103">Создание Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="e8f5d-103">Create managedDeviceEncryptionState</span></span>

> <span data-ttu-id="e8f5d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f5d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f5d-106">Создание нового объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="e8f5d-106">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8f5d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e8f5d-107">Prerequisites</span></span>
<span data-ttu-id="e8f5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8f5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8f5d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8f5d-110">Permission type</span></span>|<span data-ttu-id="e8f5d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8f5d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8f5d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8f5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8f5d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8f5d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8f5d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8f5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8f5d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-115">Not supported.</span></span>|
|<span data-ttu-id="e8f5d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8f5d-116">Application</span></span>|<span data-ttu-id="e8f5d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8f5d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8f5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="e8f5d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8f5d-119">Request headers</span></span>
|<span data-ttu-id="e8f5d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8f5d-120">Header</span></span>|<span data-ttu-id="e8f5d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e8f5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8f5d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8f5d-122">Authorization</span></span>|<span data-ttu-id="e8f5d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8f5d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e8f5d-124">Accept</span></span>|<span data-ttu-id="e8f5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8f5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8f5d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8f5d-126">Request body</span></span>
<span data-ttu-id="e8f5d-127">В тексте запроса добавьте представление объекта Манажеддевицеенкриптионстате в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-127">In the request body, supply a JSON representation for the managedDeviceEncryptionState object.</span></span>

<span data-ttu-id="e8f5d-128">В следующей таблице приведены свойства, необходимые при создании Манажеддевицеенкриптионстате.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-128">The following table shows the properties that are required when you create the managedDeviceEncryptionState.</span></span>

|<span data-ttu-id="e8f5d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8f5d-129">Property</span></span>|<span data-ttu-id="e8f5d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e8f5d-130">Type</span></span>|<span data-ttu-id="e8f5d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e8f5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8f5d-132">id</span><span class="sxs-lookup"><span data-stu-id="e8f5d-132">id</span></span>|<span data-ttu-id="e8f5d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e8f5d-133">String</span></span>|<span data-ttu-id="e8f5d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-134">Key of the entity.</span></span>|
|<span data-ttu-id="e8f5d-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e8f5d-135">userPrincipalName</span></span>|<span data-ttu-id="e8f5d-136">String</span><span class="sxs-lookup"><span data-stu-id="e8f5d-136">String</span></span>|<span data-ttu-id="e8f5d-137">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="e8f5d-137">User name</span></span>|
|<span data-ttu-id="e8f5d-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="e8f5d-138">deviceType</span></span>|[<span data-ttu-id="e8f5d-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="e8f5d-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="e8f5d-140">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-140">Platform of the device.</span></span> <span data-ttu-id="e8f5d-141">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="e8f5d-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="e8f5d-142">osVersion</span></span>|<span data-ttu-id="e8f5d-143">String</span><span class="sxs-lookup"><span data-stu-id="e8f5d-143">String</span></span>|<span data-ttu-id="e8f5d-144">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="e8f5d-144">Operating system version of the device</span></span>|
|<span data-ttu-id="e8f5d-145">ТпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="e8f5d-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="e8f5d-146">String</span><span class="sxs-lookup"><span data-stu-id="e8f5d-146">String</span></span>|<span data-ttu-id="e8f5d-147">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="e8f5d-147">Device TPM Version</span></span>|
|<span data-ttu-id="e8f5d-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="e8f5d-148">deviceName</span></span>|<span data-ttu-id="e8f5d-149">String</span><span class="sxs-lookup"><span data-stu-id="e8f5d-149">String</span></span>|<span data-ttu-id="e8f5d-150">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="e8f5d-150">Device name</span></span>|
|<span data-ttu-id="e8f5d-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="e8f5d-151">encryptionReadinessState</span></span>|[<span data-ttu-id="e8f5d-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="e8f5d-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="e8f5d-153">Состояние готовности к шифрованию.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-153">Encryption readiness state.</span></span> <span data-ttu-id="e8f5d-154">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="e8f5d-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="e8f5d-155">encryptionState</span></span>|[<span data-ttu-id="e8f5d-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="e8f5d-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="e8f5d-157">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-157">Device encryption state.</span></span> <span data-ttu-id="e8f5d-158">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="e8f5d-159">Енкриптионполицисеттингстате</span><span class="sxs-lookup"><span data-stu-id="e8f5d-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="e8f5d-160">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="e8f5d-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e8f5d-161">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-161">Encryption policy setting state.</span></span> <span data-ttu-id="e8f5d-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e8f5d-163">Адванцедбитлоккерстатес</span><span class="sxs-lookup"><span data-stu-id="e8f5d-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="e8f5d-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="e8f5d-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="e8f5d-165">Расширенное состояние BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-165">Advanced BitLocker State.</span></span> <span data-ttu-id="e8f5d-166">Возможные значения: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`,. `networkError`</span><span class="sxs-lookup"><span data-stu-id="e8f5d-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="e8f5d-167">Полицидетаилс</span><span class="sxs-lookup"><span data-stu-id="e8f5d-167">policyDetails</span></span>|<span data-ttu-id="e8f5d-168">Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="e8f5d-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="e8f5d-169">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="e8f5d-169">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="e8f5d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8f5d-170">Response</span></span>
<span data-ttu-id="e8f5d-171">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-171">If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8f5d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="e8f5d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8f5d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8f5d-173">Request</span></span>
<span data-ttu-id="e8f5d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
Content-type: application/json
Content-length: 658

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
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e8f5d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8f5d-175">Response</span></span>
<span data-ttu-id="e8f5d-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8f5d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 707

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
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "Policy Id value",
      "policyName": "Policy Name value"
    }
  ]
}
```





