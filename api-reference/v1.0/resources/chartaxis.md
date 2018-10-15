# <a name="chartaxis-resource-type"></a>Тип ресурса ChartAxis

Представляет одну ось на диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get ChartAxis](../api/chartaxis_get.md) | [WorkbookChartAxis](chartaxis.md) |Чтение свойств и связей объекта chartAxis.|
|[Update](../api/chartaxis_update.md) | [WorkbookChartAxis](chartaxis.md)   |Обновление объекта ChartAxis. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| id       |string   | Уникальный идентификационный код. Только для чтения.|
|majorUnit|Json|Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.|
|maximum|Json|Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.|
|minimum|Json|Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.|
|minorUnit|Json|Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartAxisFormat](chartaxisformat.md)|Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.|
|majorGridlines|[WorkbookChartGridlines](chartgridlines.md)|Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.|
|minorGridlines|[WorkbookChartGridlines](chartgridlines.md)|Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.|
|title|[WorkbookChartAxisTitle](chartaxistitle.md)|Представляет название оси. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->