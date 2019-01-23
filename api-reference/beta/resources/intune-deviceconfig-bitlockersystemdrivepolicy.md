---
title: Тип ресурса bitLockerSystemDrivePolicy
description: Базовый политики шифрования BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425710"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>Тип ресурса bitLockerSystemDrivePolicy

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый политики шифрования BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Выберите метод шифрования для дисков операционной системы. Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Логический|Требовать дополнительную проверку подлинности при запуске системы.|
|startupAuthenticationBlockWithoutTpmChip|Логический|Указывает, следует ли разрешить BitLocker без совместимого TPM (требуется пароль или ключ запуска на флэш-накопитель USB).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, является ли запуска TPM разрешенных/необходимые/не разрешены. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, является ли ПИН-кода запуска TPM разрешенных/необходимые/не разрешены. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, является ли ключ запуска TPM разрешенных/необходимые/не разрешены. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, если прикрепление запуска TPM и ключ разрешенных/необходимые/не разрешены. Возможные значения: `blocked`, `required`, `allowed`.|
|minimumPinLength|Int32|Указывает минимальную длину ПИН-кодов запуска. Допустимые значения 4 до 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);|Разрешает Восстановление зашифрованного BitLocker дисков операционной системы в случае отсутствия данные ключа требуется запуска. Этот параметр политики применяется при включении BitLocker.|
|prebootRecoveryEnableMessageAndUrl|Логический|Включение восстановления до загрузки сообщение и URL-адрес. Если requireStartupAuthentication имеет значение false, это значение не влияет на.|
|prebootRecoveryMessage|String|Определяет сообщение настраиваемого восстановления.|
|prebootRecoveryUrl|String|Определяет URL-адрес настраиваемого восстановления.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```




