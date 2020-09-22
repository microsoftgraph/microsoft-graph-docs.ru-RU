---
title: Тип ресурса Каллрауте
description: Представляет тип маршрута вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9ff55759e71cda0876a2ce5b0a65e47bcaf917a0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069269"
---
# <a name="callroute-resource-type"></a>Тип ресурса Каллрауте

Пространство имен: microsoft.graph

Представляет тип маршрута вызова.

## <a name="properties"></a>Свойства

| Свойство            | Тип                          | Описание                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| Наконец               | [identitySet](identityset.md) | Идентификатор, разрешенный в вызове.               |
| Исходный текст            | [identitySet](identityset.md) | Идентификатор, который изначально использовался при вызове.           |
| раутингтипе         | Строка                        | Возможные значения: `forwarded`, `lookup`, `selfFork`.  |

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

