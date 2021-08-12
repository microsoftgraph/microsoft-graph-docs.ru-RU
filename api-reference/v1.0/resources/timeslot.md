---
title: Тип ресурсов timeSlot
description: Период времени.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 08ba0c696c511e5a80c25262ba9d1d4cab6d2231aabea01cec0f573d70cd6ec1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189200"
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
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, который начинается. |
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, который заканчивается.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

