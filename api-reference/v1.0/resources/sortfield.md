# <a name="sortfield-resource-type"></a>Тип ресурса SortField

Представляет условие в операции сортировки.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|ascending|логический|Указывает, выполняется ли сортировка по возрастанию.|
|color|строка|Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.|
|dataOption|строка|Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.|
|key|int|Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).|
|sortOn|строка|Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.|
|icon|[WorkbookIcon](icon.md)|Представляет целевой значок условия при сортировке по значку ячейки.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->