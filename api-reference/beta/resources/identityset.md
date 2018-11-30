---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
ms.openlocfilehash: 71620da04ea9d7f67d69422ce175182d406d44f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077911"
---
# <a name="identityset-resource-type"></a>Тип ресурса identitySet

Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
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
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a>Свойства

| Свойство    | Тип                    | Описание                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| application | [Identity](identity.md) | Необязательный. Приложение, связанное с данным действием.  |
| Устройство
      | [Identity](identity.md) | Необязательный. Устройство, связанное с данным действием.       |
| phone       | [identity](identity.md) | Необязательный атрибут. Номер телефона, связанного с этого действия. |
| user        | [Identity](identity.md) | Необязательный. Пользователь, связанный с данным действием.         |

## <a name="remarks"></a>Примечания 

В разделе [вызова](call.md) использования ресурсов **IdentitySet** .


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->