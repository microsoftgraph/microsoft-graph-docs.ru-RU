---
title: Тип ресурса dataSourceContainer
description: Базовый класс для хранителей и источников данных, отличных от хранителей.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 7482e31ab1a43cf4c60e7c211acb38d8cac42bfa
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946131"
---
# <a name="datasourcecontainer-resource-type"></a>Тип ресурса dataSourceContainer

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовый класс [для eDiscoveryCustodian](../resources/security-ediscoverycustodian.md) и [eDiscoveryNonCutodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) Это абстрактный тип.
Наследует [от сущности](../resources/entity.md).

## <a name="methods"></a>Методы

Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|holdStatus|Строка|Состояние удержания dataSourceContainer.Возможные значения: `notApplied`, `applied`, `applying`, , `removing``partial`|
|createdDateTime|DateTimeOffset|Дата и время создания сущности dataSourceContainer.|
|displayName|Строка|Отображаемое имя сущности dataSourceContainer.|
|id|String|Уникальный идентификатор dataSourceContainer. Наследуется [от сущности](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения dataSourceContainer.|
|releasedDateTime|DateTimeOffset|Дата и время освобождения dataSourceContainer из дела.|
|status|String|Последнее состояние dataSourceContainer. Возможные значения: `Active`, `Released`.|

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
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

