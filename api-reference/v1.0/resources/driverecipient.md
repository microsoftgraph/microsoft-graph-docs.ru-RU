---
author: JeremyKelley
ms.date: 09/10/2017
title: DriveRecipient
localization_priority: Normal
ms.prod: sharepoint
description: Ресурс DriveRecipient представляет человека, группу или другого получателя, которому можно предоставить доступ с помощью действия invite.
doc_type: resourcePageType
ms.openlocfilehash: 72bb8c3ab42dc6240d6c088a6634f969dd6a03e14c71053c12a3abc742247093
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54149991"
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

