---
title: Тип ресурса scheduleItem
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: e5d14826a27153af27648484554ec864d62ed6c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890435"
---
# <a name="scheduleitem-resource-type"></a>Тип ресурса scheduleItem

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Элемент, сведения о доступности пользователя, соответствующего Фактическое событие в календаре пользователя по умолчанию. Этот элемент применяется к ресурсам, а также.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Даты, времени и часового пояса, название которого заканчивается соответствующего события. |
|isPrivate |Логический |Уровень конфиденциальности сообщения соответствующего события. Значение true, если событие помечено `private`, и false в противном случае. |
|location |String | Расположение, где удерживается или посетившие из соответствующих событий. Необязательное.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Даты, времени и часового пояса, который запускает соответствующего события. |
|status |Строка | Состояние доступности пользователя или ресурсов во время соответствующего события. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |Строка | Строка темы соответствующего события. Необязательное.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
