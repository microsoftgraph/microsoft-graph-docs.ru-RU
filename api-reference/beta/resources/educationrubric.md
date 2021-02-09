---
title: Тип ресурса educationRubric
description: Рубрика ограды, которую можно прикрепить к назначению
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37e1d4a6267f1f1292a72cc7f34b8135483091ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161938"
---
# <a name="educationrubric-resource-type"></a>Тип ресурса educationRubric

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Рубрика ограды, которую можно прикрепить к назначению. Рубрика связана с **educationUser** (преподавателем) и прикреплена к одному или более **ресурсам educationAssignment.** 

Дополнительные [сведения см. в обзоре рубрики для](/graph/education-rubric-overview) образования.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание educationRubric](../api/educationuser-post-rubrics.md) | [educationRubric](educationrubric.md) | Создание объекта educationRubric. |
| [Get educationRubric](../api/educationrubric-get.md) | [educationRubric](educationrubric.md) | Чтение свойств и связей объекта educationRubric. |
| [Обновление educationRubric](../api/educationrubric-update.md) | [educationRubric](educationrubric.md) | Обновление объекта educationRubric. |
| [Удаление educationRubric](../api/educationrubric-delete.md) | Нет | Удаление объекта educationRubric. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот ресурс.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|(описание)|[itemBody](itembody.md)|Описание этой рубрики.|
|displayName|String|Имя этой рубрики.|
|grading|[educationAssignmentGradeType](educationassignmentgradetype.md)|Тип классификации этой рубрики — null для рубрики без пунктов или [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) для рубрики точек.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь, который изменял ресурс.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|levels|[Коллекция rubricLevel](rubriclevel.md)|Коллекция уровней, которые составляет эта рубрика.|
|qualities|[Коллекция rubricQuality](rubricquality.md)|Коллекция качеств, из которых состоит эта рубрика.|

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