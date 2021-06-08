---
title: тип ресурса timeOffItem
description: Представляет версию timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8fbe535fcbc63f94a50e65c62c694ffaac1a9aed
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786084"
---
# <a name="timeoffitem-resource-type"></a>тип ресурса timeOffItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет версию [timeOff](timeoff.md).

## <a name="properties"></a>Свойства
| Свойство                         | Тип                    | Описание                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| timeOffReasonId               | Строка                  | ID этого `timeOffReason` **времениOffItem**. Обязательный.     |
| startDateTime               | DateTimeOffset                  | Дата начала и время **для timeOffItem**. Обязательный элемент. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| endDateTime               | DateTimeOffset                  | Дата окончания и время **для timeOffItem**. Обязательный элемент. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
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
  "theme": {"@odata.type": "microsoft.graph.scheduleEntityTheme"}
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


