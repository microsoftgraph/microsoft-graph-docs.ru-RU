# <a name="tablesort-resource-type"></a>Тип ресурса TableSort

Управляет операциями сортировки для объектов Table.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableSort](../api/tablesort_get.md) | [WorkbookTableSort](tablesort.md) |Чтение свойств и связей объекта tableSort.|
|[Apply](../api/tablesort_apply.md)|Нет|Выполняет сортировку.|
|[Clear](../api/tablesort_clear.md)|Нет|Удаляет текущие параметры сортировки таблицы. При этом сбрасывается состояние кнопок в заголовках, но порядок сортировки таблицы остается неизменным.|
|[Reapply](../api/tablesort_reapply.md)|Нет|Повторно применяет текущие параметры сортировки к таблице.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|fields|Коллекция [WorkbookSortField](sortfield.md)|Указывает текущие условия, которые использовались при последней сортировке таблицы. Только для чтения.|
|matchCase|логический|Указывает, учитывался ли регистр при последней сортировке таблице. Только для чтения.|
|method|строка|Представляет метод сортировки китайских знаков, который в последний раз использовался для сортировки таблицы. Возможные значения: `PinYin`, `StrokeCount`. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->