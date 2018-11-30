---
title: Тип ресурса meetingCapability
description: Содержит возможности собрания
ms.openlocfilehash: 438193d08ab5542f07d4cbf61704520d81433e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078084"
---
# <a name="meetingcapability-resource-type"></a>Тип ресурса meetingCapability

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит возможности собрания

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Description|
|:---------------|:--------|:----------|
| allowAnonymousUsersToDialOut | Логический | Указывает, может ли анонимные пользователи исходящие звонки на собрании. |
| autoAdmittedUsers | String | Возможные значения: `everyoneInCompany`, `everyone`. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
