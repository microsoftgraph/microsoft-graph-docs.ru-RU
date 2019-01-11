---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 33ed0410ab807cf9d9d6a0a49cb06b43d9966e46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853531"
---
# <a name="rangeborder-resource-type"></a>Тип ресурса RangeBorder

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет границу объекта.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeBorder](../api/rangeborder-get.md) | [RangeBorder](rangeborder.md) |Чтение свойств и связей объекта rangeBorder.|
|[обновление](../api/rangeborder-update.md). | [RangeBorder](rangeborder.md) |Обновление объекта RangeBorder. |
|[List](../api/rangeborder-list.md) | Коллекция объектов [RangeBorder](rangeborder.md) |Получение коллекции объектов rangeBorder. |
|[Itemat](../api/rangebordercollection-itemat.md)|[RangeBorder](rangeborder.md)|Возвращает объект границы по его индексу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|color|строка|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).|
|id|строка|Представляет идентификатор границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.|
|sideIndex|string|Постоянное значение, указывающее определенную сторону границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.|
|style|строка|Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.|
|weight|string|Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
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
