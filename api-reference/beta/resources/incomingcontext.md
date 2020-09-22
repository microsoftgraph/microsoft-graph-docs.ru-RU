---
title: Тип ресурса Инкомингконтекст
description: Контекст, связанный с входящим звонком.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdbaaadc55877aee89f7ea984d60818cbbad0814
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016571"
---
# <a name="incomingcontext-resource-type"></a>Тип ресурса Инкомингконтекст

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контекст, связанный с входящим звонком.

## <a name="properties"></a>Свойства

| Свойство              | Тип                          | Описание                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| обсерведпартиЦипантид | String                        | Идентификатор участника, который находится под наблюдением. Только для чтения.         |
| онбехалфоф            | [identitySet](identityset.md) | Идентификатор, который вызывается от имени пользователя.                   |
| саурцепартиЦипантид   | String                        | Идентификатор участника, который инициировал входящий вызов. Только для чтения.  |
| получатель            | [identitySet](identityset.md) | Удостоверение, которое передал вызов.                                 |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "sourceParticipantId": "String",
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


