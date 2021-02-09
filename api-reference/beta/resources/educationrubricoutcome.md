---
title: Тип ресурса educationRubricOutcome
description: EducationOutcome, который предоставляет оградимую рубрику
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c8132159fa70c175a46a43a13ebce981299f2431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161917"
---
# <a name="educationrubricoutcome-resource-type"></a>Тип ресурса educationRubricOutcome

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[EducationOutcome,](educationoutcome.md) который предоставляет оградимую рубрику.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Обновление объекта educationOutcome. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменял ресурс.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|publishedRubricQualityFeedback|[Коллекция rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Копия свойства rubricQualityFeedback, которая происходит, когда учащемуся отпущен класс.|
|publishedRubricQualitySelectedLevels|[Коллекция rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|Копия свойства rubricQualitySelectedLevels, которая сделана, когда учащемуся был освобожден класс.|
|rubricQualityFeedback|[Коллекция rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)|Коллекция определенных отзывов для каждого качества этой рубрики.|
|rubricQualitySelectedLevels|[Коллекция rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)|Уровень, выбранный преподавателем для каждого качества при классификации этого задания.|

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

