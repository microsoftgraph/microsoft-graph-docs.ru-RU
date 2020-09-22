---
title: Тип ресурса Рубриклевел
description: Уровень Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 14a7c084aad907ce2e5f90b06f17b64aca9c331e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016114"
---
# <a name="rubriclevel-resource-type"></a>Тип ресурса Рубриклевел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Уровень Rubric. Описание связи между Rubric *качеством*, *уровнями*и *критериями*можно узнать в разделе [едукатионрубрик](educationrubric.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|[itemBody](itembody.md)|Описание этого уровня Rubric.|
|displayName|String|Имя этого уровня Rubric.|
|снижения|[едукатионассигнментградетипе](educationassignmentgradetype.md)|Значение null, если это неrubricная точка. [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) , если это точки Rubric.|
|левелид|String|ИДЕНТИФИКАТОР этого ресурса.|

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

