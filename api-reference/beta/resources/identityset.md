---
author: JeremyKelley
description: Ресурс identitySet — это набор ключей для ресурсов удостоверений.
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
ms.openlocfilehash: 50f6b45c3121f770019d9b5be7e0492242711e1c
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453718"
---
# <a name="identityset-resource-type"></a>Тип ресурса identitySet

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **identitySet** — это набор ключей для ресурсов [удостоверений.](identity.md)

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
| conversation| [Identity](identity.md) | Необязательный. Команда или канал, связанный с этим действием.       |
| conversationIdentityType| [Identity](identity.md) | Необязательный. Указывает, определяет ли свойство **беседы** команду или канал.|
| Устройство      | [Identity](identity.md) | Необязательный. Устройство, связанное с данным действием.       |
| phone       | [identity](identity.md) | Необязательно. Номер телефона, связанный с этим действием. |
| user        | [Identity](identity.md) | Необязательный. Пользователь, связанный с данным действием.         |

## <a name="remarks"></a>Заметки 

См. в этой ленте [Call](call.md) for use of **identitySet** resources.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->


