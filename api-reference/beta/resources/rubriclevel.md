---
title: Тип ресурса Рубриклевел
description: Уровень Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 24af9e9be6dc9b63934a02193958e0267dde8dea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521014"
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