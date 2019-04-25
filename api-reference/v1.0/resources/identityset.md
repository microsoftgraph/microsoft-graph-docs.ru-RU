---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
ms.openlocfilehash: 369068dd48b9173032542303e3fd9831d25e6e9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567573"
---
# <a name="identityset-resource-type"></a>Тип ресурса IdentitySet

Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a>Свойства

| Свойство    | Тип                    | Описание                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| application | [Идентификация](identity.md) | Необязательный. Приложение, связанное с данным действием. |
| Устройство      | [Идентификация](identity.md) | Необязательный. Устройство, связанное с данным действием.      |
| user        | [Identity](identity.md) | Необязательный. Пользователь, связанный с данным действием.        |

## <a name="remarks"></a>Заметки 

Сведения об использовании ресурсов **IdentitySet** см. в описании типа [DriveItem](driveitem.md).


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
