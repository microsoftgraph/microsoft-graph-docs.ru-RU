---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: f2901412dcf1d52d8b117afa214da159b4553a8a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008644"
---
# <a name="scheduleitem-resource-type"></a>Тип ресурса Счедулеитем

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу (комнате или оборудованию).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие. |
|Частный |Boolean |Чувствительность соответствующего события. Значение true, если событие помечено `private`, в противном случае — false. Необязательно. |
|location |String | Расположение, в котором находится соответствующее событие. Необязательно.|
|начать |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в котором начинается соответствующее событие. |
|status |freeBusyStatus | Состояние доступности пользователя или ресурса во время соответствующего события. Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Строка темы соответствующего события. Необязательно.|


## <a name="json-representation"></a>Представление JSON

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
  "tocPath": "",
  "suppressions": []
}
-->
