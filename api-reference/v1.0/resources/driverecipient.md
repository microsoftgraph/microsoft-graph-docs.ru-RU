---
author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
ms.localizationpriority: medium
ms.prod: sharepoint
description: Ресурс driveRecipient представляет человека, группу или другого получателя, который должен делиться с помощью действия приглашения.
doc_type: resourcePageType
ms.openlocfilehash: 4788b02e0ec52965475745a4e234beaaf6b2910e
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115391"
---
# <a name="driverecipient-resource"></a>ресурс driveRecipient

Пространство имен: microsoft.graph

Представляет человека, группу или другого получателя для обмена элементом диска с помощью действия [приглашения.](../api/driveitem-invite.md)

При использовании  [приглашения](../api/driveitem-invite.md) для добавления разрешений объект **driveRecipient** указывает электронную почту, псевдоним или  **objectId** получателя.
Требуется только одно из этих значений; несколько значений не принимаются.

## <a name="properties"></a>Свойства
Ниже перечислены свойства ресурса получателя.

| Имя свойства | Тип   | Описание                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | String | Электронный адрес получателя (если с получателем связан электронный адрес).                  |
| alias         | String | Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности). |
| objectId      | String | Уникальный идентификатор получателя в каталоге.                                               |

## <a name="json-representation"></a>Представление JSON

<!-- { 
  "blockType": "resource", 
  "@odata.type": "microsoft.graph.driveRecipient", 
  "optionalProperties": ["alias", "objectId", "email"] } -->
```json
{
  "email": "string",
  "alias": "string",
  "objectId": "string",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->

