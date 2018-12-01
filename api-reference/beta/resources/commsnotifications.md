---
title: Тип ресурса уведомлений
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 96246491c386971fe18184f26269d4abe3af6e6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082500"
---
# <a name="notifications-resource-type"></a>Тип ресурса уведомлений

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

## <a name="properties"></a>Свойства

| Свойство       | Тип                                       | Описание |
|:---------------|:-------------------------------------------|:------------|
| value          | [уведомления](commsnotification.md) семейства сайтов | Уведомление об изменении в ресурсе. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->