---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: Элементы данных, связанные с приглашением, группы ресурсов SharingInvitation в одну структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eaf917ccdd64a50dab9cdf6f2ed477716c18a0185be03812793d115247e17e93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134940"
---
# <a name="sharinginvitation-resource-type"></a>Тип ресурса SharingInvitation

Пространство имен: microsoft.graph

Элементы данных, связанные с приглашением, группы ресурсов **SharingInvitation** в одну структуру.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

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

| Имя свойства  | Тип            | Описание
|:---------------|:----------------|:------------------------------------------
| email          | String          | Электронный адрес получателя приглашения к совместному использованию. Только для чтения.
| invitedBy      | [identitySet][] | Предоставляет сведения об отправителе приглашения, создавшего данное разрешение (если такие сведения доступны). Только для чтения.
| signInRequired | Boolean         | Значение `true` указывает, что получатель приглашения должен выполнить вход для доступа к предоставленному элементу. Только для чтения.

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/SharingInvitation"
} -->

