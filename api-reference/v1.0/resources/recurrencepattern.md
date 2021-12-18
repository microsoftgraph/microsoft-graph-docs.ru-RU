---
title: Тип ресурса recurrencePattern
description: 'Описывает частоту повторения события. '
ms.localizationpriority: medium
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f267f0b934eae9c0c5a85a02da8f5785bc262892
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545366"
---
# <a name="recurrencepattern-resource-type"></a>Тип ресурса recurrencePattern

Пространство имен: microsoft.graph

Описывает частоту повторения события. Этот общий объект используется для определения повторения [](event.md)обзоров [доступа,](accessreviewscheduledefinition.md)событий календаря и назначений пакетов доступа [в](accesspackageassignment.md) Azure AD.

В зависимости от того, каков конкретный сценарий, вы можете задать расписание повторения события одним из 6 способов. Для каждого типа расписания необходимо задать временной интервал между повторениями. Фактические экземпляры повторяющегося события всегда соответствуют этому расписанию и происходят в диапазоне дат, указанном для события. Повторяющееся событие всегда определяется соответствующими ресурсами **recurrencePattern** (частотой повторения события) и [recurrenceRange](recurrencerange.md) (продолжительностью повторения).

С помощью свойства **type** можно указывать различные типы объектов **recurrencePattern**, а с помощью свойства **interval** — временной интервал между повторениями, который может быть указан в днях, неделях, месяцах или годах (в зависимости от значения свойства **type**). Обратите внимание на то, какие свойства требуются для каждого типа, как описано в приведенной ниже таблице.

> **Примечание.** Включайте только те свойства, которые требуются для расписания повторения. Любое указанное свойство, для которого не задано допустимое значение, приводит к ошибке.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|День месяца, в который происходит событие. Обязательное, если для **type** задано значение `absoluteMonthly` или `absoluteYearly`. |
|daysOfWeek|коллекция dayOfWeek|Коллекция дней недели, в которые происходит событие. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. <br>Если для **type** задано значение `relativeMonthly` или `relativeYearly`, а **daysOfWeek** указывает несколько дней, то событие происходит в первый день, соответствующий расписанию. <br> Обязательный параметр, если для **type** задано значение `weekly`, `relativeMonthly` или `relativeYearly`.|
|firstDayOfWeek|dayOfWeek|Первый день недели. Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. Значение по умолчанию: `sunday`. Обязательное, если для **type** задано значение `weekly`. |
|index|weekIndex|Указывает, в какой экземпляр разрешенных дней, указанных в **daysOfWeek,** происходит событие, засчитано из первой инстанции в месяц. Допустимые значения: `first`, `second`, `third`, `fourth`, `last`. Значение по умолчанию: `first`. Необязательное, если для **type** задано значение `relativeMonthly` или `relativeYearly`. |
|interval|Int32|Количество единиц между повторениями. Единицами могут быть дни, недели, месяцы или годы (в зависимости от значения **type**). Обязательное. |
|month|Int32|Месяц, в который происходит событие.  Это число от 1 до 12.|
|type|recurrencePatternType|Тип расписания повторения: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly`, `relativeYearly`. Обязательное. Дополнительные сведения см. [в добавлении значений свойства типа](#values-of-type-property).|

> [!IMPORTANT]
> Для отзывов о доступе поддерживаются только **свойства dayOfMonth,** **интервал** и тип **(** `weekly` , ). `absoluteMonthly`

### <a name="values-of-type-property"></a>Значения свойства типа

<!-- Note that this isn't a compliant enums declaration format. The recurrencePatternType enum has been declared in the enums.md file so that this H3 section can be customized to provide additional details -->

| Значение свойства type | Описание | Пример | Обязательные свойства |
|:--------|:--------|:--------|:----------|
| `daily` | Событие повторяется через количество дней, указанное в свойстве **interval**. | Повторение события каждые 3 дня. | **type**, **interval** |
| `weekly` | Событие повторяется в одни и те же дни недели с учетом указанного количества недель между последовательностями экземпляров. | Повторение события в понедельник и вторник каждую вторую неделю. | **type**, **interval**, **daysOfWeek**, **firstDayOfWeek**  <br/><br/> **Примечание:** Для отзывов о **доступе поддерживаются** только свойства интервала **и** типа.|
| `absoluteMonthly` | Событие повторяется в указанный день месяца (например, 15-го числа) в соответствии с количеством месяцев между повторениями. | Ежеквартальное повторение события (каждые 3 месяца) 15-го числа. | **type**, **interval**, **dayOfMonth** <br/><br/> **Примечание:** Для обзоров доступа **поддерживается только интервал,** **dayOfMonth** и **свойства** типа.|
| `relativeMonthly` | Событие повторяется в указанные дни одной и той же (по счету) недели месяца в соответствии с количеством месяцев между повторениями. | Повторение события во второй четверг или вторую пятницу каждые три месяца. | **type**, **interval**, **daysOfWeek** |
| `absoluteYearly` | Событие повторяется в указанный день указанного месяца в соответствии с количеством лет между повторениями. | Повторение события 15 марта каждые 3 года. | **type**, **interval**, **dayOfMonth**, **month** |
| `relativeYearly` | Событие повторяется в указанные дни одной и той же (по счету) недели определенного месяца в соответствии с количеством лет между повторениями. | Повторение события во второй четверг или вторую пятницу ноября каждые 3 года. | **type**, **interval**, **daysOfWeek**, **month** |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/recurrencepattern.md/microsoft.graph.recurrencePattern/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->

