# <a name="recurrencepattern-resource-type"></a>Тип ресурса recurrencePattern

Частота события.


## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|День месяца, в который происходит событие.|
|daysOfWeek|Коллекция строк|Коллекция дней недели, в которые происходит событие. Возможные значения: `Sunday`, `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday`, `Saturday`.|
|firstDayOfWeek|String|День недели, с которого начинается повторение. Возможные значения: `Sunday`, `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday`, `Saturday`.|
|индекс|String|Индекс недели, с которой начинается повторение: `First`, `Second`, `Third`, `Fourth`, `Last`.|
|interval|Int32|Количество единиц заданного типа между повторениями.|
|month|Int32|Месяц, в котором происходит событие.  Это число от 1 до 12.|
|type|String|Тип расписания повторения: `Daily`, `Weekly`, `AbsoluteMonthly`, `RelativeMonthly`, `AbsoluteYearly`, `RelativeYearly`.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencepattern"
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
  "tocPath": ""
}-->