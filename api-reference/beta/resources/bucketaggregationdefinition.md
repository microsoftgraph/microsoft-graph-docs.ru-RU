---
title: Тип ресурса Буккетаггрегатиондефинитион
description: Предоставляет подробные сведения о том, как должны создаваться агрегатионс в результатах.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f9fdadefc43b99b8772217db9a9b101357a1c9c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193985"
---
# <a name="bucketaggregationdefinition-resource-type"></a>Тип ресурса Буккетаггрегатиондефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает сведения для агрегирования результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|sortBy|буккетаггрегатионсортпроперти| Возможные значения: `count` Сортировать по количеству совпадений в агрегате, чтобы отсортировать их по алфавиту в соответствии с ключом в агрегате `keyAsString` , `keyAsNumber` для числовой сортировки на основе ключа в агрегате. Обязательно.
|по убыванию|Логическое|`True` , чтобы указать порядок сортировки по убыванию. По умолчанию используется `false` порядок сортировки по возрастанию. Необязательно.|
|префиксфилтер|String|Фильтр для определения условия соответствия. Ключ должен начинаться с указанного префикса, возвращаемого в ответе. Необязательно.|
|минимумкаунт|Int32|Минимальное количество элементов, которые должны присутствовать в агрегате для возврата в сегменте. Необязательно.|
|ranges|Коллекция [буккетаггрегатионранже](bucketaggregationrange.md)|Задает диапазоны ручных вычислений для вычисления агрегатов. Это допустимо только для уточнений, не являющихся строками даты или числового типа. Необязательно.|

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