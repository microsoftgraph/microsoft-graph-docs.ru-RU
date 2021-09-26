---
title: Тип ресурса Table
description: Представляет таблицу Excel.
author: lumine2008
ms.localizationpriority: high
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 35764b91133a943f378df3aaa359447727249ec3
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764005"
---
# <a name="table-resource-type"></a>Тип ресурса Table

Пространство имен: microsoft.graph

Представляет таблицу Excel.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Table](../api/table-get.md) | [WorkbookTable](table.md) |Чтение свойств и связей объекта таблицы.|
|[Создание объекта TableColumn](../api/table-post-columns.md) |[WorkbookTableColumn](workbooktablecolumn.md)| Создание объекта TableColumn путем добавления в коллекцию столбцов.|
|[Список столбцов](../api/table-list-columns.md) |Коллекция [WorkbookTableColumn](workbooktablecolumn.md)| Получение коллекции объектов TableColumn.|
|[Создание объекта TableRow](../api/table-post-rows.md) |[WorkbookTableRow]( workbooktablerow.md)| Создание объекта TableRow путем добавления в коллекцию строк.|
|[Список строк](../api/table-list-rows.md) |Коллекция [WorkbookTableRow]( workbooktablerow.md)| Получение коллекции объектов TableRow.|
|[Update](../api/table-update.md) | [WorkbookTable](table.md)   |Обновление объекта Table. |
|[Databodyrange](../api/table-databodyrange.md)|[Range](range.md)|Получает объект диапазона, связанный с основными данными таблицы.|
|[Headerrowrange](../api/table-headerrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой заголовков таблицы.|
|[Range](../api/table-range.md)|[Range](range.md)|Получает объект диапазона, связанный со всей таблицей.|
|[Totalrowrange](../api/table-totalrowrange.md)|[Range](range.md)|Получает объект диапазона, связанный со строкой итогов таблицы.|
|[Clearfilters](../api/table-clearfilters.md)|Нет|Удаляет все фильтры, примененные к таблице.|
|[Converttorange](../api/table-converttorange.md)|[Range](range.md)|Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.|
|[Delete](../api/table-delete.md)|Нет|Удаляет таблицу.|
|[Reapplyfilters](../api/table-reapplyfilters.md)|Нет|Повторно применяет все текущие фильтры к таблице.|
|[List](../api/table-list.md) | Коллекция [WorkbookTable](table.md) |Получение коллекции объектов table. |
|[Add](../api/tablecollection-add.md)|[WorkbookTable](table.md)|Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|string|Возвращает значение, однозначно идентифицирующее таблицу в данной книге. Значение идентификатора остается прежним, даже если переименовать таблицу. Это свойство должно интерпретироваться как непрозрачное строковое значение и не должно преобразовываться в любой другой тип. Только для чтения.|
|name|string|Имя таблицы.|
|showHeaders|boolean|Указывает, отображается ли строка заголовков. Можно задать это значение, чтобы отобразить или скрыть строку заголовков.|
|showTotals|boolean|Указывает, отображается ли строка итогов. Можно задать это значение, чтобы отобразить или скрыть строку итогов.|
|style|string|Постоянное значение, представляющее стиль таблицы. Возможные значения: от TableStyleLight1 до TableStyleLight21, от TableStyleMedium1 до TableStyleMedium28, от TableStyleStyleDark1 до TableStyleStyleDark11. Также можно указать настраиваемый пользовательский стиль, имеющийся в книге.|
|highlightFirstColumn|Boolean|Указывает, содержит ли первый столбец специальное форматирование.   |
|highlightLastColumn|Boolean|Указывает, содержит ли последний столбец специальное форматирование. |
|showBandedColumns|Boolean|Указывает, чередуется ли форматирование четных и нечетных столбцов для более удобного просмотра таблицы.   |
|showBandedRows|Boolean|Указывает, чередуется ли форматирование четных и нечетных строк для более удобного просмотра таблицы.    |
|showFilterButton|Boolean|Указывает, видны ли кнопки фильтрации в верхней части заголовков столбцов. Это свойство можно использовать, только если таблица содержит строку заголовков.   |
|legacyId|String|Устаревший идентификатор, используемый в старых клиентах Excel. Значение идентификатора остается прежним, даже если переименовать таблицу. Это свойство должно интерпретироваться как непрозрачное строковое значение и не должно преобразовываться в любой другой тип. Только для чтения.   |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|columns|Коллекция [WorkbookTableColumn](workbooktablecolumn.md)|Представляет коллекцию всех столбцов в таблице. Только для чтения.|
|rows|Коллекция [WorkbookTableRow]( workbooktablerow.md)|Представляет коллекцию всех строк в таблице. Только для чтения.|
|sort|[WorkbookTableSort](tablesort.md)|Представляет сортировку для таблицы. Только для чтения.|
|worksheet|[WorkbookWorksheet](worksheet.md)|Лист, содержащий текущую таблицу. Только для чтения.|

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

