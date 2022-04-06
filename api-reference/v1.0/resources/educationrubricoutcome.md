---
title: Тип ресурса educationRubricOutcome
description: EducationOutcome, предоставляющий оцениваемую rubric.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 831cac7de7510ebc83cf6dc0ddbf5190d1e3d9d9
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685070"
---
# <a name="educationrubricoutcome-resource-type"></a>Тип ресурса educationRubricOutcome

Пространство имен: microsoft.graph

[EducationOutcome](educationoutcome.md), предоставляющий оцениваемую rubric.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Обновление объекта educationOutcome. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Уникальный идентификатор для educationRubricOutcome.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменяет ресурс.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|publishedRubricQualityFeedback|[Коллекция rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Копия свойства rubricQualityFeedback, которая создается при выпуске оценки учащемуся.|
|publishedRubricQualitySelectedLevels|[Коллекция rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|Копия свойства rubricQualitySelectedLevels, которая создается при выпуске оценки учащемуся.|
|rubricQualityFeedback|[Коллекция rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Коллекция определенных отзывов для каждого качества этого учебника.|
|rubricQualitySelectedLevels|[Коллекция rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|Уровень, выбранный преподавателем для каждого качества во время проверки этого задания.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "publishedRubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "publishedRubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}],
  "rubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "rubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubricOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

