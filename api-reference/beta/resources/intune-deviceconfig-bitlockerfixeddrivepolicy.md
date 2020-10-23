---
title: Тип ресурса свойства bitlockerfixeddrivepolicy
description: Политики фиксированного диска BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d53028e901d65403e282abecb91ca70d68cec96
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690709"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a>Тип ресурса свойства bitlockerfixeddrivepolicy

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политики фиксированного диска BitLocker.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[битлоккеренкриптионмесод](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|Выберите метод шифрования для несъемных дисков. Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.|
|requireEncryptionForWriteAccess|Boolean|Этот параметр политики определяет, требуется ли защита BitLocker для несъемных дисков с данными на компьютере.|
|recoveryOptions|[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);|Этот параметр политики позволяет управлять восстановлением несъемных дисков с данными, защищенных с помощью BitLocker, в отсутствие необходимых учетных данных. Этот параметр политики применяется при включении BitLocker.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```





