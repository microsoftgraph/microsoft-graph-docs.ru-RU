---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c32264311400951152f892e6f88d70645f47064
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947612"
---
# <a name="rangeborder-resource-type"></a>Тип ресурса RangeBorder

Представляет границу объекта.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeBorder](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |Чтение свойств и связей объекта rangeBorder.|
|[обновление](../api/rangeborder-update.md). | [WorkbookRangeBorder](rangeborder.md) |Обновление объекта RangeBorder. |
|[List](../api/rangeborder-list.md) | [WorkbookRangeBorder](rangeborder.md) коллекции |Получение коллекции объектов rangeBorder. |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|Возвращает объект границы по его индексу.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|color|строка|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).|
|id|строка|Представляет граница идентификатор. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.|
|sideIndex|строка|Постоянное значение, указывающее, конкретной стороны границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.|
|style|строка|Одна из констант линии, определяющее тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.|
|weight|строка|Задает Вес границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.|

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
