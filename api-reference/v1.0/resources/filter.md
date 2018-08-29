# <a name="filter-resource-type"></a>Тип ресурса Filter

Управляет фильтрацией столбца таблицы.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Применить](../api/filter_apply.md)|Нет|Применяет заданные условия фильтра для определенного столбца.|
|[Clear](../api/filter_clear.md)|Нет|Сбрасывает фильтр для определенного столбца.|

## <a name="properties"></a>Свойства

| Имя | Тип   |Описание|
|:---------------|:--------|:----------|
|criteria|[WorkbookFilterCriteria](filtercriteria.md)|Текущий фильтр, заданный для определенного столбца. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->