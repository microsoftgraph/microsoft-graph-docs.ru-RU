---
title: Тип ресурса ИнвитатионпартиЦипантинфо
description: '**ИнвитатионпартиЦипант** используется для представления набора удостоверений, связанных с приглашением на беседу, и предоставляет дополнительные параметры приглашения.'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8b42e89f89332e58fa2f7edcf39c774446c6b9d9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913403"
---
# <a name="invitationparticipantinfo-resource-type"></a>Тип ресурса ИнвитатионпартиЦипантинфо

Этот ресурс используется для представления объекта, приглашенного на вызов группы. 

## <a name="properties"></a>Свойства

| Свойство                           | Тип                          | Описание                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| хищения                           | [identitySet](identityset.md) | [Удостоверение](identityset.md) , связанное с этим приглашением.                   |
| реплацескаллид                     | String                        | Необязательный параметр. Вызов, частью которого в данный момент является целевое удостоверение. Этот вызов будет сброшен после добавления участника. |

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
