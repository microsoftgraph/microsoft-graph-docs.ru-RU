---
title: Тип ресурса recurrencePattern
description: Описывает частоту повторения события.
localization_priority: Normal
ms.openlocfilehash: 4798ce7fc33fd6dec7aec1b8c333ae66c917e373
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512264"
---
# <a name="recurrencepattern-resource-type"></a>Тип ресурса recurrencePattern

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает частоту повторения [события](event.md).

В зависимости от того, каков конкретный сценарий, вы можете задать расписание повторения события одним из 6 способов. Для каждого типа расписания необходимо задать временной интервал между повторениями. Фактические экземпляры повторяющегося события всегда соответствуют этому расписанию и происходят в диапазоне дат, указанном для события. Повторяющееся событие всегда определяется соответствующими ресурсами **recurrencePattern** (частотой повторения события) и [recurrenceRange](recurrencerange.md) (продолжительностью повторения).

С помощью свойства **type** можно указывать различные типы объектов **recurrencePattern**, а с помощью свойства **interval** — временной интервал между повторениями, который может быть указан в днях, неделях, месяцах или годах (в зависимости от значения свойства **type**). Обратите внимание на то, какие свойства требуются для каждого типа, как описано в приведенной ниже таблице.

> **Примечание.** Включайте только те свойства, которые требуются для расписания повторения. Любое указанное свойство, для которого не задано допустимое значение, приводит к ошибке.

| Тип расписания повторения | Значение свойства type | Описание | Пример | Обязательные свойства |
|:---------------|:--------|:--------|:--------|:----------|
| С учетом дней | `daily` | Событие повторяется через количество дней, указанное в свойстве **interval**. | Повторение события каждые 3 дня. | **type**, **interval** |
| С учетом недель | `weekly` | Событие повторяется в одни и те же дни недели с учетом указанного количества недель между последовательностями экземпляров. | Повторение события в понедельник и вторник каждую вторую неделю. | **type**, **interval**, **daysOfWeek**, **firstDayOfWeek** |
| С учетом месяцев (на абсолютной основе) | `absoluteMonthly` | Событие повторяется в указанный день месяца (например, 15-го числа) в соответствии с количеством месяцев между повторениями. | Ежеквартальное повторение события (каждые 3 месяца) 15-го числа. | **type**, **interval**, **dayOfMonth** |
| С учетом месяцев (на относительной основе) | `relativeMonthly` | Событие повторяется в указанные дни одной и той же (по счету) недели месяца в соответствии с количеством месяцев между повторениями. | Повторение события во второй четверг или вторую пятницу каждые три месяца. | **type**, **interval**, **daysOfWeek** |
| С учетом количества лет (на абсолютной основе) | `absoluteYearly` | Событие повторяется в указанный день указанного месяца в соответствии с количеством лет между повторениями. | Повторение события 15 марта каждые 3 года. | **type**, **interval**, **dayOfMonth**, **month** |
| С учетом количества лет (на относительной основе) | `relativeYearly` | Событие повторяется в указанные дни одной и той же (по счету) недели определенного месяца в соответствии с количеством лет между повторениями. | Повторение события во второй четверг или вторую пятницу ноября каждые 3 года. | **type**, **interval**, **daysOfWeek**, **month** |


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|День месяца, в который происходит событие. Обязательное, если для **type** задано значение `absoluteMonthly` или `absoluteYearly`. |
|daysOfWeek|Коллекция String|Коллекция дней недели, в которые происходит событие. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. <br>Если для **type** задано значение `relativeMonthly` или `relativeYearly`, а **daysOfWeek** указывает несколько дней, то событие происходит в первый день, соответствующий расписанию. <br> Обязательный параметр, если для **type** задано значение `weekly`, `relativeMonthly` или `relativeYearly`.|
|firstDayOfWeek|String|Первый день недели. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. Значение по умолчанию: `sunday`. Обязательное, если для **type** задано значение `weekly`. |
|index|String|Указывает, в какой из разрешенных дней, указанных в **daysOfsWeek**, происходит событие (начиная с первого экземпляра за месяц). Возможные значения: `first`, `second`, `third`, `fourth`, `last`. Значение по умолчанию: `first`. Необязательное, если для **type** задано значение `relativeMonthly` или `relativeYearly`. |
|interval|Int32|Количество единиц между повторениями. Единицами могут быть дни, недели, месяцы или годы (в зависимости от значения **type**). Обязательный. |
|month|Int32|Месяц, в который происходит событие.  Это число от 1 до 12.|
|type|String|Тип расписания повторения: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly`, `relativeYearly`. Обязательное.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencePattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recurrencepattern.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
