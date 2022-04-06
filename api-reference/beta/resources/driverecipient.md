---
author: JeremyKelley
description: Ресурс driveRecipient представляет человека, группу или другого получателя, который должен делиться с помощью действия приглашения.
ms.date: 09/10/2017
title: DriveRecipient
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1b7b666e520af98fd6fae193b770357a7813504e
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722579"
---
# <a name="driverecipient-resource"></a>ресурс driveRecipient

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет человека, группу или другого получателя для обмена элементом диска с помощью действия [приглашения](../api/driveitem-invite.md) .

При использовании [приглашения](../api/driveitem-invite.md) для добавления разрешений объект **driveRecipient** может указать адрес электронной почты **, псевдоним** или **objectId** получателя. 
Требуется только одно из этих значений; несколько значений не принимаются.

## <a name="properties"></a>Свойства

Ниже перечислены свойства ресурса получателя.

| Свойство | Тип   | Описание                                                                                             |
| :------- | :----- | :------------------------------------------------------------------------------------------------------ |
| email    | String | Электронный адрес получателя (если с получателем связан электронный адрес).                  |
| alias    | String | Псевдоним объекта домена для тех случаев, когда электронный адрес недоступен (например, для групп безопасности). |
| objectId | String | Уникальный идентификатор получателя в каталоге.                                               |

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

<!--
{
  "type": "#page.annotation",
  "description": "Recipients resource defines a single recipient for the sharing invitation and permissions collection.",
  "keywords": "sharing,share,permissions,action.invite,invite,email",
  "section": "documentation",
  "tocPath": "Resources/Recipients",
  "suppressions": []
}
-->
