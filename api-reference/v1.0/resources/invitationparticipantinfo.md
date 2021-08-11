---
title: тип ресурса invitationParticipantInfo
description: '**InvitationParticipant** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5b8432cf28dd078add91b517f75bc33a71fc4e8134ecff8155c97cc0acc887c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202247"
---
# <a name="invitationparticipantinfo-resource-type"></a>тип ресурса invitationParticipantInfo

Пространство имен: microsoft.graph

Этот ресурс используется для представления объекта, приглашенного на групповой вызов. 

## <a name="properties"></a>Свойства

| Свойство                           | Тип                          | Описание                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| удостоверение                           | [identitySet](identityset.md) | [IdentitySet,](identityset.md) связанный с этим приглашением.                   |
| replacesCallId                     | String                        | Необязательный параметр. Вызов, частью которого в настоящее время является тождественность целевого пользователя. Этот вызов будет отброшен после того, как будет добавлен участник. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

