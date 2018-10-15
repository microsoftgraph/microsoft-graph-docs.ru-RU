# <a name="worksheet-resource-type"></a>Тип ресурса Worksheet

Лист Excel представляет собой сетку ячеек. Он может содержать данные, таблицы, диаграммы и т. д.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get Worksheet](../api/worksheet_get.md) | [WorkbookWorksheet](worksheet.md) |Чтение свойств и связей объекта worksheet (лист).|
|[Create Chart](../api/worksheet_post_charts.md) |[WorkbookChart](chart.md)| Создание нового объекта Chart (диаграмма) путем добавления в коллекцию диаграмм.|
|[List names](../api/worksheet_list_names.md) |Коллекция [WorkbookNamedItem](nameditem.md)| Получение коллекции именованных элементов, связанной с листом.|
|[List charts](../api/worksheet_list_charts.md) |Коллекция [WorkbookChart](chart.md)| Получение коллекции объектов Chart (диаграмма).|
|[Create Table](../api/worksheet_post_tables.md) |[WorkbookTable](table.md)| Создание нового объекта Table (таблица) путем добавления в коллекцию таблиц.|
|[List tables](../api/worksheet_list_tables.md) |Коллекция [WorkbookTable](table.md)| Получение коллекции объектов Table (таблица).|
|[Update](../api/worksheet_update.md) | [WorkbookWorksheet](worksheet.md)   |Обновление объекта Worksheet (лист). |
|[Cell](../api/worksheet_cell.md)|[Range](range.md)|Получает объект диапазона, содержащий одну ячейку, на основе номеров строки и столбца. Ячейка может выходить за пределы родительского диапазона, если она расположена в сетке листа.|
|[Range](../api/worksheet_range.md)|[Range](range.md)|Возвращает объект range (диапазон), указанный по адресу или имени.|
|[Usedrange](../api/worksheet_usedrange.md)|[Range](range.md)|Используемый диапазон — это наименьший диапазон, включающий в себя все ячейки, которые содержат значение или форматирование. Если лист пустой, эта функция вернет верхнюю левую ячейку.|
|[Delete](../api/worksheet_delete.md)|Нет|Удаляет лист из книги.|
|[List](../api/worksheet_list.md) | Коллекция [WorkbookWorksheet](worksheet.md) |Получение коллекции объектов worksheet (лист). |
|[Add](../api/worksheetcollection_add.md)|[WorkbookWorksheet](worksheet.md)|Добавляет новый объект worksheet (лист) в книгу. Лист будет добавлен после существующих листов. |
|[List pivotTables](../api/workbookworksheet_list_pivottables.md) |Коллекция [workbookPivotTable](workbookpivottable.md)| Получение коллекции объектов workbookPivotTable.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Возвращает значение, однозначно идентифицирующее лист в данной книге. Значение идентификатора остается прежним, даже если переименовать или переместить лист. Только для чтения.|
|name|string|Отображаемое имя листа.|
|position|int|Положение листа (начиная с нуля) в книге.|
|visibility|string|Видимость листа. Возможные значения: `Visible`, `Hidden`, `VeryHidden`.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|charts|Коллекция [WorkbookChart](chart.md)|Возвращает коллекцию диаграмм, имеющихся на листе. Только для чтения.|
|names|Коллекция [WorkbookNamedItem](nameditem.md)|Возвращает коллекцию имен, связанных с листом. Только для чтения.|
|pivotTables|Коллекция [workbookPivotTable](workbookpivottable.md)| Коллекция сводных таблиц на листе. |
|protection|[WorkbookWorksheetProtection](worksheetprotection.md)|Возвращает объект sheet protection (защита листа) для листа. Только для чтения.|
|tables|Коллекция [WorkbookTable](table.md)|Коллекция таблиц, имеющихся на листе. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
