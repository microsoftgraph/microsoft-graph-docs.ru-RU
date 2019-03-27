---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу (комнате или оборудованию).
localization_priority: Normal
ms.openlocfilehash: 8a30dcb4394a963e35047fab00391f0cc7eb7715
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926619"
---
# <a name="scheduleitem-resource-type"></a>Тип ресурса Счедулеитем

Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу (комнате или оборудованию).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие. |
|Частный |Boolean |Чувствительность соответствующего события. Значение true, если событие помечено `private`, в противном случае — false. Необязательный.|
|location |String | Расположение, в котором находится соответствующее событие. Необязательный.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в котором начинается соответствующее событие. |
|status |Фрибусистатус | Состояние доступности пользователя или ресурса во время соответствующего события. Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown` |
|subject |String | Строка темы соответствующего события. Необязательный.|


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
