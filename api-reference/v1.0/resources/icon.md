---
title: Тип ресурса Icon
description: Представляет значок ячейки.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 84953f4917b3cbf4b5792ed3a7b74600ec2457c6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054905"
---
# <a name="icon-resource-type"></a>Тип ресурса Icon

Пространство имен: microsoft.graph

Представляет значок ячейки.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта Icon](../api/icon-get.md) | [Icon](icon.md) |Чтение свойств и связей объекта значка.|
|[Обновление](../api/icon-update.md) | [Icon](icon.md)  |Обновление объекта значка. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|index|int|Представляет собой индекс значка данного набора.|
|set|string|Представляет набор, в который входит значок. Возможные значения:,,,,,,,,,,,,,,,,,,, `Invalid` `ThreeArrows` `ThreeArrowsGray` `ThreeFlags` `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns` `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack` `FourRating` , `FourTrafficLights` , `FiveArrows` , `FiveArrowsGray` `FiveRating` `FiveQuarters` `ThreeStars` `ThreeTriangles` `FiveBoxes` ,,,,,.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

