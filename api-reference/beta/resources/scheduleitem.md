---
title: Тип ресурса Счедулеитем
description: Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу.
localization_priority: Normal
ms.openlocfilehash: d8b0d7bc18c00ca8bda3ef91b2ec8c629c980a97
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343470"
---
# <a name="scheduleitem-resource-type"></a>Тип ресурса Счедулеитем

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Элемент, описывающий доступность пользователя, соответствующего фактическому событию, в календаре пользователя по умолчанию. Этот элемент также применяется к ресурсу (комнате или оборудованию).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в течение которого заканчивается соответствующее событие. |
|Частный |Логический |Чувствительность соответствующего события. Значение true, если событие помечено `private`, в противном случае — false. Необязательно. |
|location |String | Расположение, в котором находится соответствующее событие. Необязательно.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Дата, время и часовой пояс, в котором начинается соответствующее событие. |
|status |Фрибусистатус | Состояние доступности пользователя или ресурса во время соответствующего события. Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown` |
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
