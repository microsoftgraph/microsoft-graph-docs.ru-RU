---
title: Тип ресурса Воркбуктаблеколумн
description: Представляет столбец в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 07dbcd2e900ced3fe235300cfab2b4922ddccc9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007076"
---
# <a name="workbooktablecolumn-resource-type"></a>Тип ресурса Воркбуктаблеколумн

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет столбец в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableColumn](../api/tablecolumn-get.md) | [Воркбуктаблеколумн](workbooktablecolumn.md) |Чтение свойств и связей объекта tableColumn.|
|[Обновление](../api/tablecolumn-update.md) | [Воркбуктаблеколумн](workbooktablecolumn.md) |Обновление объекта TableColumn. |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный с основными данными столбца.|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со строкой заголовков столбца.|
|[Range](../api/tablecolumn-range.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со всем столбцом.|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со строкой итогов столбца.|
|[Удаление](../api/tablecolumn-delete.md)|Нет|Удаляет столбец из таблицы.|
|[Список](../api/tablecolumn-list.md) | Коллекция [воркбуктаблеколумн](workbooktablecolumn.md) |Получение коллекции объектов tableColumn. |
|[Itemat](../api/tablecolumncollection-itemat.md)|[Воркбуктаблеколумн](workbooktablecolumn.md)|Возвращает столбец на основании его позиции в коллекции.|
|[Add](../api/tablecolumncollection-add.md)|[Воркбуктаблеколумн](workbooktablecolumn.md)|Добавляет новый столбец в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|int|Возвращает уникальный ключ, идентифицирующий столбец в таблице. Только для чтения.|
|index|int|Возвращает номер индекса столбца в коллекции столбцов таблицы. Используется нулевой индекс. Только для чтения.|
|name|string|Возвращает имя столбца таблицы. Только для чтения.|
|values|Json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|filter|[Воркбукфилтер](workbookfilter.md)|Возвращает фильтр, применяемый к столбцу. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
