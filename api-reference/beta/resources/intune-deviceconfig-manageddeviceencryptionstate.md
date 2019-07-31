---
title: Тип ресурса Манажеддевицеенкриптионстате
description: Отчет о шифровании для каждого устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb212599c56410b7f66d6f8baa8db1d06d36ba60
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000883"
---
# <a name="manageddeviceencryptionstate-resource-type"></a>Тип ресурса Манажеддевицеенкриптионстате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Отчет о шифровании для каждого устройства

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажеддевицеенкриптионстатес](../api/intune-deviceconfig-manageddeviceencryptionstate-list.md)|Коллекция [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Список свойств и связей объектов [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|
|[Получение Манажеддевицеенкриптионстате](../api/intune-deviceconfig-manageddeviceencryptionstate-get.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Чтение свойств и связей объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|
|[Создание Манажеддевицеенкриптионстате](../api/intune-deviceconfig-manageddeviceencryptionstate-create.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Создание нового объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|
|[Удаление Манажеддевицеенкриптионстате](../api/intune-deviceconfig-manageddeviceencryptionstate-delete.md)|Нет|Удаляет объект [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md).|
|[Обновление Манажеддевицеенкриптионстате](../api/intune-deviceconfig-manageddeviceencryptionstate-update.md)|[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)|Обновление свойств объекта [манажеддевицеенкриптионстате](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userPrincipalName|String|Имя пользователя|
|deviceType|[deviceTypes](../resources/intune-deviceconfig-devicetypes.md)|Платформа устройства. Возможные значения: `desktop`, `windowsRT`, `winMO6`, `nokia` `windowsPhone` `mac` `winCE` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `android` `iSocConsumer`,,,,,,,,,,,,,,,,,,,,, `winEmbedded` `iPhone` `iPad` `iPod` , `blackberry`, `palm`, `unknown`.|
|osVersion|String|Версия операционной системы устройства|
|ТпмспеЦификатионверсион|String|Версия TPM устройства|
|deviceName|String|Имя устройства|
|encryptionReadinessState|[encryptionReadinessState](../resources/intune-deviceconfig-encryptionreadinessstate.md)|Состояние готовности к шифрованию. Возможные значения: `notReady`, `ready`.|
|encryptionState|[encryptionState](../resources/intune-deviceconfig-encryptionstate.md)|Состояние шифрования устройства. Возможные значения: `notEncrypted`, `encrypted`.|
|Енкриптионполицисеттингстате|[Комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние параметра политики шифрования. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|Адванцедбитлоккерстатес|[advancedBitLockerState](../resources/intune-deviceconfig-advancedbitlockerstate.md)|Расширенное состояние BitLocker. Возможные значения: `success`, `noUserConsent`, `osVolumeEncryptionMethodMismatch`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeUnprotected`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`,. `networkError`|
|Филеваултстатес|[Филеваултстате](../resources/intune-deviceconfig-filevaultstate.md)|Состояние Филеваулт. Возможные значения: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.|
|Полицидетаилс|Коллекция [енкриптионрепортполицидетаилс](../resources/intune-deviceconfig-encryptionreportpolicydetails.md)|Сведения о политике|

## <a name="relationships"></a>Отношения
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





