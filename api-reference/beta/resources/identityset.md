---
author: JeremyKelley
description: Ресурс Identity является коллекцией с ключом для ресурсов Identity.
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 60fdb901ecd74f3826604d139cad71d9d0844221
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966766"
---
# <a name="identityset-resource-type"></a>Тип ресурса Identity

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Identity** является коллекцией с ключом для ресурсов [Identity](identity.md) .

Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Свойства

| Свойство    | Тип                    | Описание                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| application | [Identity](identity.md) | Необязательный. Приложение, связанное с данным действием.  |
| conversation| [Identity](identity.md) | Необязательный. Группа или канал, связанные с этим действием.       |
| конверсатионидентититипе| [Identity](identity.md) | Необязательный. Указывает, идентифицирует ли свойство **беседы** группу или канал.|
| Устройство      | [Identity](identity.md) | Необязательный. Устройство, связанное с данным действием.       |
| phone       | [identity](identity.md) | Необязательный параметр. Номер телефона, связанный с этим действием. |
| user        | [Identity](identity.md) | Необязательный. Пользователь, связанный с данным действием.         |

## <a name="remarks"></a>Заметки 

Ознакомьтесь со статьей [вызов](call.md) для использования ресурсов **удостоверений** .


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->


