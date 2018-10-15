# <a name="chartseries-resource-type"></a>Тип ресурса ChartSeries

Представляет ряд в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartSeries](../api/chartseries_get.md) | [WorkbookChartSeries](chartseries.md) |Чтение свойств и связей объекта chartSeries.|
|[Создание объекта ChartPoints](../api/chartseries_post_points.md) |[ChartPoints](chartpoint.md)| Создание объекта ChartPoints путем добавления в коллекцию точек.|
|[Список точек](../api/chartseries_list_points.md) |Коллекция объектов [ChartPoints](chartpoint.md)| Получение коллекции объектов ChartPoints.|
|[Обновление](../api/chartseries_update.md) | [WorkbookChartSeries](chartseries.md) |Обновление объекта ChartSeries. |
|[Список](../api/chartseries_list.md) | Коллекция [WorkbookChartSeries](chartseries.md) |Получение коллекции объектов chartSeries. |
|[ItemAt](../api/chartseriescollection_itemat.md)|[WorkbookChartSeries](chartseries.md)|Возвращает ряд на основании сведений о его позиции в коллекции.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|name|string (строка)|Представляет имя ряда в диаграмме.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|format|[WorkbookChartSeriesFormat](chartseriesformat.md)|Представляет форматирование ряда диаграммы, включая формат заливки и линий. Только для чтения.|
|points|Коллекция [WorkbookChartPoint](chartpoint.md)|Представляет коллекцию всех точек в ряду. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->