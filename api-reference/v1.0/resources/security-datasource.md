---
title: Тип ресурса dataSource
description: Сущность dataSource — это абстрактный базовый класс, используемый для определения источников содержимого для обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c388280b0c6c8f005c59dcdfb11aa20fafa18dbd
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66840193"
---
# <a name="datasource-resource-type"></a>Тип ресурса dataSource

Пространство имен: microsoft.graph.security



Сущность dataSource — это абстрактный базовый класс, используемый для определения источников содержимого для обнаружения электронных данных.

## <a name="methods"></a>Методы

Нет.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший **источник данных**.|
|createdDateTime|DateTimeOffset|Дата и время **создания источника** данных.|
|displayName|Строка|Отображаемое имя **источника данных**. Это будет имя сайта SharePoint.|
|id|String| Идентификатор источника **данных**. Это не идентификатор фактического сайта.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|Состояние удержания **источника данных**. Возможные значения: `notApplied`, , `applied`, `applying`, `removing``partial`|
## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.dataSource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.dataSource",
  "id": "String (identifier)",
  "displayName": "String",
  "holdStatus": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

