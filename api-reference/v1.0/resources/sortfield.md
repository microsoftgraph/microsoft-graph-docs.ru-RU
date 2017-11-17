# <a name="sortfield-resource-type"></a>Тип ресурса SortField

Представляет условие в операции сортировки.

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|ascending|boolean|Указывает, выполняется ли сортировка по возрастанию.|
|color|string|Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.|
|dataOption|string|Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.|
|key|int|Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).|
|sortOn|string|Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|icon|[Icon](icon.md)|Представляет целевой значок условия при сортировке по значку ячейки.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
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