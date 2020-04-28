---
title: Тип ресурса Каллрауте
description: Тип Каллрауте.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9a2ac5e0e8656cf6d7dcde2528d7ca000368d640
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507798"
---
# <a name="callroute-resource-type"></a>Тип ресурса Каллрауте

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип Каллрауте.

## <a name="properties"></a>Свойства

| Свойство            | Тип                          | Описание                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| Наконец               | [identitySet](identityset.md) | Идентификатор, разрешенный в вызове.               |
| Исходный текст            | [identitySet](identityset.md) | Идентификатор, который изначально использовался при вызове.           |
| раутингтипе         | String                        | Возможные значения: `forwarded`, `lookup`, `selfFork`.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
