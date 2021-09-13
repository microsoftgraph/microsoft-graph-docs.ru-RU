---
title: тип ресурса invitationParticipantInfo
description: '**InvitationParticipant** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f048fae8d5d63aac8a64dc0e8d3193de5cc5aef5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084428"
---
# <a name="invitationparticipantinfo-resource-type"></a>тип ресурса invitationParticipantInfo

Пространство имен: microsoft.graph

Этот ресурс используется для представления объекта, приглашенного на групповой вызов. 

## <a name="properties"></a>Свойства

| Свойство                           | Тип                          | Описание                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| удостоверение                           | [identitySet](identityset.md) | [IdentitySet,](identityset.md) связанный с этим приглашением.                   |
| replacesCallId                     | String                        | Необязательный параметр. Вызов, частью которого в настоящее время является тождественность целевого пользователя. Этот вызов будет отброшен после того, как будет добавлен участник. |

## <a name="json-representation"></a>Представление в формате JSON

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

