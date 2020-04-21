---
title: Тип ресурса recurrenceRange
description: 'Описывает диапазон дат, согласно которому повторяется событие. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ca2c98cce412843361947b97c330a0b2394f138a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521210"
---
# <a name="recurrencerange-resource-type"></a>Тип ресурса recurrenceRange

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает диапазон дат, согласно которому повторяется [событие](event.md). 

Вы можете задать диапазон дат для повторяющегося события одним из 3 способов (в зависимости от сценария). Необходимо всегда указывать значение **startDate** для диапазона дат, но вы можете задать повторяющееся событие, которое перестает повторяться в определенный день либо повторяется бесконечно или определенное количество раз. Обратите внимание, что фактические экземпляры события в диапазоне дат всегда соответствуют расписанию повторения, заданному для повторяющегося события. Повторяющееся событие всегда определяется соответствующими ресурсами [recurrencePattern](recurrencepattern.md) (частотой повторения события) и **recurrenceRange** (продолжительностью повторения).


## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|endDate|Date|Дата, с которой перестает применяться расписание повторения. В зависимости от того, каково расписание повторения события, последний экземпляр собрания может приходиться на другую дату. Обязательное, если для **type** задано значение `endDate`.|
|numberOfOccurrences|Int32|Количество повторений события. Обязательное свойство, которое должно быть положительным, если для **type** задано значение `numbered`.|
|recurrenceTimeZone|String |Часовой пояс для свойств **startDate** и **endDate**. Необязательное. Если это свойство не задано, используется часовой пояс события.|
|startDate|Date|Дата, с которой начинает применяться расписание повторения. В зависимости от того, каково расписание повторения события, первый экземпляр собрания может приходиться на эту или более позднюю дату. Должно быть задано то же значение, что и для свойства **start** повторяющегося [события](event.md). Обязательное.|
|type|String|Диапазон повторения. Возможные значения: `endDate`, `noEnd`, `numbered`. Обязательное.|

С помощью свойства **type** можно указывать различные типы для **recurrenceRange**. Обратите внимание на обязательные свойства для каждого типа, описанные в приведенной ниже таблице.

| Свойство type  | Тип диапазона повторения | Описание | Пример | Обязательные свойства |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |Диапазон с датой окончания | Событие повторяется во все дни, входящие в соответствующее расписание повторения, с даты **startDate** и до даты **endDate** включительно. | Повторение события с 1 июня 2017 г. до 15 июня 2017 г. | **type**, **startDate**, **endDate** | 
|`noEnd`   |Диапазон без даты окончания | Событие повторяется во все дни, входящие в соответствующее расписание повторения, начиная с даты **startDate**. | Бесконечное повторение события с 1 июня 2017 г. | **type**, **startDate** |
|`numbered`|Диапазон с определенным количеством повторений | Событие повторяется определенное количество раз (указанное в **numberOfOccurrences**) в соответствии с расписанием повторения, начиная с даты **startDate**. | Повторение события 10 раз с 1 июня 2017 г.  | **type**, **startDate**, **numberOfOccurrences** |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/recurrencerange.md:\r\n      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |"
  ]
}
-->
