---
title: тип ресурса incomingContext
description: Представляет контекст, связанный с входящий вызов.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8f7409048acb19e36446b257ed32acceff76d5783f3cf4050620de3da5e11314
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231791"
---
# <a name="incomingcontext-resource-type"></a>тип ресурса incomingContext

Пространство имен: microsoft.graph

Представляет контекст, связанный с входящий вызов.

## <a name="properties"></a>Свойства

| Свойство              | Тип                          | Описание                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| sourceParticipantId   | String                        | ID участника, который вызвал входящий вызов. Только для чтения.  |
| observedParticipantId | String                        | ID участника, который находится под наблюдением. Только для чтения.         |
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

