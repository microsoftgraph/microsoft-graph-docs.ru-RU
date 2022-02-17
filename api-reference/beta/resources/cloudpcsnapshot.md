---
title: тип ресурса cloudPcSnapshot
description: Представляет снимок облачного КОМПЬЮТЕРА.
author: xintaozMS
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 14cf7ecffe7980db32abf81d475f45ac5725c64c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878782"
---
# <a name="cloudpcsnapshot-resource-type"></a>тип ресурса cloudPcSnapshot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет снимок параметров устройства облачного компьютера, которые можно использовать для восстановления системы устройства.


Наследуется [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Снимки списка](../api/virtualendpoint-list-snapshots.md)|[коллекция cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Получите список объектов [cloudPcSnapshot](../resources/cloudpcsnapshot.md) и их свойств.|
|[Get cloudPcSnapshot](../api/cloudpcsnapshot-get.md)|[cloudPcSnapshot](../resources/cloudpcsnapshot.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPcSnapshot](../resources/cloudpcsnapshot.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|cloudPcId|String|Уникальный идентификатор облачного компьютера.|
|createdDateTime|DateTimeOffset|Дата и время, в которые был сделан снимок. Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|Строка|Уникальный идентификатор для снимка устройства облачного ПК в определенный момент времени. Наследуется [от сущности](../resources/entity.md).|
|lastRestoredDateTime|DateTimeOffset|Дата и время последнего использования снимка для восстановления устройства Облачного ПК. Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|status|[cloudPcSnapshotStatus](#cloudpcsnapshotstatus-values)|Состояние снимка облачного КОМПЬЮТЕРА. Возможные значения: `ready`, `unknownFutureValue`.|

### <a name="cloudpcsnapshotstatus-values"></a>значения cloudPcSnapshotStatus 

|Member|Описание|
|:---|:---|
|готово|Снимок готов к восстановлению устройства облачного ПК.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcSnapshot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSnapshot",
  "cloudPcId": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastRestoredDateTime": "String (timestamp)",
  "status": "String"
}
```

