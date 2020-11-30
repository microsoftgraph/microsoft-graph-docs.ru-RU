---
title: Тип ресурса Сеарчхит
description: Описание объекта Сеарчхит
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bad671657e46068263d3386eb0bb04026cfaa28e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378017"
---
# <a name="searchhit-resource-type"></a>Тип ресурса Сеарчхит

Пространство имен: microsoft.graph

Представляет один результат в списке результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hitId|Строка|Внутренний идентификатор элемента.|
|rank|Int32|Ранг или порядок результатов.|
|contentSource|Строка|Имя источника контента, частью которого является **екстерналитем** .|
|summary|Строка|Сводка результатов, если доступна сводка.|
|resource|[entity](entity.md)|Базовое представление результатов поиска в Microsoft Graph.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

