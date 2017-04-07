# <a name="charttitle-resource-type"></a>Тип ресурса ChartTitle

Представляет объект заголовка диаграммы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта ChartTitle](../api/charttitle_get.md) | [ChartTitle](charttitle.md) |Чтение свойств и связей объекта chartTitle.|
|[Обновление](../api/charttitle_update.md) | [ChartTitle](charttitle.md)    |Обновление объекта ChartTitle. |

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|overlay|boolean|Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.|
|text|string|Представляет текст заголовка диаграммы.|
|visible|boolean|Логическое значение, представляющее видимость объекта заголовка диаграммы.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|format|[ChartTitleFormat](charttitleformat.md)|Представляет форматирование названия диаграммы, включая формат заливки и шрифта. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->