# <a name="rangeformat-resource-type"></a>Тип ресурса RangeFormat

Объект формата, в который включены шрифт, заливка, границы, выравнивание и другие свойства диапазона.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeFormat](../api/rangeformat_get.md) | [WorkbookRangeFormat](rangeformat.md) |Чтение свойств и связей объекта rangeFormat.|
|[Создание объекта RangeBorder](../api/rangeformat_post_borders.md) |[WorkbookRangeBorder](rangeborder.md)| Создание объекта RangeBorder путем добавления в коллекцию границ.|
|[Список границ](../api/rangeformat_list_borders.md) |Коллекция [WorkbookRangeBorder](rangeborder.md)| Получение коллекции объектов RangeBorder.|
|[Обновление](../api/rangeformat_update.md) | [WorkbookRangeFormat](rangeformat.md) |Обновление объекта RangeFormat. |
|[Autofitcolumns](../api/rangeformat_autofitcolumns.md)|Нет|Изменяет ширину столбцов текущего диапазона на оптимальную с учетом текущих данных в столбцах.|
|[Autofitrows](../api/rangeformat_autofitrows.md)|Нет|Изменяет высоту строк текущего диапазона на оптимальную с учетом текущих данных в столбцах.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|columnWidth|double|Возвращает или задает ширину всех столбцов в пределах диапазона. Если столбцы разной ширины, будет возвращено значение NULL.|
|horizontalAlignment|строка|Представляет горизонтальное выравнивание для указанного объекта. Возможные значения: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.|
|rowHeight|double|Возвращает или задает высоту всех строк в диапазоне. Если строки разной высоты, будет возвращено значение NULL.|
|verticalAlignment|строка|Представляет вертикальное выравнивание для указанного объекта. Возможные значения: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.|
|wrapText|логический|Указывает, использует ли Excel обтекание текстом для объекта. Значение null указывает, что для диапазона в целом не применяется согласованный параметр обтекания.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|borders|Коллекция [WorkbookRangeBorder](rangeborder.md)|Коллекция объектов границ, которые применяются к общему выделенному диапазону. Только для чтения.|
|fill|[WorkbookRangeFill](rangefill.md)|Возвращает объект заливки, определенный для всего диапазона. Только для чтения.|
|font|[WorkbookRangeFont](rangefont.md)|Возвращает объект шрифта, определенный для общего выбранного диапазона. Только для чтения.|
|protection|[WorkbookFormatProtection](formatprotection.md)|Возвращает объект защиты формата для диапазона. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->