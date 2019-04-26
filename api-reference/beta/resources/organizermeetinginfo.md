---
title: Тип ресурса Организермитингинфо
description: Сведения о собрании, содержащие организатора собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 129e8a60edd89d45eb6e48715a59231475d52b99
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341763"
---
# <a name="organizermeetinginfo-resource-type"></a>Тип ресурса Организермитингинфо

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о собрании, содержащие организатора собрания.

## <a name="properties"></a>Свойства

| Свойство                     | Тип                          | Описание                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| Алловконверсатионвисаусост | Логический                       | Указывает, может ли беседа продолжиться после закрытия узла беседы. |
| organizer                    | [identitySet](identityset.md) | Удостоверение Azure Active Directory для организатора.  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.meetingInfo",
   "openType": true,
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "microsoft.graph.identitySet" }
}
```

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
