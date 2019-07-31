---
title: Тип ресурса Воркбуктабле
description: Представляет таблицу Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1568cc1f08ded8ffdbac04e040bccefe63e9dd02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963887"
---
# <a name="workbooktable-resource-type"></a>Тип ресурса Воркбуктабле

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет таблицу Excel.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбуктабле](../api/table-get.md) | [Воркбуктабле](workbooktable.md) |Чтение свойств и связей объекта таблицы.|
|[Создание Воркбуктаблеколумн](../api/table-post-columns.md) |[Воркбуктаблеколумн](workbooktablecolumn.md)| Создание объекта TableColumn путем добавления в коллекцию столбцов.|
|[Список столбцов](../api/table-list-columns.md) |Коллекция [воркбуктаблеколумн](workbooktablecolumn.md)| Получение коллекции объектов TableColumn.|
|[Создание Воркбуктаблеров](../api/table-post-rows.md) |[Воркбуктаблеров](workbooktablerow.md)| Создание объекта TableRow путем добавления в коллекцию строк.|
|[Список строк](../api/table-list-rows.md) |Коллекция [воркбуктаблеров](workbooktablerow.md)| Получение коллекции объектов TableRow.|
|[Update](../api/table-update.md) | [Воркбуктабле](workbooktable.md)   |Обновление объекта Table. |
|[Databodyrange](../api/table-databodyrange.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный с основными данными таблицы.|
|[Headerrowrange](../api/table-headerrowrange.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со строкой заголовков таблицы.|
|[Range](../api/table-range.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со всей таблицей.|
|[Totalrowrange](../api/table-totalrowrange.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со строкой итогов таблицы.|
|[Clearfilters](../api/table-clearfilters.md)|Нет|Удаляет все фильтры, примененные к таблице.|
|[Converttorange](../api/table-converttorange.md)|[workbookRange](workbookrange.md)|Преобразовывает таблицу в обычный диапазон ячеек. Все данные сохраняются.|
|[Delete](../api/table-delete.md)|Нет.|Удаляет таблицу.|
|[Reapplyfilters](../api/table-reapplyfilters.md)|Нет|Повторно применяет все текущие фильтры к таблице.|
|[List](../api/table-list.md) | Коллекция [воркбуктабле](workbooktable.md) |Получение коллекции объектов table. |
|[Add](../api/tablecollection-add.md)|[Воркбуктабле](workbooktable.md)|Создание таблицы. Исходный адрес диапазона определяет лист, на который будет добавлена таблица. Если не удается добавить таблицу (например, если адрес недействителен или одна таблица будет перекрываться другой), выводится сообщение об ошибке.|

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

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|columns|Коллекция [воркбуктаблеколумн](workbooktablecolumn.md)|Представляет коллекцию всех столбцов в таблице. Только для чтения.|
|rows|Коллекция [воркбуктаблеров](workbooktablerow.md)|Представляет коллекцию всех строк в таблице. Только для чтения.|
|sort|[Воркбуктаблесорт](workbooktablesort.md)|Представляет сортировку для таблицы. Только для чтения.|
|worksheet|[Воркбукворкшит](workbookworksheet.md)|Лист, содержащий текущую таблицу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
