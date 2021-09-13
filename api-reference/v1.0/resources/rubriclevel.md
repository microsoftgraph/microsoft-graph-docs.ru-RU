---
title: тип ресурса rubricLevel
description: Уровень рубрики.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5db0dac5bf68047f0ebc9dd38554d002a678dca6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113534"
---
# <a name="rubriclevel-resource-type"></a>тип ресурса rubricLevel

Пространство имен: microsoft.graph

Уровень рубрики. 

См. [в рубрике EducationRubric](educationrubric.md) описание взаимосвязи между качествами,  *уровнями* и критериями *рубрики.*

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|[itemBody](itembody.md)|Описание этого уровня рубрики.|
|displayName|Строка|Имя этого уровня рубрики.|
|классификация|[educationAssignmentGradeType](educationassignmentgradetype.md)|Null, если это не пункты рубрики; [educationAssignmentPointsGradeType,](educationassignmentpointsgradetype.md) если это точки рубрики.|
|levelId|Строка|ID этого ресурса.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

