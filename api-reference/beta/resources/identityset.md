---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
ms.openlocfilehash: 10b39bd5747e10ea4340bb5b4c54df0f94eb4229
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547146"
---
# <a name="identityset-resource-type"></a>Тип ресурса Identity

Ресурс **Identity** является коллекцией с ключом для ресурсов [Identity](identity.md) .
Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.

## <a name="json-representation"></a>Представление в формате JSON

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
| application | [Идентификация](identity.md) | Необязательный. Приложение, связанное с данным действием.  |
| conversation| [Identity](identity.md) | Необязательный. Группа или канал, связанные с этим действием.       |
| Конверсатионидентититипе| [Identity](identity.md) | Необязательный. Указывает, идентифицирует **** ли свойство беседы группу или канал.|
| Устройство      | [Идентификация](identity.md) | Необязательный. Устройство, связанное с данным действием.       |
| phone       | [identity](identity.md) | Необязательно. Номер телефона, связанный с этим действием. |
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
