---
title: Тип ресурса Icon
description: Представляет значок ячейки.
localization_priority: Normal
ms.openlocfilehash: 833fa4cb4061a96b01077c3adeb7dcaed49e0a02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567811"
---
# <a name="icon-resource-type"></a>Тип ресурса Icon

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
|set|string|Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags` `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns` `FourTrafficLights` `FiveArrows` `FiveArrowsGray` `FiveRating` `FiveQuarters` `ThreeStars` `FourRedToBlack` `FourRating`,,,,,,,,,,,,,,,,,,,,,, `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` , `ThreeTriangles`, `FiveBoxes`.|

## <a name="relationships"></a>Отношения
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
