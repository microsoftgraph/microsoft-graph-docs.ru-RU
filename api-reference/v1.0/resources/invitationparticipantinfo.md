---
title: Тип ресурса invitationParticipantInfo
description: '**InvitationParticipant** используется для представления набора удостоверений, связанных с приглашением к беседе, и предоставляет дополнительные параметры приглашения.'
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c09e15063524fbba0f9a53b69786545399c8e35a
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191684"
---
# <a name="invitationparticipantinfo-resource-type"></a>Тип ресурса invitationParticipantInfo

Пространство имен: microsoft.graph

Этот ресурс используется для представления сущности, которая приглашена на групповой вызов. 

## <a name="properties"></a>Свойства

| Свойство                           | Тип                          | Описание                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| Идентичности                           | [identitySet](identityset.md) | Набор [удостоверений,](identityset.md) связанный с этим приглашением.                   |
| participantId                      | Строка                        | Необязательный параметр. Идентификатор целевого участника.                                          |
| replacesCallId                     | Строка                        | Необязательный параметр. Вызов, частью которого в настоящее время является целевое удостоверение. При одноранговом случае вызов будет удален после успешного добавления участника. |

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
  "participantId": "String",  
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

