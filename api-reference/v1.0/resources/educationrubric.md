---
title: Тип ресурса educationRubric
description: Категорию оценки, которую можно присоединить к назначению.
ms.localizationpriority: medium
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f123f0d20f8069c6bfb41258afc2b9d6c3a0e207
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685252"
---
# <a name="educationrubric-resource-type"></a>Тип ресурса educationRubric

Пространство имен: microsoft.graph

Категорию оценки, которую можно присоединить к назначению. Rubric связан с **educationUser** (преподавателем) и присоединен к одному или нескольким **ресурсам educationAssignment** . 

[Дополнительные сведения см. в статье "](/graph/education-rubric-overview)Общие сведения о образованиях".

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание educationRubric](../api/educationuser-post-rubrics.md) | [educationRubric](educationrubric.md) | Создайте объект educationRubric. |
| [Получение educationRubric](../api/educationrubric-get.md) | [educationRubric](educationrubric.md) | Чтение свойств и связей объекта educationRubric. |
| [Обновление educationRubric](../api/educationrubric-update.md) | [educationRubric](educationrubric.md) | Обновление объекта educationRubric. |
| [Удаление educationRubric](../api/educationrubric-delete.md) | Никаких других изменений не происходит | Удаление объекта educationRubric. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Уникальный идентификатор для rubric.|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот ресурс.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.|
|description|[itemBody](itembody.md)|Описание этого учебника.|
|displayName|String|Имя этого учебника.|
|Профилирования|[educationAssignmentGradeType](educationassignmentgradetype.md)|Тип оценки этого rubric — null для rubric без точек или [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) для rubric точек.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменяет ресурс.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|Уровней|[Коллекция rubricLevel](rubriclevel.md)|Коллекция уровней, в которые содержится эта таблица.|
|Качества|[Коллекция rubricQuality](rubricquality.md)|Коллекция качества, которая является частью этого учебника.|

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
  "id": "String (identifier)",
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
