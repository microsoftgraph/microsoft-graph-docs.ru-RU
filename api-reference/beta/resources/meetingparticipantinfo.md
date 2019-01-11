---
title: Тип ресурса meetingParticipantInfo
description: Сведения о участник в собрании.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: d7b5ae17bd3bfb566bce0da9814b86aab98173da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834260"
---
# <a name="meetingparticipantinfo-resource-type"></a>Тип ресурса meetingParticipantInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сведения о участник в собрании.

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание                              |
|:---------------|:------------------------------|:-----------------------------------------|
| identity       | [identitySet](identityset.md) | Сведения об удостоверениях участника. |
| Имя участника-пользователя            | Строка                        | Имя участника-пользователя участника.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
