---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3fe1c55ca1cac12ac5514c8b703be4d85254044f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143785"
---
# <a name="rangeborder-resource-type"></a>Тип ресурса RangeBorder

Пространство имен: microsoft.graph

Представляет границу объекта.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeBorder](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |Чтение свойств и связей объекта rangeBorder.|
|[Обновление](../api/rangeborder-update.md) | [WorkbookRangeBorder](rangeborder.md) |Обновление объекта RangeBorder. |
|[Список](../api/rangeborder-list.md) | [Коллекция WorkbookRangeBorder](rangeborder.md) |Получение коллекции объектов rangeBorder. |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|Получает объект границы по индексу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|color|string|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).|
|id|string|Представляет идентификатор границы. Возможные значения: `EdgeTop` `EdgeBottom` , , , , , , `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` . Только для чтения.|
|sideIndex|string|Постоянное значение, указывающее определенную сторону границы. Возможные значения: `EdgeTop` `EdgeBottom` , , , , , , `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` . Только для чтения.|
|style|string|Одна из констант стиля линии, определяющая стиль линии границы. Возможные значения: `None` `Continuous` , , , , , , `Dash` `DashDot` `DashDotDot` `Dot` `Double` `SlantDashDot` .|
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

