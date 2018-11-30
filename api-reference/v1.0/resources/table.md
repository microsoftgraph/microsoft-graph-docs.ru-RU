---
title: Тип ресурса Table
description: Представляет таблицу Excel.
ms.openlocfilehash: 029f2477570b6ad1c85f6c92d64fd25d3ae8dac0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026635"
---
# <a name="table-resource-type"></a>Тип ресурса Table

Представляет таблицу Excel.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Table](../api/table-get.md) | [WorkbookTable](table.md) |Чтение свойств и связей объекта таблицы.|
|[Создание объекта TableColumn](../api/table-post-columns.md) |[WorkbookTableColumn](tablecolumn.md)| Создание объекта TableColumn путем добавления в коллекцию столбцов.|
|[Список столбцов](../api/table-list-columns.md) |[WorkbookTableColumn](tablecolumn.md) коллекции| Получение коллекции объектов TableColumn.|
|[Создание объекта TableRow](../api/table-post-rows.md) |[WorkbookTableRow](tablerow.md)| Создание объекта TableRow путем добавления в коллекцию строк.|
|[Список строк](../api/table-list-rows.md) |[WorkbookTableRow](tablerow.md) коллекции| Получение коллекции объектов TableRow.|
|[Обновление](../api/table-update.md) | [WorkbookTable](table.md)   |Обновление объекта Table. |
|[Databodyrange](../api/table-databodyrange.md)|[Range](range.md)|Получает объект диапазона, связанный с основными данными таблицы.|
|[Headerrowrange](../api/table-headerrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой заголовков таблицы.|
|[Range](../api/table-range.md)|[Range](range.md)|Получает объект диапазона, связанный со всей таблицей.|
|[Totalrowrange](../api/table-totalrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой итогов таблицы.|
|[Clearfilters](../api/table-clearfilters.md)|Нет|Удаляет все фильтры, примененные к таблице.|
|[Converttorange](../api/table-converttorange.md)|[Range](range.md)|Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.|
|[Delete](../api/table-delete.md)|Нет|Удаляет таблицу.|
|[Reapplyfilters](../api/table-reapplyfilters.md)|Нет|Повторно применяет все текущие фильтры к таблице.|
|[Список](../api/table-list.md) | [WorkbookTable](table.md) коллекции |Получение коллекции объектов table. |
|[Add](../api/tablecollection-add.md)|[WorkbookTable](table.md)|Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|строка|Возвращает значение, однозначно идентифицирующее таблицу в данной книге. Значение идентификатора остается прежним, даже если переименовать таблицу. Это свойство должно интерпретироваться как непрозрачное строковое значение и не должно преобразовываться в любой другой тип. Только для чтения.|
|name|строка|Имя таблицы.|
|showHeaders|boolean|Указывает, отображается ли строка заголовков. Можно задать это значение, чтобы отобразить или скрыть строку заголовков.|
|showTotals|boolean|Указывает, отображается ли строка итогов. Можно задать это значение, чтобы отобразить или скрыть строку итогов.|
|style|строка|Постоянное значение, представляющее стиля таблицы. Возможные значения: TableStyleLight1 через TableStyleLight21, TableStyleMedium1 через TableStyleMedium28, TableStyleStyleDark1 через TableStyleStyleDark11. Также можно указать настраиваемых пользовательских стиля присутствует в книге.|
|highlightFirstColumn|Boolean|Указывает, содержит ли первый столбец специальное форматирование.   |
|highlightLastColumn|Boolean|Указывает, содержит ли последний столбец специальное форматирование. |
|showBandedColumns|Boolean|Указывает, чередуется ли форматирование четных и нечетных столбцов для более удобного просмотра таблицы.   |
|showBandedRows|Boolean|Указывает, чередуется ли форматирование четных и нечетных строк для более удобного просмотра таблицы.    |
|showFilterButton|Boolean|Указывает, видны ли кнопки фильтрации в верхней части заголовков столбцов. Это свойство можно использовать, только если таблица содержит строку заголовков.   |
|legacyId|String|Устаревший идентификатор, используемый в старых клиентах Excel. Значение идентификатора остается прежним, даже если переименовать таблицу. Это свойство должно интерпретироваться как непрозрачное строковое значение и не должно преобразовываться в любой другой тип. Только для чтения.   |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|columns|[WorkbookTableColumn](tablecolumn.md) коллекции|Представляет коллекцию всех столбцов в таблице. Только для чтения.|
|rows|[WorkbookTableRow](tablerow.md) коллекции|Представляет коллекцию всех строк в таблице. Только для чтения.|
|sort|[WorkbookTableSort](tablesort.md)|Представляет сортировку для таблицы. Только для чтения.|
|лист|[WorkbookWorksheet](worksheet.md)|Лист, содержащий текущую таблицу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTable"
}-->

```json
{
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "id": "String (identifier)",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String",
  "legacyId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
