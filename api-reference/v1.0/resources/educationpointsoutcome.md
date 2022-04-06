---
title: Тип ресурса educationPointsOutcome
description: EducationOutcome с числовым оценок.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e0dcab6cc22aa694754c13fce2104aed97d10200
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685224"
---
# <a name="educationpointsoutcome-resource-type"></a>Тип ресурса educationPointsOutcome

Пространство имен: microsoft.graph

[EducationOutcome](educationoutcome.md) с числовым оценок.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Обновление объекта educationOutcome. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Уникальный идентификатор для educationPointsOutcome.|
|points|[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)|Числовой класс, который преподаватель предоставил учащемуся для этого задания.|
|publishedPoints|[educationAssignmentPointsGrade](educationassignmentpointsgrade.md)|Копия свойства points, которая создается при выпуске оценки учащемуся.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

