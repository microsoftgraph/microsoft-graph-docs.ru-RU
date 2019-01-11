---
title: Тип ресурса commsNotifications
description: Список уведомлений, используемого серверами коммуникаций для отправки нескольких уведомлений в одном пакете.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9ce629e17c85806d7e05bce99d6a62f9fa9cbff8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851501"
---
# <a name="commsnotifications-resource-type"></a>Тип ресурса commsNotifications

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Список уведомлений, используемого серверами коммуникаций для отправки нескольких уведомлений в одном пакете.

## <a name="properties"></a>Свойства

| Свойство       | Тип                                                 | Описание                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| value          | [commsNotification](commsnotification.md) коллекции | Уведомление об изменении в ресурсе. |

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
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
