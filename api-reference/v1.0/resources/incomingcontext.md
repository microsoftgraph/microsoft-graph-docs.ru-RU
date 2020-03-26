---
title: Тип ресурса Инкомингконтекст
description: Представляет контекст, связанный с входящим вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6acd1928b223789df7580a5f74eefc723570ca93
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962569"
---
# <a name="incomingcontext-resource-type"></a>Тип ресурса Инкомингконтекст

Пространство имен: microsoft.graph

Представляет контекст, связанный с входящим вызовом.

## <a name="properties"></a>Свойства

| Свойство              | Тип                          | Описание                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| саурцепартиЦипантид   | String                        | Идентификатор участника, который инициировал входящий вызов. Только для чтения.  |
| обсерведпартиЦипантид | String                        | Идентификатор участника, который находится под наблюдением. Только для чтения.         |
| онбехалфоф            | [identitySet](identityset.md) | Идентификатор, который вызывается от имени пользователя.                   |
| получатель            | [identitySet](identityset.md) | Удостоверение, которое передал вызов.                                 |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sourceParticipantId",
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "transferor": {"@odata.type": "#microsoft.graph.identitySet"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "incomingContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
