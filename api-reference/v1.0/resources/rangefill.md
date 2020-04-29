---
title: Тип ресурса RangeFill
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 37bc96fdd0dad65a1f6b5b6bcec244ef96b915ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447026"
---
# <a name="rangefill-resource-type"></a>Тип ресурса RangeFill

Пространство имен: microsoft.graph

Представляет фон объекта диапазона.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта RangeFill](../api/rangefill-get.md) | [воркбукранжефилл](rangefill.md) |Чтение свойств и связей объекта rangeFill.|
|[Обновление](../api/rangefill-update.md) | [воркбукранжефилл](rangefill.md)   |Обновление объекта RangeFill. |
|[Clear](../api/rangefill-clear.md)|Нет|Сбрасывает фон диапазона.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|color|string|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
