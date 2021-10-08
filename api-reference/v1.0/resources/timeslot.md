---
title: Тип ресурсов timeSlot
description: Период времени.
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 055797d4dccb4d74f8fe55ce8c0a75c9ab27e417
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240749"
---
# <a name="timeslot-resource-type"></a>Тип ресурсов timeSlot

Пространство имен: microsoft.graph

Представляет интервал времени для собрания.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, который заканчивается. |
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, который начинается.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

