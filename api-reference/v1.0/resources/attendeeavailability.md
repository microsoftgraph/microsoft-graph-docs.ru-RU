# <a name="attendeeavailability-resource-type"></a>Тип ресурсов attendeeAvailability

Тип и занятость участника.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|attendee|[AttendeeBase](attendeebase.md)|Тип участника (сведения о том, является ли участник пользователем или ресурсом, а также о том, обязательный ли он, если объект представляет пользователя).|
|availability|Строка| Состояние занятости участника. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->