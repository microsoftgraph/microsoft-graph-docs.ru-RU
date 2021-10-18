---
title: тип ресурса authoredNote
description: Представляет свойства заметки, написанной автором
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 30c635ada7a981a4a02c2a20b8904a02d5f24458
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446938"
---
# <a name="authorednote-resource-type"></a>тип ресурса authoredNote

Пространство имен: microsoft.graph

Представляет свойства заметки, написанной автором.

Наследует от [объекта](../resources/entity.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|author|[identity](../resources/identity.md)|Сведения об авторе заметки.|
|содержимое|[itemBody](../resources/itembody.md)|Содержимое заметки.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authoredNote",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authoredNote",
  "author": {
    "@odata.type": "microsoft.graph.identity"
  },
  "content": {
    "@odata.type": "microsoft.graph.itemBody",
    "content": "String",
    "contentType": "String"
  },
  "createdDateTime": "String (timestamp)"
}
```

