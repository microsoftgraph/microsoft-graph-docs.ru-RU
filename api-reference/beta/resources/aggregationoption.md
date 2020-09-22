---
title: Тип ресурса Аггрегатионоптион
description: Указывает объект Аггрегатионоптион
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c18cc1801e5eac76d2fa4396f809ff68f59a78fe
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193971"
---
# <a name="aggregationoption-resource-type"></a>Тип ресурса Аггрегатионоптион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, какие статистические выражения должны возвращаться вместе с результатами поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|поле|String|Задает поле в схеме указанного типа сущностей, для которого необходимо вычислить статистическое выражение. Обязательно.|
|size|Int32|Число возвращаемых ресурсов [сеарчбуккет](searchBucket.md) . Этот параметр не является обязательным, если диапазон предоставляется вручную в запросе поиска. Необязательно.|
|буккетдефинитион|[буккетаггрегатиондефинитион](bucketaggregationdefinition.md)|Задает критерии для вычисления агрегата. Необязательно.|

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