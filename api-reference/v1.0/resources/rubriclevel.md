---
title: тип ресурса rubricLevel
description: Уровень рубрики.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef944854949e590abc5a3455cc9683d18f069ebb932be337eb6351d64899fd09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249134"
---
# <a name="rubriclevel-resource-type"></a>тип ресурса rubricLevel

Пространство имен: microsoft.graph

Уровень рубрики. 

См. [в рубрике EducationRubric](educationrubric.md) описание взаимосвязи между качествами,  *уровнями* и критериями *рубрики.*

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|[itemBody](itembody.md)|Описание этого уровня рубрики.|
|displayName|String|Имя этого уровня рубрики.|
|классификация|[educationAssignmentGradeType](educationassignmentgradetype.md)|Null, если это не пункты рубрики; [educationAssignmentPointsGradeType,](educationassignmentpointsgradetype.md) если это точки рубрики.|
|levelId|String|ID этого ресурса.|

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

