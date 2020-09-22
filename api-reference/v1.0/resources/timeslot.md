---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 874b587db2bb9e2234fcacca9b3e3b0cf5c2f89b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090755"
---
# <a name="timeslot-resource-type"></a>Тип ресурсов timeSlot

Пространство имен: microsoft.graph

Представляет интервал времени для собрания.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, с которого начинается период. |
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, в течение которого заканчивается срок.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

