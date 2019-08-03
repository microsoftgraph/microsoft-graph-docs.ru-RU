---
title: Тип ресурса Едукатионрубрик
description: Rubricа, который можно прикрепить к назначению
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b43b611465af4dabb62d9dd741eb9a8670f241b9
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173239"
---
# <a name="educationrubric-resource-type"></a>Тип ресурса Едукатионрубрик

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Rubricа, который можно прикрепить к назначению. Rubric связан с **educationUser** (преподавателем) и подключен к одному или нескольким ресурсам **educationAssignment** . 

Более подробную информацию вы найдете в статье [образование Rubric Overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) .

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Едукатионрубрик](../api/educationrubric-get.md) | [Едукатионрубрик](educationrubric.md) | Чтение свойств и связей объекта Едукатионрубрик. |
| [Обновление Едукатионрубрик](../api/educationrubric-update.md) | [Едукатионрубрик](educationrubric.md) | Обновление объекта Едукатионрубрик. |
| [Удаление Едукатионрубрик](../api/educationrubric-delete.md) | Нет | Удаление объекта Едукатионрубрик. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy|[identitySet](identityset.md)|Пользователь, создавший этот ресурс.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|description|[itemBody](itembody.md)|Описание этого Rubric.|
|displayName|String|Имя этого Rubric.|
|снижения|[Едукатионассигнментградетипе](educationassignmentgradetype.md)|Тип ступенчатости этого Rubric — NULL для нулевых точек Rubric или [едукатионассигнментпоинтсградетипе](educationassignmentpointsgradetype.md) для точек Rubric.|
|lastModifiedBy|[identitySet](identityset.md)|Последний пользователь для изменения ресурса.|
|lastModifiedDateTime|DateTimeOffset|Момент времени последнего изменения ресурса.  Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|тонов|Коллекция [рубриклевел](rubriclevel.md)|Коллекция уровней, составляющих данный Rubric.|
|являются|Коллекция [рубриккуалити](rubricquality.md)|Коллекция качеств, составляющих этот Rubric.|

## <a name="relationships"></a>Отношения

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