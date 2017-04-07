# <a name="rangefill-resource-type"></a>Тип ресурса RangeFill

Представляет фон объекта диапазона.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeFill](../api/rangefill_get.md) | [RangeFill](rangefill.md) |Чтение свойств и связей объекта rangeFill.|
|[Обновление](../api/rangefill_update.md) | [RangeFill](rangefill.md)    |Обновление объекта RangeFill. |
|[Clear](../api/rangefill_clear.md)|Нет|Сбрасывает фон диапазона.|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|color|string|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->