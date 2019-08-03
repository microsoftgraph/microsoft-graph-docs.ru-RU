---
title: Тип ресурса Едукатионрубрикауткоме
description: Едукатионауткоме, обеспечивающий высококачественный Rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4640daa1bb93945463cffc9dcf54d4db23b84da1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173260"
---
# <a name="educationrubricoutcome-resource-type"></a>Тип ресурса Едукатионрубрикауткоме

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект [едукатионауткоме](educationoutcome.md) , обеспечивающий высококачественную Rubric.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление Едукатионауткоме](../api/educationoutcome-update.md) | [Едукатионауткоме](educationoutcome.md) | Обновление объекта Едукатионауткоме. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь для изменения ресурса.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Публишедрубриккуалитифидбакк|Коллекция [рубриккуалитифидбаккмодел](rubricqualityfeedbackmodel.md)|Копия свойства Рубриккуалитифидбакк, выполняемого при отпадении оценки на учащийся.|
|Публишедрубриккуалитиселектедлевелс|Коллекция [рубриккуалитиселектедколумнмодел](rubricqualityselectedcolumnmodel.md)|Копия свойства Рубриккуалитиселектедлевелс, выполняемого при отпадении оценки на учащийся.|
|Рубриккуалитифидбакк|Коллекция [рубриккуалитифидбаккмодел](rubricqualityfeedbackmodel.md)|Коллекция определенных отзывов для каждого качества этого Rubric.|
|Рубриккуалитиселектедлевелс|Коллекция [рубриккуалитиселектедколумнмодел](rubricqualityselectedcolumnmodel.md)|Уровень, который преподаватель выбрал для каждого качества при ступенчатом назначении.|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "baseType": "",
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