---
title: Тип ресурса Битлоккеррековерикэй
description: Ресурс ключа восстановления BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 038feb77f7ca57d426a44c04b3d9c93ae29e5aa4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082074"
---
# <a name="bitlockerrecoverykey-resource-type"></a>Тип ресурса Битлоккеррековерикэй

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сохраненный ключ BitLocker, который содержит фактический ключ восстановления с помощью **ключевого** свойства.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список Рековерикэйс](../api/bitlocker-list-recoverykeys.md)|Коллекция [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md)|Получение списка объектов [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) и их свойств.|
|[Получение Битлоккеррековерикэй](../api/bitlockerrecoverykey-get.md)|[битлоккеррековерикэй](../resources/bitlockerrecoverykey.md)|Получение свойств и связей объекта [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) . Note: свойство **Key** не возвращается по умолчанию.|

> **Note**: только некоторые роли имеют разрешения на вызов этих API.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время первоначального резервного копирования ключа в Azure Active Directory.|
|deviceId|String|ИДЕНТИФИКАТОР устройства, с которого создана резервная копия ключа BitLocker.|
|id|Строка|Уникальный идентификатор для ключа BitLocker.|
|ключа|Строка|Ключ восстановления BitLocker.|
|волуметипе|волуметипе|Указывает тип тома, с которым связан ключ BitLocker. Возможные значения: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.|

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
  "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
  "createdDateTime": "2020-06-15T13:45:30.0000000Z",
  "volumeType": 1,
  "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
  "key": "123456-231453-873456-213546-654678-765689-123456-324565"
}
```

