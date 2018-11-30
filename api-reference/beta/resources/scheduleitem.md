---
title: Тип ресурса scheduleItem
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: a7a31f47cde92549a72299b22a40b10c6f7845c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080206"
---
# <a name="scheduleitem-resource-type"></a>Тип ресурса scheduleItem

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Элемент, сведения о доступности пользователя, соответствующего Фактическое событие в календаре пользователя по умолчанию. Этот элемент применяется к ресурсам, а также.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Даты, времени и часового пояса, название которого заканчивается соответствующего события. |
|isPrivate |Логический |Уровень конфиденциальности сообщения соответствующего события. Значение true, если событие помечено `private`, и false в противном случае. |
|location |String | Расположение, где удерживается или посетившие из соответствующих событий. Необязательный атрибут.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Даты, времени и часового пояса, который запускает соответствующего события. |
|status |String | Состояние доступности пользователя или ресурсов во время соответствующего события. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Строка темы соответствующего события. Необязательный атрибут.|


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