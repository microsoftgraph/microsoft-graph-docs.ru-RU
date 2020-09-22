---
title: Тип ресурса Тимеоффитем
description: Представляет версию объекта Тимеофф.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 47af5866c4e8645b8b03aa0403b7cf0bc75e0715
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090811"
---
# <a name="timeoffitem-resource-type"></a>Тип ресурса Тимеоффитем

Пространство имен: microsoft.graph

Представляет версию объекта [тимеофф](timeoff.md).

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| тимеоффреасонид               | string                  | Идентификатор объекта `timeOffReason` для этого параметра `timeOffItem` . Обязательный.     |
| startDateTime               | DateTimeOffset                  | Дата и время начала для ресурса `timeOffItem`. Обязательный элемент. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| endDateTime               | DateTimeOffset                  | Дата и время окончания для ресурса `timeOffItem`. Обязательный элемент. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: "2014-01-01T00:00:00Z". |
| theme | scheduleEntityTheme   | Поддерживаемые цвета: белый, синий, зеленый, фиолетовый, розовый, желтый, серый, темно-синий, темно-зеленый, темно-фиолетовый, темно-розовый, темно-желтый. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

