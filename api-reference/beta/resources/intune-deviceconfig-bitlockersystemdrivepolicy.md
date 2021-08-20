---
title: тип ресурса bitLockerSystemDrivePolicy
description: Базовые политики шифрования BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 61366c25539538f7026c0e844a4958ab7c1d0c95ec87b9375016e9791fe6d4ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54250030"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>тип ресурса bitLockerSystemDrivePolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовые политики шифрования BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[bitLockerEncryptionMethod](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Выберите метод шифрования для дисков операционной системы. Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Логический|Требуется дополнительная проверка подлинности при запуске.|
|startupAuthenticationBlockWithoutTpmChip|Логический|Указывает, следует ли разрешить BitLocker без совместимого TPM (требуется пароль или ключ запуска на флеш-накопителе USB).|
|startupAuthenticationTpmUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешен ли запуск TPM/требуется/отсеяно. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|startupAuthenticationTpmPinUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешен ли пин-код запуска TPM/required/disallowed. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|startupAuthenticationTpmKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешен ли ключ запуска TPM/ требуется/отсеяно. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|startupAuthenticationTpmPinAndKeyUsage|[configurationUsage](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешены ли пин-код и ключ для запуска TPM. Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.|
|minimumPinLength|Int32|Указывает минимальную длину пин-кода запуска. Допустимые значения от 4 до 20|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);|Позволяет восстановить диски зашифрованной операционной системы BitLocker при отсутствии необходимой информации о ключе запуска. Этот параметр политики применяется при включке BitLocker.|
|prebootRecoveryEnableMessageAndUrl|Логический|Включить сообщение о восстановлении перед загрузкой и URL-адрес. Если требуетсяStartupAuthentication является ложным, это значение не влияет.|
|prebootRecoveryMessage|String|Определяет настраиваемые сообщения восстановления.|
|prebootRecoveryUrl|String|Определяет настраиваемый URL-адрес восстановления.|

## <a name="relationships"></a>Связи
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




