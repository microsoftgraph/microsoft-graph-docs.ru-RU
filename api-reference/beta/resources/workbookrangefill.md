---
title: Тип ресурса Воркбукранжефилл
description: Представляет фон объекта диапазона.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eea7337fa4aefb1bde607740b9a2fc78264dae91
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348977"
---
# <a name="workbookrangefill-resource-type"></a>Тип ресурса Воркбукранжефилл

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет фон объекта диапазона.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Воркбукранжефилл](../api/rangefill-get.md) | [Воркбукранжефилл](workbookrangefill.md) |Чтение свойств и связей объекта rangeFill.|
|[Обновление](../api/rangefill-update.md) | [Воркбукранжефилл](workbookrangefill.md)   |Обновление объекта RangeFill. |
|[Clear](../api/rangefill-clear.md)|Нет|Сбрасывает фон диапазона.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|color|string|HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова в HTML (например, orange).|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
