---
title: Тип ресурса Едукатионрубрик
description: Rubricа, который можно прикрепить к назначению
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 154e153166c45a0eb671ab554d1b8ed337fb9830
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406074"
---
# <a name="educationrubric-resource-type"></a>Тип ресурса Едукатионрубрик

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rubricа, который можно прикрепить к назначению. Rubric связан с **educationUser** (преподавателем) и подключен к одному или нескольким ресурсам **educationAssignment** . 

Более подробную информацию вы найдете в статье [образование Rubric Overview](/graph/education-rubric-overview) .

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание Едукатионрубрик](../api/educationuser-post-rubrics.md) | [едукатионрубрик](educationrubric.md) | Создание нового объекта Едукатионрубрик. |
| [Получение Едукатионрубрик](../api/educationrubric-get.md) | [едукатионрубрик](educationrubric.md) | Чтение свойств и связей объекта Едукатионрубрик. |
| [Обновление Едукатионрубрик](../api/educationrubric-update.md) | [едукатионрубрик](educationrubric.md) | Обновление объекта Едукатионрубрик. |
| [Удаление Едукатионрубрик](../api/educationrubric-delete.md) | Нет | Удаление объекта Едукатионрубрик. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот ресурс.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|[itemBody](itembody.md)|Описание этого Rubric.|
|displayName|String|Имя этого Rubric.|
|снижения|[едукатионассигнментградетипе](educationassignmentgradetype.md)|Тип ступенчатости этого Rubric — NULL для нулевых точек Rubric или [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) для точек Rubric.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь для изменения ресурса.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|тонов|Коллекция [рубриклевел](rubriclevel.md)|Коллекция уровней, составляющих данный Rubric.|
|являются|Коллекция [рубриккуалити](rubricquality.md)|Коллекция качеств, составляющих этот Rubric.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "baseType": "",
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