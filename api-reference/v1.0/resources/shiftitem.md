---
title: Тип ресурса shiftItem
description: shiftItem представляет версию ресурса shift.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d66206d127c5de8bd23b6d1f363359d9eff03ee
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032176"
---
# <a name="shiftitem-resource-type"></a>Тип ресурса shiftItem

Пространство имен: microsoft.graph

Представляет версию ресурса [shift](shift.md).

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | Заметки о переносе `shiftItem` для .      |
| displayName               | string                  | Метка переноса `shiftItem` . |
| startDateTime               | DateTimeOffset                  | Дата и время начала для ресурса `shiftItem`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Обязательный. |
| endDateTime               | DateTimeOffset                 | Дата и время окончания для ресурса `shiftItem`. Обязательный элемент. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
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

