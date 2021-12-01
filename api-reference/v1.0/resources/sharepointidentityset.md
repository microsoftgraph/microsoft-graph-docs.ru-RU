---
author: tushar20
title: тип ресурсов sharePointIdentitySet
ms.localizationpriority: medium
description: Представляет собой набор ключей для sharePointIdentity и ресурсов удостоверений.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f8bf2e51c1b4af1935b5885ac91b767e444691e5
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242677"
---
# <a name="sharepointidentityset-resource-type"></a>тип ресурсов sharePointIdentitySet

Представляет коллекцию ресурсов [sharePointIdentity](sharePointIdentity.md) с ключами. Этот ресурс распространяется на ресурс **identitySet,** чтобы предоставить пользователю SharePoint определенных сведений.

Этот ресурс используется для представления набора удостоверений, связанных с  различными событиями для элемента, например созданных или измененных последним _путем_.

Сведения об использовании см. [в driveItem.][]

## <a name="properties"></a>Свойства

| Свойство    | Тип                   | Описание |
|:------------|:-----------------------|:----------------------------------------------------------- |
| application | [identity][]           | Приложение, связанное с данным действием. Необязательный параметр. |
| device;      | [identity][]           | Устройство, связанное с данным действием. Необязательный параметр. |
| group;       | [identity][]           | Группа, связанная с этим действием. Необязательный параметр. |
| пользователь        | [identity][]           | Пользователь, связанный с данным действием. Необязательный параметр. |
| siteUser    | [sharePointIdentity][] | Пользователь SharePoint, связанный с этим действием. Необязательный параметр. |
| siteGroup   | [sharePointIdentity][] | Группа SharePoint, связанная с этим действием. Необязательный параметр. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.sharePointIdentitySet",
       "optionalProperties": ["user", "application", "group", "device", "siteUser", "siteGroup"],
       "openType": true } -->

```json
{
  /** inherited from IdentitySet **/
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"},
  
  "group": {"@odata.type": "microsoft.graph.identity"},
  "siteUser": {"@odata.type": "microsoft.graph.sharePointIdentity"},
  "siteGroup":{"@odata.type": "microsoft.graph.sharePointIdentity"}
}
```

[driveItem]: driveItem.md
[identity]: identity.md
[sharePointIdentity]: sharePointIdentity.md

<!-- {
  "type": "#page.annotation",
  "description": "SharePointIdentity set is a collection of identities/sharePointIdentities",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/SharePointIdentitySet"
} -->
