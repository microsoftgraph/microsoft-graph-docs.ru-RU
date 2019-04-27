---
title: Тип ресурса Воркбуктаблеров
description: Представляет строку в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 2c43fab3024d04a9e58f5de23e849c7b98fafeed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33349018"
---
# <a name="workbooktablerow-resource-type"></a>Тип ресурса Воркбуктаблеров

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableRow](../api/tablerow-get.md) | [Воркбуктаблеров](workbooktablerow.md) |Чтение свойств и связей объекта tableRow.|
|[Обновление](../api/tablerow-update.md) | [Воркбуктаблеров](workbooktablerow.md)  |Обновление объекта tableRow. |
|[Range](../api/tablerow-range.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со всей строкой.|
|[Delete](../api/tablerow-delete.md)|Нет|Удаляет строку из таблицы.|
|[Список](../api/tablerow-list.md) | Коллекция [воркбуктаблеров](workbooktablerow.md) |Получение коллекции объектов tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[Воркбуктаблеров](workbooktablerow.md)|Получает строку на основании ее позиции в коллекции.|
|[Add](../api/tablerowcollection-add.md)|[Воркбуктаблеров](workbooktablerow.md)|Добавляет новую строку в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|index|int|Возвращает номер индекса строки в коллекции строк таблицы. Используется нулевой индекс. Только для чтения.|
|values|Json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookTableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
