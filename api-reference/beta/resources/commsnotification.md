---
title: Тип ресурса Коммснотификатион
description: Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4ec3df8bc56e6164af3b7752333d28bd10665d67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507606"
---
# <a name="commsnotification-resource-type"></a>Тип ресурса Коммснотификатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.

## <a name="properties"></a>Свойства
| Свойство       | Тип    | Описание                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| changeType     | String  | Возможные значения: `created`, `updated`, `deleted`.      |
| Resourceurl экземпляром       | String  | URI ресурса, который был изменен.                      |

> **Примечание:** `resourceData` доступно в виде дополнительных данных. Это либо сущность, либо коллекция сущностей в зависимости от количества изменений, упакованных в уведомление.

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
