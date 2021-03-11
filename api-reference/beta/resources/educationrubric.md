---
title: тип ресурса educationRubric
description: Рубрика классификации, которую можно прикрепить к назначению
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2e5c9713de4da614c8bfb0f6332930edb8ad775b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721584"
---
# <a name="educationrubric-resource-type"></a>тип ресурса educationRubric

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Рубрика классификации, которую можно прикрепить к назначению. Рубрика связана с **educationUser** (учителем) и присоединена к одному или более ресурсам **educationAssignment.** 

Дополнительные [сведения см. в рубрике Образование.](/graph/education-rubric-overview)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание educationRubric](../api/educationuser-post-rubrics.md) | [educationRubric](educationrubric.md) | Создайте новый объект educationRubric. |
| [Get educationRubric](../api/educationrubric-get.md) | [educationRubric](educationrubric.md) | Чтение свойств и связей объекта educationRubric. |
| [Обновление educationRubric](../api/educationrubric-update.md) | [educationRubric](educationrubric.md) | Обновление объекта educationRubric. |
| [Удаление educationRubric](../api/educationrubric-delete.md) | Нет | Удаление объекта educationRubric. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот ресурс.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|description|[itemBody](itembody.md)|Описание этой рубрики.|
|displayName|String|Название этой рубрики.|
|классификация|[educationAssignmentGradeType](educationassignmentgradetype.md)|Тип классификации этой рубрики — null для неочковой рубрики или [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) для рубрики точек.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменит ресурс.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|уровни|[коллекция rubricLevel](rubriclevel.md)|Коллекция уровней, в которые состоит эта рубрика.|
|качества|[rubricQuality](rubricquality.md) collection|Коллекция качеств, из которых состоит эта рубрика.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->