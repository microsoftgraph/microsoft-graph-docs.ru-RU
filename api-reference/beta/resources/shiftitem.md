---
title: Тип ресурса shiftItem
description: shiftItem представляет версию ресурса shift.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: df012df0ec563a29f15e40d3fefbcd1535dc5211
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008345"
---
# <a name="shiftitem-resource-type"></a>Тип ресурса shiftItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет версию ресурса [shift](shift.md).

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | Примечания для ресурса `shiftItem`.      |
| displayName               | string                  | Имя ресурса `shiftItem`. |
| startDateTime               | DateTimeOffset                  | Дата и время начала для ресурса `shiftItem`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". Обязательный элемент. |
| endDateTime               | DateTimeOffset                 | Дата и время окончания для ресурса `shiftItem`. Обязательный элемент. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| theme | scheduleEntityTheme   |  Поддерживаемые цвета: белый, синий, зеленый, фиолетовый, розовый, желтый, серый, темно-синий, темно-зеленый, темно-фиолетовый, темно-розовый, темно-желтый. |
| activities    | Коллекция [shiftActivity](shiftactivity.md)   | Добавочная часть ресурса shift, содержащая сведения о том, где и когда находится сотрудник во время своей смены. Например, выполняет задание, на плановом перерыве или на обеде. Обязательный элемент. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
