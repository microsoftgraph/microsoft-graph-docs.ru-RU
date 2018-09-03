# <a name="tablerow-resource-type"></a>Тип ресурса TableRow

Представляет строку в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение TableRow](../api/tablerow_get.md) | [WorkbookTableRow](tablerow.md) |Чтение свойств и связей объекта tableRow.|
|[Обновление](../api/tablerow_update.md) | [WorkbookTableRow](tablerow.md)  |Обновление объекта tableRow. |
|[Range](../api/tablerow_range.md)|[Range](range.md)|Возвращает объект диапазона, связанный со всей строкой.|
|[Удаление](../api/tablerow_delete.md)|Нет|Удаляет строку из таблицы.|
|[Список](../api/tablerow_list.md) | Коллекция [WorkbookTableRow](tablerow.md) |Получение коллекции объектов tableRow. |
|[Itemat](../api/tablerowcollection_itemat.md)|[WorkbookTableRow](tablerow.md)|Получение строки на основании сведений о ее позиции в коллекции.|
|[Add](../api/tablerowcollection_add.md)|[WorkbookTableRow](tablerow.md)|Добавляет новую строку в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|index|int|Возвращает номер индекса строки в коллекции строк таблицы. Используется нулевой индекс. Только для чтения.|
|values|Json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->