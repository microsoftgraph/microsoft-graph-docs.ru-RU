# <a name="chartlegend-resource-type"></a>Тип ресурса ChartLegend

Представляет легенду в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartLegend](../api/chartlegend_get.md) | [WorkbookChartLegend](chartlegend.md) |Чтение свойств и связей объекта chartLegend.|
|[Update](../api/chartlegend_update.md) | [WorkbookChartLegend](chartlegend.md) |Обновление объекта ChartLegend. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|overlay|boolean (логический)|Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.|
|position|string (строка)|Представляет положение условного обозначения диаграммы. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`,`Custom`.|
|visible|boolean (логический)|Логическое значение, представляющее видимость объекта ChartLegend.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartLegendFormat](chartlegendformat.md)|Представляет форматирование условного обозначения диаграммы, включая заливку и шрифт. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->