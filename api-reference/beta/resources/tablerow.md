---
title: Тип ресурса TableRow
description: Представляет строку в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2d96ef5c23361cd8b15b47af54a0584e21c48b95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971664"
---
# <a name="tablerow-resource-type"></a>Тип ресурса TableRow

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет строку в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableRow](../api/tablerow-get.md) | [TableRow](tablerow.md) |Чтение свойств и связей объекта tableRow.|
|[обновление](../api/tablerow-update.md). | [TableRow](tablerow.md)  |Обновление объекта tableRow. |
|[Range](../api/tablerow-range.md)|[Range](range.md)|Возвращает объект диапазона, связанный со всей строкой.|
|[Delete](../api/tablerow-delete.md)|Нет|Удаляет строку из таблицы.|
|[List](../api/tablerow-list.md) | Коллекция объектов [TableRow](tablerow.md) |Получение коллекции объектов tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[TableRow](tablerow.md)|Получает строку на основании сведений о ее позиции в коллекции.|
|[Add](../api/tablerowcollection-add.md)|[TableRow](tablerow.md)|Добавляет новую строку в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|index|int|Возвращает номер индекса строки в коллекции строк таблицы. Используется нулевой индекс. Только для чтения.|
|values|json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
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
