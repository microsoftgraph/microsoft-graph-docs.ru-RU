---
title: Тип ресурса commsNotification
description: Связь уведомлений базовый тип, который был опубликован серверами коммуникаций для уведомление об изменениях.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e5b929997cf17d13043264d42421418321aae84e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977698"
---
# <a name="commsnotification-resource-type"></a>Тип ресурса commsNotification

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Связь уведомлений базовый тип, который был опубликован серверами коммуникаций для уведомление об изменениях.

## <a name="properties"></a>Свойства
| Свойство       | Тип    | Описание                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | Строка  | Возможные значения: `created`, `updated`, `deleted`.      |
| resource       | Строка  | URI-идентификатор ресурса, который был изменен.                      |

> **Примечание:** `resourceData` доступен в качестве дополнительных данных. Это объект или Collection(entity) в зависимости от изменений, упакованный в уведомления.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "changeType": "created | updated | deleted",
  "resource": "String"
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E",
        "state": "incoming"
      }
    }
  ]
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
