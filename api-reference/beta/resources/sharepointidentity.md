---
author: tushar20
title: тип ресурсов sharePointIdentity
ms.localizationpriority: medium
description: Представляет SharePoint субъекта.
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b235f3271c9a39bd99672ad1e0b374f1af5e1b19
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61243043"
---
# <a name="sharepointidentity-resource-type"></a>тип ресурсов sharePointIdentity

Представляет **объект sharePointId** _субъекта_.

Этот ресурс распространяется  на ресурс удостоверений, чтобы предоставить возможность SharePoint определенных сведений; например, **loginName** или SharePoint идентификаторы.

## <a name="properties"></a>Свойства

| Свойство         | Тип                        | Описание |
|:------------     |:----------------------------|:--------------------------------- |
| displayName      | Строка                      | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или в курсе. Например, если пользователь изменит свое отображаемое имя, API может отображать новое значение в последующем ответе, но элементы, сопоставленные с пользователем, будут отображаться без изменения при использовании [разности](../api/driveitem-delta.md). |
| id               | Строка                      | Уникальный идентификатор удостоверения. Это может быть Azure Active Directory или SharePoint. |
| loginName        | Строка                      | Знак во имя SharePoint удостоверения. |
| thumbnails       | Коллекция объектов [thumbnailSet][] | Коллекция, которая [содержит объекты thumbnailSet,][] связанные с элементом. Дополнительные сведения см. [в списке эскизов для driveItem.][] Только для чтения. Допускается значение null. |

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.sharePointIdentity",
  "openType": true,
  "optionalProperties": ["displayName", "thumbnails"]
} -->

```json
{
  "loginName": "string",

  /** inherited from Identity */
  "displayName": "string",
  "id": "string",
  "thumbnails": [{ "@odata.type": "microsoft.graph.thumbnailSet" }]
}
```

[thumbnailSet]: thumbnailset.md
[Эскизы списка для driveItem]: ../api/driveitem-list-thumbnails.md

<!-- {
  "type": "#page.annotation",
  "description": "SharePoint Identity contains information about an app, user, or group.",
  "keywords": "sharePointIdentity, loginName, sharePointId, owner, modifier, app, user, group",
  "section": "documentation",
  "tocPath&quot;: &quot;Resources/SharePointIdentity"
} -->
