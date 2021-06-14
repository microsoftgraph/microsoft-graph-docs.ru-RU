---
title: тип ресурса rubricQuality
description: Качество рубрики.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82fdb8fa226ab6eb2c38b1e49e12904ff26b6491
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911522"
---
# <a name="rubricquality-resource-type"></a>тип ресурса rubricQuality

Пространство имен: microsoft.graph

Качество рубрики. 

См. [в рубрике EducationRubric](educationrubric.md) описание взаимосвязи между качествами,  *уровнями* и критериями *рубрики.*

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|criteria|[rubricCriterion](rubriccriterion.md) collection|Набор критериев для этого качества рубрики.|
|description|[itemBody](itembody.md)|Описание этого качества рубрики.|
|displayName|String|Имя этого качества рубрики.|
|qualityId|String|ID этого ресурса.|
|weight|Одинарное|Если есть, то числовой вес для этого качества.  Весы должны добавить до 100.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

