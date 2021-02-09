---
title: Тип ресурса managedDeviceEncryptionState
description: Отчет о шифровании для каждого устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fb45813f19ef2ef33653902c4468cedf7aed3e7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154259"
---
# <a name="manageddeviceencryptionstate-resource-type"></a><span data-ttu-id="d4956-103">Тип ресурса managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-103">managedDeviceEncryptionState resource type</span></span>

<span data-ttu-id="d4956-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4956-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4956-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4956-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4956-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d4956-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4956-107">Отчет о шифровании для каждого устройства</span><span class="sxs-lookup"><span data-stu-id="d4956-107">Encryption report per device</span></span>

## <a name="methods"></a><span data-ttu-id="d4956-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d4956-108">Methods</span></span>
|<span data-ttu-id="d4956-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d4956-109">Method</span></span>|<span data-ttu-id="d4956-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4956-110">Return Type</span></span>|<span data-ttu-id="d4956-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d4956-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4956-112">Список managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="d4956-112">List managedDeviceEncryptionStates</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|<span data-ttu-id="d4956-113">[Коллекция managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4956-113">[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) collection</span></span>|<span data-ttu-id="d4956-114">Список свойств и связей объектов [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4956-114">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>|
|[<span data-ttu-id="d4956-115">Get managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-115">Get managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[<span data-ttu-id="d4956-116">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-116">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="d4956-117">Чтение свойств и связей объекта [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4956-117">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="d4956-118">Создание managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-118">Create managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[<span data-ttu-id="d4956-119">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-119">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="d4956-120">Создание объекта [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4956-120">Create a new [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|
|[<span data-ttu-id="d4956-121">Удаление managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-121">Delete managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|<span data-ttu-id="d4956-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d4956-122">None</span></span>|<span data-ttu-id="d4956-123">Удаляет [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4956-123">Deletes a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).</span></span>|
|[<span data-ttu-id="d4956-124">Обновление managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-124">Update managedDeviceEncryptionState</span></span>](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[<span data-ttu-id="d4956-125">managedDeviceEncryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-125">managedDeviceEncryptionState</span></span>](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|<span data-ttu-id="d4956-126">Обновление свойств объекта [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)</span><span class="sxs-lookup"><span data-stu-id="d4956-126">Update the properties of a [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4956-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4956-127">Properties</span></span>
|<span data-ttu-id="d4956-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4956-128">Property</span></span>|<span data-ttu-id="d4956-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d4956-129">Type</span></span>|<span data-ttu-id="d4956-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d4956-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4956-131">id</span><span class="sxs-lookup"><span data-stu-id="d4956-131">id</span></span>|<span data-ttu-id="d4956-132">String</span><span class="sxs-lookup"><span data-stu-id="d4956-132">String</span></span>|<span data-ttu-id="d4956-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d4956-133">Key of the entity.</span></span>|
|<span data-ttu-id="d4956-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4956-134">userPrincipalName</span></span>|<span data-ttu-id="d4956-135">String</span><span class="sxs-lookup"><span data-stu-id="d4956-135">String</span></span>|<span data-ttu-id="d4956-136">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="d4956-136">User name</span></span>|
|<span data-ttu-id="d4956-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="d4956-137">deviceType</span></span>|[<span data-ttu-id="d4956-138">deviceTypes</span><span class="sxs-lookup"><span data-stu-id="d4956-138">deviceTypes</span></span>](../resources/intune-deviceconfig-devicetypes.md)|<span data-ttu-id="d4956-139">Платформа устройства.</span><span class="sxs-lookup"><span data-stu-id="d4956-139">Platform of the device.</span></span> <span data-ttu-id="d4956-140">Возможные значения: `desktop` , , , , `windowsRT` , , , , `winMO6` , , , `nokia` , , `windowsPhone` , `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` , `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` .</span><span class="sxs-lookup"><span data-stu-id="d4956-140">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d4956-141">osVersion</span><span class="sxs-lookup"><span data-stu-id="d4956-141">osVersion</span></span>|<span data-ttu-id="d4956-142">String</span><span class="sxs-lookup"><span data-stu-id="d4956-142">String</span></span>|<span data-ttu-id="d4956-143">Версия операционной системы устройства</span><span class="sxs-lookup"><span data-stu-id="d4956-143">Operating system version of the device</span></span>|
|<span data-ttu-id="d4956-144">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="d4956-144">tpmSpecificationVersion</span></span>|<span data-ttu-id="d4956-145">String</span><span class="sxs-lookup"><span data-stu-id="d4956-145">String</span></span>|<span data-ttu-id="d4956-146">Версия TPM устройства</span><span class="sxs-lookup"><span data-stu-id="d4956-146">Device TPM Version</span></span>|
|<span data-ttu-id="d4956-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="d4956-147">deviceName</span></span>|<span data-ttu-id="d4956-148">String</span><span class="sxs-lookup"><span data-stu-id="d4956-148">String</span></span>|<span data-ttu-id="d4956-149">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="d4956-149">Device name</span></span>|
|<span data-ttu-id="d4956-150">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="d4956-150">encryptionReadinessState</span></span>|[<span data-ttu-id="d4956-151">encryptionReadinessState</span><span class="sxs-lookup"><span data-stu-id="d4956-151">encryptionReadinessState</span></span>](../resources/intune-deviceconfig-encryptionreadinessstate.md)|<span data-ttu-id="d4956-152">Состояние готовности шифрования.</span><span class="sxs-lookup"><span data-stu-id="d4956-152">Encryption readiness state.</span></span> <span data-ttu-id="d4956-153">Возможные значения: `notReady`, `ready`.</span><span class="sxs-lookup"><span data-stu-id="d4956-153">Possible values are: `notReady`, `ready`.</span></span>|
|<span data-ttu-id="d4956-154">encryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-154">encryptionState</span></span>|[<span data-ttu-id="d4956-155">encryptionState</span><span class="sxs-lookup"><span data-stu-id="d4956-155">encryptionState</span></span>](../resources/intune-deviceconfig-encryptionstate.md)|<span data-ttu-id="d4956-156">Состояние шифрования устройства.</span><span class="sxs-lookup"><span data-stu-id="d4956-156">Device encryption state.</span></span> <span data-ttu-id="d4956-157">Возможные значения: `notEncrypted`, `encrypted`.</span><span class="sxs-lookup"><span data-stu-id="d4956-157">Possible values are: `notEncrypted`, `encrypted`.</span></span>|
|<span data-ttu-id="d4956-158">encryptionPolicySettingState</span><span class="sxs-lookup"><span data-stu-id="d4956-158">encryptionPolicySettingState</span></span>|[<span data-ttu-id="d4956-159">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d4956-159">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d4956-160">Состояние параметра политики шифрования.</span><span class="sxs-lookup"><span data-stu-id="d4956-160">Encryption policy setting state.</span></span> <span data-ttu-id="d4956-161">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="d4956-161">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d4956-162">advancedBitLockerStates</span><span class="sxs-lookup"><span data-stu-id="d4956-162">advancedBitLockerStates</span></span>|[<span data-ttu-id="d4956-163">advancedBitLockerState</span><span class="sxs-lookup"><span data-stu-id="d4956-163">advancedBitLockerState</span></span>](../resources/intune-deviceconfig-advancedbitlockerstate.md)|<span data-ttu-id="d4956-164">Состояние Advanced BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d4956-164">Advanced BitLocker State.</span></span> <span data-ttu-id="d4956-165">Возможные значения: `success` , , , , , , , `noUserConsent` , , `osVolumeUnprotected` , , `osVolumeTpmRequired` , , `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` , `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` . `networkError`</span><span class="sxs-lookup"><span data-stu-id="d4956-165">Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.</span></span>|
|<span data-ttu-id="d4956-166">fileVaultStates</span><span class="sxs-lookup"><span data-stu-id="d4956-166">fileVaultStates</span></span>|[<span data-ttu-id="d4956-167">fileVaultState</span><span class="sxs-lookup"><span data-stu-id="d4956-167">fileVaultState</span></span>](../resources/intune-deviceconfig-filevaultstate.md)|<span data-ttu-id="d4956-168">Состояние FileVault.</span><span class="sxs-lookup"><span data-stu-id="d4956-168">FileVault State.</span></span> <span data-ttu-id="d4956-169">Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span><span class="sxs-lookup"><span data-stu-id="d4956-169">Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.</span></span>|
|<span data-ttu-id="d4956-170">policyDetails</span><span class="sxs-lookup"><span data-stu-id="d4956-170">policyDetails</span></span>|<span data-ttu-id="d4956-171">[Коллекция encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)</span><span class="sxs-lookup"><span data-stu-id="d4956-171">[encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md) collection</span></span>|<span data-ttu-id="d4956-172">Сведения о политике</span><span class="sxs-lookup"><span data-stu-id="d4956-172">Policy Details</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4956-173">Связи</span><span class="sxs-lookup"><span data-stu-id="d4956-173">Relationships</span></span>
<span data-ttu-id="d4956-174">Нет</span><span class="sxs-lookup"><span data-stu-id="d4956-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4956-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4956-175">JSON Representation</span></span>
<span data-ttu-id="d4956-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4956-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "deviceType": "String",
  "osVersion": "String",
  "tpmSpecificationVersion": "String",
  "deviceName": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "encryptionPolicySettingState": "String",
  "advancedBitLockerStates": "String",
  "fileVaultStates": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
      "policyId": "String",
      "policyName": "String"
    }
  ]
}
```




