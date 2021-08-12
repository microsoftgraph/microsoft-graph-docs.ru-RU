---
title: тип ресурса educationRubricOutcome
description: EducationOutcome, который содержит градуарную рубрику.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3fad9c8aa16653875060f1ec35a7abd09e875643aea77e40c665300878ba86b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54229279"
---
# <a name="educationrubricoutcome-resource-type"></a>тип ресурса educationRubricOutcome

Пространство имен: microsoft.graph

[EducationOutcome,](educationoutcome.md) который содержит градуарную рубрику.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Обновление объекта educationOutcome. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменит ресурс.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|publishedRubricQualityFeedback|[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection|Копия свойства rubricQualityFeedback, которое будет сделано после выпуска класса для учащегося.|
|publishedRubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection|Копия свойства rubricQualitySelectedLevels, выполненного при отсвойке класса учащемуся.|
|rubricQualityFeedback|[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection|Коллекция конкретных отзывов для каждого качества этой рубрики.|
|rubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection|Уровень, выбранный преподавателем для каждого качества при классификации этого назначения.|

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

