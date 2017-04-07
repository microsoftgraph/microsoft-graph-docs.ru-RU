# <a name="timeconstraint-resource-type"></a>Тип ресурсов timeConstraint

Периоды времени для указанного действия.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|activityDomain|String|Описание действия (необязательно). Возможные значения: `unknown`, `work`, `personal`. [findMeetingTimes](../api/user_findmeetingtimes.md) всегда действует так, будто задано значение `work`, и возвращает варианты собраний (если таковые находятся) только в рабочие часы организатора или участника.|
|timeslots|Коллекция [timeSlot](timeslot.md)|Массив, содержащий значения периодов времени.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->