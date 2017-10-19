---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 75fa8212f77873b86748f6d8f63c8e62c8d6a0ca
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="sharinginvitation-resource-type"></a>Тип ресурса SharingInvitation

Ресурс **SharingInvitation** — это единая структура, объединяющая элементы данных, связанные с приглашениями.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}
```

## <a name="properties"></a>Свойства

| Имя свойства  | Тип                          | Описание                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| email          | String                        | Электронный адрес получателя приглашения к совместному использованию. Только для чтения.                                          |
| invitedBy      | [identitySet](identityset.md) | Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения. |
| signInRequired | Boolean                       | Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.                     |

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).


<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
