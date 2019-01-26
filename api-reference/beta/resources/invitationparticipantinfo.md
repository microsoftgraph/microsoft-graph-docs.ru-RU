---
title: Тип ресурса invitationParticipantInfo
description: '**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 666de597d40570a567ea88a375ab15d1e5f09038
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573601"
---
# <a name="invitationparticipantinfo-resource-type"></a>Тип ресурса invitationParticipantInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**InvitationParticipant** используется для представления набора удостоверения, связанного с приглашением беседы и предоставляет приглашение Дополнительные параметры.

## <a name="properties"></a>Свойства

| Свойство                           | Тип                          | Описание                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointType                       | operationStatus               | Возможные значения: `default`, `voicemail`. |
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
  "endpointType": "operationStatus",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
