# <a name="chart-resource-type"></a>Тип ресурса Chart

Представляет объект диаграммы в книге.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Chart](../api/chart_get.md) | [Chart](chart.md) |Чтение свойств и связей объекта диаграммы.|
|[Создание объекта ChartSeries](../api/chart_post_series.md) |[ChartSeries](chartseries.md)| Создание объекта ChartSeries путем добавления в коллекцию рядов.|
|[Список рядов](../api/chart_list_series.md) |Коллекция объектов [ChartSeries](chartseries.md)| Получение коллекции объектов ChartSeries.|
|[Обновление](../api/chart_update.md) | [Chart](chart.md)    |Обновление объекта Chart. |
|[Image](../api/chart_image.md)|Строка изображения с кодировкой base64|Отрисовывает диаграмму в виде изображения с кодировкой base64, масштабируя ее в соответствии с указанным размером.|
|[Delete](../api/chart_delete.md)|Нет|Удаляет объект диаграммы.|
|[Setdata](../api/chart_setdata.md)|Нет|Сбрасывает исходные данные для диаграммы.|
|[Setposition](../api/chart_setposition.md)|Нет|Располагает диаграмму относительно ячеек на листе.|
|[Список](../api/chart_list.md) | Коллекция объектов [Chart](chart.md) |Получение коллекции объектов диаграмм. |
|[Itemat](../api/chartcollection_itemat.md)|[Chart](chart.md)|Возвращает диаграмму с учетом ее положения в коллекции.|
|[Add](../api/chartcollection_add.md)|[Chart](chart.md)|Создает диаграмму.|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|height|double|Обозначает высоту объекта диаграммы (в пунктах).|
|id|string|Возвращает диаграмму с учетом ее положения в коллекции. Только для чтения.|
|left|double|Расстояние в пунктах от левого края диаграммы до начала листа.|
|name|string|Обозначает имя объекта диаграммы.|
|top|double|Представляет расстояние в пунктах от верхнего края объекта до верхнего края первой строки (на листе) или до верхнего края области диаграммы (на диаграмме).|
|width|double|Представляет ширину объекта диаграммы (в пунктах).|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|axes|[ChartAxes](chartaxes.md)|Представляет оси диаграммы. Только для чтения.|
|dataLabels|[ChartDataLabels](chartdatalabels.md)|Представляет метки данных на диаграмме. Только для чтения.|
|format|[ChartAreaFormat](chartareaformat.md)|Инкапсулирует свойства формата для области диаграммы. Только для чтения.|
|legend|[ChartLegend](chartlegend.md)|Представляет условные обозначения для диаграммы. Только для чтения.|
|series|Коллекция объектов [ChartSeries](chartseries.md)|Представляет один ряд данных или коллекцию рядов данных в диаграмме. Только для чтения.|
|title|[ChartTitle](charttitle.md)|Представляет заголовок указанной диаграммы, включая его текст, видимость, положение и форматирование. Только для чтения.|
|лист|[Worksheet](worksheet.md)|Лист, содержащий текущую диаграмму. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->