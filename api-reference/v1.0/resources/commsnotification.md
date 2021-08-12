---
title: тип ресурса commsNotification
description: Базовый тип уведомлений о связи, который публикуется на серверах связи для уведомления об изменениях.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ff7d46a6d081889897940a93d5d111ffa2956a21fc61411060cad08ed2f7d5ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252020"
---
# <a name="commsnotification-resource-type"></a>тип ресурса commsNotification

Пространство имен: microsoft.graph

Базовый тип уведомлений о связи, который публикуется на серверах связи для уведомления об изменениях.

## <a name="properties"></a>Свойства
| Свойство       | Тип    | Описание                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | String  | Возможные значения: `created`, `updated`, `deleted`.      |
| resourceUrl       | String  | URI измененного ресурса.                      |

> **Примечание:** `resourceData` доступны в качестве дополнительных данных. Это объект или коллекция сущностей в зависимости от количества изменений, упакованных в уведомлении.

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

