---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: harini84
ms.openlocfilehash: b4bbf2586543b4f731c136eaffbc955741191db6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812799"
---
# <a name="scheduleitem-resource-type"></a>Тип ресурса Счедулеитем

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу (комнате или оборудованию).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие. |
|Частный |Логический |Чувствительность соответствующего события. Значение true, если событие помечено `private` , в противном случае — false. Необязательное свойство. |
|location |String | Расположение, в котором находится соответствующее событие. Необязательное свойство.|
|начать |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в котором начинается соответствующее событие. |
|status |freeBusyStatus | Состояние доступности пользователя или ресурса во время соответствующего события. Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Строка темы соответствующего события. Необязательное свойство.|


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
  "tocPath": "",
  "suppressions": []
}
-->
