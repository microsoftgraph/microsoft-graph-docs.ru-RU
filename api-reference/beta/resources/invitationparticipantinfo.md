---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569966"
---
# <a name="invitationparticipantinfo-resource-type"></a>Тип ресурса ИнвитатионпартиЦипантинфо

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.

## <a name="properties"></a>Свойства

| Свойство                           | Тип                          | Описание                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| Ендпоинттипе                       | String                        | Возможные значения: `default`, `voicemail`. |
| хищения                           | [identitySet](identityset.md) | [Удостоверение](identityset.md) , связанное с этим приглашением.                   |
| languageId                         | String                        | Строка языка и региональных параметров языка.                                                                                     |
| региональных                             | String                        | Регион участника.                                                           |
| Реплацескаллид                     | String                        | Необязательное свойство. Вызов, частью которого в данный момент является целевой иденити. Этот вызов будет сброшен после добавления участника. |

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
