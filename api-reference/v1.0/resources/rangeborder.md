---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3f906b1e98134b255858015efd765df2194c4a5b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533906"
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
|color|строка|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).|
|id|строка|Представляет идентификатор границы. Возможные `EdgeTop`значения:, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`,. `DiagonalUp` Только для чтения.|
|сидеиндекс|string|Постоянное значение, указывающее определенную сторону границы. Возможные `EdgeTop`значения:, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`,. `DiagonalUp` Только для чтения.|
|style|string|Одна из констант стиля линии, определяющая стиль линии границы. Возможные `None`значения:, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`,. `SlantDashDot`|
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
