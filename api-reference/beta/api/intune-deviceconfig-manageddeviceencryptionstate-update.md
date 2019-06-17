---
title: Обновление Манажеддевицеенкриптионстате
description: Обновление свойств объекта Манажеддевицеенкриптионстате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1303ba6a6b20d4077b79f7dfef9804d36e93c99f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962969"
---
# <a name="update-manageddeviceencryptionstate"></a><span data-ttu-id="7c0c7-103">Обновление Манажеддевицеенкриптионстате</span><span class="sxs-lookup"><span data-stu-id="7c0c7-103">Update managedDeviceEncryptionState</span></span>

> <span data-ttu-id="7c0c7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c0c7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c0c7-106">Обновление свойств объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .</span><span class="sxs-lookup"><span data-stu-id="7c0c7-106">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c0c7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c0c7-107">Prerequisites</span></span>
<span data-ttu-id="7c0c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c0c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c0c7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c0c7-110">Permission type</span></span>|<span data-ttu-id="7c0c7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c0c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c0c7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c0c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c0c7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c0c7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c0c7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c0c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c0c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-115">Not supported.</span></span>|
|<span data-ttu-id="7c0c7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c0c7-116">Application</span></span>|<span data-ttu-id="7c0c7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c0c7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c0c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="request-headers"></a><span data-ttu-id="7c0c7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c0c7-119">Request headers</span></span>
|<span data-ttu-id="7c0c7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c0c7-120">Header</span></span>|<span data-ttu-id="7c0c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7c0c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c0c7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c0c7-122">Authorization</span></span>|<span data-ttu-id="7c0c7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c0c7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7c0c7-124">Accept</span></span>|<span data-ttu-id="7c0c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c0c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c0c7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c0c7-126">Request body</span></span>
<span data-ttu-id="7c0c7-127">В тексте запроса добавьте представление объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-127">In the request body, supply a JSON representation for the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

<span data-ttu-id="7c0c7-128">В следующей таблице приведены свойства, необходимые при создании [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span><span class="sxs-lookup"><span data-stu-id="7c0c7-128">The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>

|<span data-ttu-id="7c0c7-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c0c7-129">Property</span></span>|<span data-ttu-id="7c0c7-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7c0c7-130">Type</span></span>|<span data-ttu-id="7c0c7-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7c0c7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0c7-132">id</span><span class="sxs-lookup"><span data-stu-id="7c0c7-132">id</span></span>|<span data-ttu-id="7c0c7-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7c0c7-133">String</span></span>|<span data-ttu-id="7c0c7-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-134">Key of the entity.</span></span>|
|<span data-ttu-id="7c0c7-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7c0c7-135">userPrincipalName</span></span>|<span data-ttu-id="7c0c7-136">String</span><span class="sxs-lookup"><span data-stu-id="7c0c7-136">String</span></span>|<span data-ttu-id="7c0c7-137">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="7c0c7-137">User name</span></span>|
|<span data-ttu-id="7c0c7-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="7c0c7-138">deviceType</span></span>|[<span data-ttu-id="7c0c7-139">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="7c0c7-139">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="7c0c7-140">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-140">Platform of the device.</span></span> <span data-ttu-id="7c0c7-141">Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-141">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="7c0c7-142">osVersion</span><span class="sxs-lookup"><span data-stu-id="7c0c7-142">osVersion</span></span>|<span data-ttu-id="7c0c7-143">String</span><span class="sxs-lookup"><span data-stu-id="7c0c7-143">String</span></span>|<span data-ttu-id="7c0c7-144">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="7c0c7-144">Operating system version of the device</span></span>|
|<span data-ttu-id="7c0c7-145">ТпмспеЦификатионверсион</span><span class="sxs-lookup"><span data-stu-id="7c0c7-145">tpmSpecificationVersion</span></span>|<span data-ttu-id="7c0c7-146">String</span><span class="sxs-lookup"><span data-stu-id="7c0c7-146">String</span></span>|<span data-ttu-id="7c0c7-147">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="7c0c7-147">Device TPM Version</span></span>|
|<span data-ttu-id="7c0c7-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="7c0c7-148">deviceName</span></span>|<span data-ttu-id="7c0c7-149">String</span><span class="sxs-lookup"><span data-stu-id="7c0c7-149">String</span></span>|<span data-ttu-id="7c0c7-150">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="7c0c7-150">Device name</span></span>|
|<span data-ttu-id="7c0c7-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="7c0c7-151">encryptionReadinessState</span></span>|[<span data-ttu-id="7c0c7-152">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="7c0c7-152">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="7c0c7-153">Состояние готовности к шифрованию.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-153">Encryption readiness state.</span></span> <span data-ttu-id="7c0c7-154">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-154">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="7c0c7-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="7c0c7-155">encryptionState</span></span>|[<span data-ttu-id="7c0c7-156">encryptionState</span><span class="sxs-lookup"><span data-stu-id="7c0c7-156">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="7c0c7-157">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-157">Device encryption state.</span></span> <span data-ttu-id="7c0c7-158">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-158">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="7c0c7-159">Енкриптионполицисеттингстате</span><span class="sxs-lookup"><span data-stu-id="7c0c7-159">encryptionPolicySettingState</span></span>|[<span data-ttu-id="7c0c7-160">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="7c0c7-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7c0c7-161">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-161">Encryption policy setting state.</span></span> <span data-ttu-id="7c0c7-162">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7c0c7-163">Адванцедбитлоккерстатес</span><span class="sxs-lookup"><span data-stu-id="7c0c7-163">advancedBitLockerStates</span></span>|[<span data-ttu-id="7c0c7-164">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="7c0c7-164">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="7c0c7-165">Расширенное состояние BitLocker.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-165">Advanced BitLocker State.</span></span> <span data-ttu-id="7c0c7-166">Возможные значения: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`,. `networkError`</span><span class="sxs-lookup"><span data-stu-id="7c0c7-166">Possible values are: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="7c0c7-167">Полицидетаилс</span><span class="sxs-lookup"><span data-stu-id="7c0c7-167">policyDetails</span></span>|<span data-ttu-id="7c0c7-168">Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="7c0c7-168">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="7c0c7-169">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="7c0c7-169">Policy Details</span></span>|



## <a name="response"></a><span data-ttu-id="7c0c7-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c0c7-170">Response</span></span>
<span data-ttu-id="7c0c7-171">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-171">If successful, this method returns a `200 OK` response code and an updated [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c0c7-172">Пример</span><span class="sxs-lookup"><span data-stu-id="7c0c7-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c0c7-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c0c7-173">Request</span></span>
<span data-ttu-id="7c0c7-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
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

### <a name="response"></a><span data-ttu-id="7c0c7-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c0c7-175">Response</span></span>
<span data-ttu-id="7c0c7-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c0c7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





