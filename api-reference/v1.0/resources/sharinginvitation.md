---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: Ресурс SharingInvitation группировать элементы данных, связанные с приглашениями, в единую структуру.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f90382fa2f65ed2c56afc53ef0a142913eb05579
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240082"
---
# <a name="sharinginvitation-resource-type"></a>Тип ресурса SharingInvitation

Пространство имен: microsoft.graph

Ресурс **SharingInvitation** группировать элементы данных, связанные с приглашениями, в единую структуру.

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
  "tocPath": "Facets/SharingInvitation"
} -->

