---
title: Тип ресурса Коммснотификатион
description: Базовый тип уведомления о связи, который публикуется серверами Communications Server для уведомления об изменениях.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c87c12aee367a6520485a222702f827ae833aa98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033967"
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

> **Примечание:** `resourceData` доступна в виде дополнительных данных. Это либо сущность, либо коллекция сущностей в зависимости от количества изменений, упакованных в уведомление.

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


