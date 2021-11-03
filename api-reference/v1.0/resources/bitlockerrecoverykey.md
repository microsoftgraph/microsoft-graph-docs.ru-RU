---
title: тип ресурса bitlockerRecoveryKey
description: Ресурс ключа восстановления BitLocker
author: hafowler
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8805b8cd633558145787f6a3c4f941fcabad0c62
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696142"
---
# <a name="bitlockerrecoverykey-resource-type"></a>тип ресурса bitlockerRecoveryKey

Пространство имен: microsoft.graph

Представляет сохраненный ключ BitLocker, содержащий фактический ключ восстановления с помощью **свойства ключа.**

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список recoveryKeys](../api/bitlocker-list-recoverykeys.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection|Получите список объектов [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) и их свойств.|
|[Get bitlockerRecoveryKey](../api/bitlockerrecoverykey-get.md)|[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)|Извлечение свойств и связей [объекта bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md) Примечание. **Свойство ключа** не возвращается по умолчанию.|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время, когда клавиша изначально была отсвеяна до Azure Active Directory. Значение null не допускается.|
|deviceId|String|Идентификатор устройства с ключом BitLocker изначально отсвеялся. Поддерживает `$filter` (`eq`).|
|id|String|Уникальный идентификатор для ключа BitLocker.|
|ключа|String|Ключ восстановления BitLocker. Возвращается только с помощью оператора `$select`. Значение null не допускается.|
|volumeType|volumeType|Указывает тип тома, с чем связан ключ BitLocker. Возможные значения: `1` (для `operatingSystemVolume` ), `2` `fixedDataVolume` (для), `3` `removableDataVolume` (для) и `4` `unknownFutureValue` (для).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "volumeType": "String",
  "deviceId": "String",
  "key": "String"
}
```

