---
title: тип ресурса incomingContext
description: Представляет контекст, связанный с входящий вызов.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 80f300fc4f3cf051466b37c4445272444fdc71bc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123358"
---
# <a name="incomingcontext-resource-type"></a>тип ресурса incomingContext

Пространство имен: microsoft.graph

Представляет контекст, связанный с входящий вызов.

## <a name="properties"></a>Свойства

| Свойство              | Тип                          | Описание                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| sourceParticipantId   | Строка                        | ID участника, который вызвал входящий вызов. Только для чтения.  |
| observedParticipantId | Строка                        | ID участника, который находится под наблюдением. Только для чтения.         |
| onBehalfOf            | [identitySet](identityset.md) | Удостоверение, которое происходит от имени вызова.                   |
| переносчик            | [identitySet](identityset.md) | Удостоверение, которое передало вызов.                                 |

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

