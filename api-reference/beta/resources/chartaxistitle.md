# <a name="chartaxistitle-resource-type"></a>Тип ресурса ChartAxisTitle

Представляет название оси диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartAxisTitle](../api/chartaxistitle_get.md) | [ChartAxisTitle](chartaxistitle.md) |Чтение свойств и связей объекта chartAxisTitle.|
|[Обновление](../api/chartaxistitle_update.md) | [ChartAxisTitle](chartaxistitle.md)    |Обновление объекта ChartAxisTitle. |

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|text|string|Обозначает название оси.|
|visible|boolean|Логическое значение, которое определяет видимость названия оси.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|format|[ChartAxisTitleFormat](chartaxistitleformat.md)|Представляет форматирование для названия оси диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->