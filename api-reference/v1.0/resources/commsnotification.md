---
title: тип ресурса commsNotification
description: Базовый тип уведомлений о связи, который публикуется на серверах связи для уведомления об изменениях.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 790704c73e07c473112eb5df99db7261d73966f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062777"
---
# <a name="commsnotification-resource-type"></a>тип ресурса commsNotification

Пространство имен: microsoft.graph

Базовый тип уведомлений о связи, который публикуется на серверах связи для уведомления об изменениях.

## <a name="properties"></a>Свойства
| Свойство       | Тип    | Описание                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | Строка  | Возможные значения: `created`, `updated`, `deleted`.      |
| resourceUrl       | Строка  | URI измененного ресурса.                      |

> **Примечание:** `resourceData` доступны в качестве дополнительных данных. Это объект или коллекция сущностей в зависимости от количества изменений, упакованных в уведомлении.

## <a name="json-representation"></a>Представление в формате JSON

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
  "@odata.type": "#microsoft.graph.commsNotification",
  "changeType": "created | updated | deleted",
  "resourceUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

