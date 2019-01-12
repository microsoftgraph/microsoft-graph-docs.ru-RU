---
title: Тип ресурса invitationParticipantInfo
description: '**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8febd66915ee0b4fba26d9253cd56d67086e63bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982899"
---
# <a name="invitationparticipantinfo-resource-type"></a>Тип ресурса invitationParticipantInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.

## <a name="properties"></a>Свойства

| Свойство                           | Тип                          | Описание                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointType                       | String                        | Возможные значения: `default`, `voicemail`. |
| identity                           | [identitySet](identityset.md) | [IdentitySet](identityset.md) , связанной с приглашением.                   |
| languageId                         | Строка                        | Строка языка и региональных параметров языка.                                                                                     |
| область                             | Строка                        | Область участника.                                                           |
| replacesCallId                     | Строка                        | Необязательный параметр. Вызов которого idenity целевой в настоящее время является частью. Этот звонок будет удалена, после добавления участника. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
