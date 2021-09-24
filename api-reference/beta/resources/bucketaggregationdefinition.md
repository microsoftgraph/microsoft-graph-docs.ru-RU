---
title: тип ресурса bucketAggregationDefinition
description: Предоставляет сведения о том, как создавать агрегации в результатах
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0100852456ec9431e0d0d0bb5cd78d2f236392bb
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507510"
---
# <a name="bucketaggregationdefinition-resource-type"></a>тип ресурса bucketAggregationDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о том, как создавать агрегации в результатах.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isDescending|Логический|`True` указать порядок сортировки как нисходящее. По умолчанию `false` имеется порядок сортировки как восходящий. Необязательное свойство.|
|minimumCount|Int32|Минимальное количество элементов, которые должны присутствовать в агрегации, которые будут возвращены в ведро. Необязательное свойство.|
|prefixFilter|String|Фильтр для определения соответствия критериям. Ключ должен начинаться с указанной префикса, которая будет возвращена в ответе. Необязательное свойство.|
|ranges|[коллекция bucketAggregationRange](bucketaggregationrange.md)|Указывает диапазоны вручную для вычисления агрегаций. Это допустимо только для неструкционных переработчиков датного или числового типа. Необязательное свойство.|
|sortBy|bucketAggregationSortProperty| Возможные значения должны сортировать по количеству совпадений в агрегации, сортировать алфавит на основе ключа в агрегации, для числовых сортировки на основе ключа в `count` агрегации. `keyAsString` `keyAsNumber` Обязательный элемент.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationDefinition",
  "baseType": null
}-->

```json
{
  "sortBy": "String",
  "isDescending": true,
  "prefixFilter": "String",
  "minimumCount": 1024,
  "ranges": [{"@odata.type": "microsoft.graph.bucketAggregationRange"}]
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