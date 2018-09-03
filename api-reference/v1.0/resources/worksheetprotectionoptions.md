# <a name="worksheetprotectionoptions-resource-type"></a>Тип ресурса WorksheetProtectionOptions

Представляет параметры защиты листа.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowAutoFilter|boolean (логический)|Представляет параметр защиты листа, разрешающий использовать функцию автофильтра.|
|allowDeleteColumns|boolean (логический)|Представляет параметр защиты листа, разрешающий удалять столбцы.|
|allowDeleteRows|boolean (логический)|Представляет параметр защиты листа, разрешающий удалять строки.|
|allowFormatCells|boolean (логический)|Представляет параметр защиты листа, разрешающий форматировать ячейки.|
|allowFormatColumns|boolean (логический)|Представляет параметр защиты листа, разрешающий форматировать столбцы.|
|allowFormatRows|boolean (логический)|Представляет параметр защиты листа, разрешающий форматировать строки.|
|allowInsertColumns|boolean (логический)|Представляет параметр защиты листа, разрешающий вставлять столбцы.|
|allowInsertHyperlinks|boolean (логический)|Представляет параметр защиты листа, разрешающий вставлять гиперссылки.|
|allowInsertRows|boolean (логический)|Представляет параметр защиты листа, разрешающий вставлять строки.|
|allowPivotTables|boolean (логический)|Представляет параметр защиты листа, разрешающий использовать функцию сводных таблиц.|
|allowSort|boolean (логический)|Представляет параметр защиты листа, разрешающий использовать функцию сортировки.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions"
}-->

```json
{
  "allowAutoFilter": true,
  "allowDeleteColumns": true,
  "allowDeleteRows": true,
  "allowFormatCells": true,
  "allowFormatColumns": true,
  "allowFormatRows": true,
  "allowInsertColumns": true,
  "allowInsertHyperlinks": true,
  "allowInsertRows": true,
  "allowPivotTables": true,
  "allowSort": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtectionOptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->