# <a name="nameditem-resource-type"></a>Тип ресурса NamedItem

Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта NamedItem](../api/nameditem_get.md) | [NamedItem](nameditem.md) |Чтение свойств и связей объекта namedItem.|
|[Обновление](../api/nameditem_update.md) | [NamedItem](nameditem.md)    |Обновление объекта NamedItem. |
|[Range](../api/nameditem_range.md)|[Range](range.md)|Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.|
|[Список](../api/nameditem_list.md) | Коллекция объектов [NamedItem](nameditem.md) |Получение коллекции объектов namedItem. |

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|name|string|Имя объекта. Только для чтения.|
|type|string|Указывает тип ссылки, связанный с именем. Возможные значения: `String`, `Integer`, `Double`, `Boolean`, `Range`. Только для чтения.|
|значение|object|Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4,75 и т. д. Только для чтения.|
|visible|boolean|Определяет, является ли объект видимым.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.range"},
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->