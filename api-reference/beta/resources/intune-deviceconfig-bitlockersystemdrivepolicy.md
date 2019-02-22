---
title: Тип ресурса Bitlockersystemdrivepolicy.
description: Основные политики шифрования BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 27b4492dd6df2821cfdeb885d3412536c0d3991c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164892"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a>Тип ресурса Bitlockersystemdrivepolicy.

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Основные политики шифрования BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[Битлоккеренкриптионмесод](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Выберите метод шифрования для дисков операционной системы. Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|startupAuthenticationRequired|Логический|Требовать дополнительной проверки подлинности при запуске.|
|startupAuthenticationBlockWithoutTpmChip|Логический|Указывает, следует ли разрешить BitLocker без совместимого ДОВЕРЕНного ПЛАТФОРМЕНного модуля (требуется пароль или ключ запуска на USB флэш-накопителе).|
|startupAuthenticationTpmUsage|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешена или не разрешена или необязательная Загрузка TPM. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinUsage|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешен ли ПИН-код для запуска TPM, обязательный или запрещенный. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmKeyUsage|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешен ли ключ запуска TPM, обязательный, обязательный или запрещенный. Возможные значения: `blocked`, `required`, `allowed`.|
|startupAuthenticationTpmPinAndKeyUsage|[Конфигуратионусаже](../resources/intune-deviceconfig-configurationusage.md)|Указывает, разрешены ли ключ и ключ ПИН-кода для запуска TPM, а какие — обязательные или запрещенные. Возможные значения: `blocked`, `required`, `allowed`.|
|minimumPinLength|Int32|Указывает минимальную длину ПИН-кода для запуска. Допустимые значения — от 4 до 20.|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);|Позволяет восстанавливать зашифрованные диски операционной системы BitLocker в отсутствие требуемых сведений о ключе запуска. Этот параметр политики применяется при включении BitLocker.|
|prebootRecoveryEnableMessageAndUrl|Логический|Включение сообщения о восстановлении перед загрузкой и URL-адреса. Если Рекуирестартупаусентикатион имеет значение false, это значение не влияет.|
|Пребутрековеримессаже|String|Определяет настраиваемое сообщение о восстановлении.|
|Пребутрековерюрл|String|Определяет настраиваемый URL-адрес для восстановления.|

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




