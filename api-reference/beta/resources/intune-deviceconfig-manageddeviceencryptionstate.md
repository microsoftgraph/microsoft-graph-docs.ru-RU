---
title: тип ресурса managedDeviceEncryptionState
description: Отчет о шифровании на устройстве
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6225eb0733c2888ea96264e9942762dd4fb48c71
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086794"
---
# <a name="manageddeviceencryptionstate-resource-type"></a>тип ресурса managedDeviceEncryptionState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отчет о шифровании на устройстве

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedDeviceEncryptionStates](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|[коллекция managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Список свойств и связей [объектов managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|
|[Get managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Чтение свойств и связей объекта [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|
|[Создание managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Создайте новый [объект managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|
|[Удаление managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|Нет|Удаляет [управляемыйDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).|
|[Обновление managedDeviceEncryptionState](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Обновление свойств объекта [managedDeviceEncryptionState.](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|userPrincipalName|String|Имя пользователя|
|deviceType|[deviceTypes](../resources/intune-deviceconfig-devicetypes.md)|Платформа устройства. Возможные значения: `desktop` `windowsRT` , , , `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `blackberry` `palm` `unknown` .|
|osVersion|String|Версия операционной системы устройства|
|tpmSpecificationVersion|String|Версия TPM устройства|
|deviceName|String|Имя устройства|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|Состояние готовности шифрования. Возможные значения: `notReady`, `ready`.|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|Состояние шифрования устройств. Возможные значения: `notEncrypted`, `encrypted`.|
|encryptionPolicySettingState|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Состояние настройки политики шифрования. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|advancedBitLockerStates|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|Состояние Advanced BitLocker. Возможные значения: `success` `noUserConsent` , , , , , `osVolumeUnprotected` , , `osVolumeTpmRequired` , `osVolumeTpmOnlyRequired` `osVolumeTpmPinRequired` `osVolumeTpmStartupKeyRequired` `osVolumeTpmPinStartupKeyRequired` `osVolumeEncryptionMethodMismatch` `recoveryKeyBackupFailed` `fixedDriveNotEncrypted` `fixedDriveEncryptionMethodMismatch` `loggedOnUserNonAdmin` `windowsRecoveryEnvironmentNotConfigured` `tpmNotAvailable` `tpmNotReady` `networkError` .|
|fileVaultStates|[fileVaultState](../resources/intune-deviceconfig-filevaultstate.md)|Состояние FileVault. Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.|
|policyDetails|[коллекция encryptionReportPolicyDetails](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)|Сведения о политике|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
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



