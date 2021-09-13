---
author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
ms.localizationpriority: medium
description: Ресурс IdentitySet представляет собой коллекцию ресурсов identity с ключами.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a37afd466cf99851ef6343f69c8d97188476ae72
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032372"
---
# <a name="identityset-resource-type"></a>Тип ресурса IdentitySet

Пространство имен: microsoft.graph

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
| application | [Identity](identity.md) | Необязательный. Приложение, связанное с данным действием. |
| Устройство      | [Identity](identity.md) | Необязательный. Устройство, связанное с данным действием.      |
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

