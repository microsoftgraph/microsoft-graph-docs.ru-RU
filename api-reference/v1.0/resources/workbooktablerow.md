---
title: тип ресурса workbookTableRow
description: Представляет строку в таблице.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4b546e3593668c167479d18bcc06e1d61f59fbb4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777227"
---
# <a name="workbooktablerow-resource-type"></a>тип ресурса workbookTableRow

Пространство имен: microsoft.graph

Представляет строку в таблице.


## <a name="methods"></a>Методы

### <a name="manage-workbooktablerow"></a>Управление книгойTableRow
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get workbookTableRow](../api/tablerow-get.md) | [workbookTableRow]( workbooktablerow.md) |Чтение свойств и связей объекта tableRow.|
|[Обновление](../api/tablerow-update.md) | [workbookTableRow]( workbooktablerow.md) |Обновление объекта workbookTableRow. |
|[удаление](../api/tablerow-delete.md);|Нет|Удаляет строку из таблицы.|
|[Создание книгиTableRow](../api/table-post-rows.md)|[workbookTableRow]( workbooktablerow.md)|Добавляет строки в таблицу.|
|[Range](../api/tablerow-range.md)|[Range](range.md)|Получает объект диапазона, связанный со всей строкой.|
|[Перечисление](../api/tablerow-list.md) | [коллекция workbookTableRow]( workbooktablerow.md) |Получение коллекции объектов tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[workbookTableRow]( workbooktablerow.md)|Получает строку на основании ее позиции в коллекции.|
|[Add](../api/tablerowcollection-add.md)|[workbookTableRow]( workbooktablerow.md)|Добавляет новую строку в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|index|Int32|Возвращает номер индекса строки в коллекции строк таблицы. Используется нулевой индекс. Только для чтения.|
|values|[Json](../resources/json.md)|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workbookTableRow",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "index": "Integer",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookTableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

