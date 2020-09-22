---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a4536607c4723a9e16d77e045e17bd151da50d36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090930"
---
# <a name="rangeborder-resource-type"></a>Тип ресурса RangeBorder

Пространство имен: microsoft.graph

Представляет границу объекта.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeBorder](../api/rangeborder-get.md) | [воркбукранжебордер](rangeborder.md) |Чтение свойств и связей объекта rangeBorder.|
|[Обновление](../api/rangeborder-update.md) | [воркбукранжебордер](rangeborder.md) |Обновление объекта RangeBorder. |
|[Список](../api/rangeborder-list.md) | Коллекция [воркбукранжебордер](rangeborder.md) |Получение коллекции объектов rangeBorder. |
|[Itemat](../api/rangebordercollection-itemat.md)|[воркбукранжебордер](rangeborder.md)|Получает объект границы по индексу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|color|string|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).|
|id|string|Представляет идентификатор границы. Возможные значения:,, `EdgeTop` `EdgeBottom` ,, `EdgeLeft` `EdgeRight` `InsideVertical` , `InsideHorizontal` , `DiagonalDown` , `DiagonalUp` . Только для чтения.|
|сидеиндекс|string|Постоянное значение, указывающее определенную сторону границы. Возможные значения:,, `EdgeTop` `EdgeBottom` ,, `EdgeLeft` `EdgeRight` `InsideVertical` , `InsideHorizontal` , `DiagonalDown` , `DiagonalUp` . Только для чтения.|
|style|string|Одна из констант стиля линии, определяющая стиль линии границы. Возможные значения:,, `None` `Continuous` ,, `Dash` `DashDot` `DashDotDot` , `Dot` , `Double` , `SlantDashDot` .|
|weight|string|Определяет толщину границы вокруг диапазона. Допустимые значения: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

