---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
description: Ресурс DriveRecipient представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия invite.
doc_type: resourcePageType
ms.openlocfilehash: d509a1819b0ad10f695d97153a8f837793b9dbe4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032727"
---
# <a name="driverecipient-resource"></a>Ресурс DriveRecipient

Пространство имен: microsoft.graph

Ресурс **DriveRecipient** представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия [invite](../api/driveitem-invite.md).

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

## <a name="properties"></a>Свойства
Ниже перечислены свойства ресурса получателя.

| Имя свойства | Тип   | Описание                                                                                             |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------|
| email         | String | Электронный адрес получателя (если с получателем связан электронный адрес).                  |
| alias         | String | Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности). |
| objectId      | String | Уникальный идентификатор получателя в каталоге.                                               |

## <a name="remarks"></a>Заметки

При добавлении разрешений с помощью действия [invite](../api/driveitem-invite.md) в объекте DriveRecipient могут быть указаны свойства **email**, **alias** и **objectId**. Достаточно указать только одно из этих значений.

<!-- {
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients"
} -->

