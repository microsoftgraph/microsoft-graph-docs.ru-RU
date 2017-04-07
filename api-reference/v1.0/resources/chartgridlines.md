# <a name="chartgridlines-resource-type"></a>Тип ресурса ChartGridlines

Представляет основные или вспомогательные линии сетки на оси диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartGridlines](../api/chartgridlines_get.md) | [ChartGridlines](chartgridlines.md) |Чтение свойств и связей объекта chartGridlines.|
|[Обновление](../api/chartgridlines_update.md) | [ChartGridlines](chartgridlines.md)    |Обновление объекта ChartGridlines. |

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|visible|boolean|Логическое значение, определяющее, отображаются ли линии сетки оси.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|format|[ChartGridlinesFormat](chartgridlinesformat.md)|Представляет форматирование линий сетки диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->