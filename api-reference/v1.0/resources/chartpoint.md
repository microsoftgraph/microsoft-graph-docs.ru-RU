# <a name="chartpoint-resource-type"></a>Тип ресурса ChartPoint

Представляет точку из ряда в диаграмме.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartPoint](../api/chartpoint_get.md) | [ChartPoint](chartpoint.md) |Чтение свойств и связей объекта chartPoint.|
|[Список](../api/chartpoint_list.md) | Коллекция объектов [ChartPoint](chartpoint.md) |Получение коллекции объектов chartPoint. |
|[Itemat](../api/chartpointscollection_itemat.md)|[ChartPoint](chartpoint.md)|Получение точки на основании ее положения в ряду.|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|value|object|Возвращает значение точки диаграммы. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|format|[ChartPointFormat](chartpointformat.md)|Инкапсулирует свойства формата точки диаграммы. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->