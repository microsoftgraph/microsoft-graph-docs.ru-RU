# <a name="worksheetprotection-resource-type"></a>Тип ресурса WorksheetProtection

Представляет защиту объекта листа.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта WorksheetProtection](../api/worksheetprotection_get.md) | [WorksheetProtection](worksheetprotection.md) |Чтение свойств и связей объекта worksheetProtection.|
|[Protect](../api/worksheetprotection_protect.md)|Нет|Защита листа. Выдает исключение, если лист защищен.|
|[Unprotect](../api/worksheetprotection_unprotect.md)|Нет|Снятие защиты с листа|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|protected|boolean|Указывает, защищен ли лист.  Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|options|[WorksheetProtectionOptions](worksheetprotectionoptions.md)|Параметры защиты листа. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->