---
title: Тип ресурса Bitlockersystemdrivepolicy.
description: Основные политики шифрования BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82ed6d717c58f740dd25d2aff18478ced48c4641
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453675"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>Тип ресурса Bitlockersystemdrivepolicy.

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Основные политики шифрования BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[битлоккеренкриптионмесод](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Выберите метод шифрования для дисков операционной системы. Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Логическое|Требовать дополнительной проверки подлинности при запуске.|
|startupAuthenticationBlockWithoutTpmChip|Логическое|Указывает, следует ли разрешить BitLocker без совместимого доверенного платформенного модуля (требуется пароль или ключ запуска на USB флэш-накопителе).|
|startupAuthenticationTpmUsage|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешена или не разрешена или необязательная Загрузка TPM. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешен ли ПИН-код для запуска TPM, обязательный или запрещенный. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmKeyUsage|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешен ли ключ запуска TPM, обязательный, обязательный или запрещенный. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешены ли ключ и ключ ПИН-кода для запуска TPM, а какие — обязательные или запрещенные. Возможные значения: `blocked`, `required`, `allowed`.|
|minimumPinLength|Int32|Указывает минимальную длину ПИН-кода для запуска. Допустимые значения — от 4 до 20.|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);|Позволяет восстанавливать зашифрованные диски операционной системы BitLocker в отсутствие требуемых сведений о ключе запуска. Этот параметр политики применяется при включении BitLocker.|
|prebootRecoveryEnableMessageAndUrl|Логическое|Включение сообщения о восстановлении перед загрузкой и URL-адреса. Если Рекуирестартупаусентикатион имеет значение false, это значение не влияет.|
|пребутрековеримессаже|String|Определяет настраиваемое сообщение о восстановлении.|
|пребутрековерюрл|String|Определяет настраиваемый URL-адрес для восстановления.|

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



