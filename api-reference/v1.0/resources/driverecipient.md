---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4792a943598911cc2f0b8329016469ca157bda58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562722"
---
# <a name="driverecipient-resource"></a>Ресурс DriveRecipient

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
