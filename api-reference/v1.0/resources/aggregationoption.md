---
title: тип ресурса aggregationOption
description: Указывает, какие агрегации следует возвращать вместе с результатами поиска
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0f5257c99b655f68859055f76e5c28dd04c03a26
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777290"
---
# <a name="aggregationoption-resource-type"></a>тип ресурса aggregationOption

Пространство имен: microsoft.graph

Указывает, какие агрегации следует возвращать вместе с результатами поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|bucketDefinition|[bucketAggregationDefinition](bucketaggregationdefinition.md)|Указывает критерии для вычисления агрегации. Необязательное свойство.|
|поле|String|Вычисляет агрегацию на поле, пока поле существует в текущем типе сущности. Обязательно.|
|size|Int32|Количество [возвращаемого ресурса searchBucket.](searchBucket.md) Это не требуется, когда диапазон предоставляется вручную в запросе поиска. Необязательное свойство.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.aggregationOption",
  "baseType": null
}-->

```json
{
  "field": "String",
  "size": 1024,
  "bucketDefinition": {"@odata.type": "microsoft.graph.bucketAggregationDefinition"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->