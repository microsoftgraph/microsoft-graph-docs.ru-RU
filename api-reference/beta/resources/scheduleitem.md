---
title: Тип ресурса scheduleItem
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ed6b7441996cdf00b33be03f70afb888cc9bb251
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511354"
---
# <a name="scheduleitem-resource-type"></a>Тип ресурса scheduleItem

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Элемент, сведения о доступности пользователя, соответствующего Фактическое событие в календаре пользователя по умолчанию. Этот элемент применяется к ресурсам, а также.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Даты, времени и часового пояса, название которого заканчивается соответствующего события. |
|IsPrivate |Логическое |Уровень конфиденциальности сообщения соответствующего события. Значение true, если событие помечено `private`, и false в противном случае. |
|location |String | Расположение, где удерживается или посетившие из соответствующих событий. Необязательный параметр.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Даты, времени и часового пояса, который запускает соответствующего события. |
|status |String | Состояние доступности пользователя или ресурсов во время соответствующего события. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Строка темы соответствующего события. Необязательный параметр.|


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
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
