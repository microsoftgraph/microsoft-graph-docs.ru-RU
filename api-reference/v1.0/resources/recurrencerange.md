# <a name="recurrencerange-resource-type"></a>Тип ресурса recurrenceRange

Продолжительность события.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|endDate|Date|Дата окончания ряда.|
|numberOfOccurrences|Int32|Количество повторений события.|
|recurrenceTimeZone|String |Часовой пояс для свойств **startDate** и **endDate**. |
|startDate|Date|Дата начала ряда.|
|type|String|Диапазон повторения: EndDate = 0, NoEnd = 1, Numbered = 2. Возможные значения: `EndDate`, `NoEnd`, `Numbered`.||

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
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
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
