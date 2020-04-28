---
title: Тип ресурса Воркбуктаблеров
description: Представляет строку в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ba7b481f4b20033e1a4ffcd42ac92421bc3536a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519122"
---
# <a name="workbooktablerow-resource-type"></a>Тип ресурса Воркбуктаблеров

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет строку в таблице.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта TableRow](../api/tablerow-get.md) | [воркбуктаблеров](workbooktablerow.md) |Чтение свойств и связей объекта tableRow.|
|[Обновление](../api/tablerow-update.md) | [воркбуктаблеров](workbooktablerow.md)  |Обновление объекта tableRow. |
|[Range](../api/tablerow-range.md)|[workbookRange](workbookrange.md)|Получает объект диапазона, связанный со всей строкой.|
|[удаление](../api/tablerow-delete.md);|Нет|Удаляет строку из таблицы.|
|[Список](../api/tablerow-list.md) | Коллекция [воркбуктаблеров](workbooktablerow.md) |Получение коллекции объектов tableRow. |
|[Itemat](../api/tablerowcollection-itemat.md)|[воркбуктаблеров](workbooktablerow.md)|Получает строку на основании ее позиции в коллекции.|
|[Add](../api/tablerowcollection-add.md)|[воркбуктаблеров](workbooktablerow.md)|Добавляет новую строку в таблицу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|index|int|Возвращает номер индекса строки в коллекции строк таблицы. Используется нулевой индекс. Только для чтения.|
|values|Json|Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.|

## <a name="relationships"></a>Связи
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
