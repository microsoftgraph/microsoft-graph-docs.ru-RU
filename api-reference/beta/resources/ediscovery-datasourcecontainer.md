---
title: Тип ресурса dataSourceContainer
description: Базовый класс для хранителей и источников данных без хранения.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: e2d7d88a3d747817858853ebc6f2909b2edde65b
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080902"
---
# <a name="datasourcecontainer-resource-type"></a>Тип ресурса dataSourceContainer

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовый класс [для хранителя](../resources/ediscovery-custodian.md) [и noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md).

Наследует от [объекта](../resources/entity.md).

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Создана дата и время создания объекта dataSourceContainer.|
|displayName|String|Отображение имени объекта dataSourceContainer.|
|id|String|Уникальный идентификатор dataSourceContainer. Унаследованный от [сущности](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время dataSourceContainer.|
|releasedDateTime|DateTimeOffset|Дата и время освобождения dataSourceContainer из дела.|
|status|microsoft.graph.ediscovery.dataSourceContainerStatus|Последнее состояние dataSourceContainer. Возможные значения: `Active`, `Released`.|

### <a name="datasourcecontainerstatus-values"></a>значения dataSourceContainerStatus

|Member|Описание|
|:---|:---|
|Активное|В этом случае dataSourceContainer находится на удержании.|
|Выпущено|В этом случае dataSourceContainer был освобожден из удержания.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSourceContainer",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSourceContainer",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
