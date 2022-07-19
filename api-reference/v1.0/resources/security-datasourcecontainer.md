---
title: Тип ресурса dataSourceContainer
description: Базовый класс для хранителей и источников данных, отличных от хранителей.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 36039c4e548b8db771cacb97c0adbb3c5361729c
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839693"
---
# <a name="datasourcecontainer-resource-type"></a>Тип ресурса dataSourceContainer

Пространство имен: microsoft.graph.security



Базовый класс для [ресурсов eDiscoveryCustodian](../resources/security-ediscoverycustodian.md) и [eDiscoveryNonCutodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .

Это абстрактный тип.

Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|Состояние удержания dataSourceContainer. Возможные значения: `notApplied`, , `applied`, `applying`, `removing``partial`|
|createdDateTime|DateTimeOffset|Дата и время создания сущности dataSourceContainer.|
|displayName|Строка|Отображаемое имя сущности dataSourceContainer.|
|id|String|Уникальный идентификатор dataSourceContainer. Наследуется [от сущности](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения dataSourceContainer.|
|releasedDateTime|DateTimeOffset|Дата и время освобождения dataSourceContainer из дела.|
|status|microsoft.graph.security.dataSourceContainerStatus|Последнее состояние dataSourceContainer. Возможные значения: `Active`, `Released`.|

### <a name="datasourcecontainerstatus-values"></a>Значения dataSourceContainerStatus

|Member|Описание|
|:----|-----------|
| Активных| Контейнер источника данных активен.|
| Выпуска | Контейнер источника данных выпущен.|

### <a name="datasourceholdstatus-values"></a>Значения dataSourceHoldStatus

|Member|Описание|
|:----|-----------|
| notApplied | Контейнер источника данных не находится на удержании.|
| Применяется | Контейнер источника данных находится на удержании.|
| Применение | Контейнер источника данных находится в состоянии удержания (активируется операция applyHold).|
| Удаление | Контейнер источника данных удаляет состояние удержания (активируется операция removeHold).|
| Частичное | Контейнер источника данных находится в смешанном состоянии, где некоторые источники находятся на удержании, а некоторые не находятся в состоянии удержания или ошибки.|
## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

