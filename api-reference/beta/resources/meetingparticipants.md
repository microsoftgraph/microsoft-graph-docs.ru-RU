---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 66bb521ae9a2222b5ea60709ac3687da930161d6
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913557"
---
# <a name="meetingparticipants-resource-type"></a>Тип ресурса МитингпартиЦипантс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Участники собрания.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| attendees | Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md) |  |
| organizer | [митингпартиЦипантинфо](meetingparticipantinfo.md) |  |
| производители | Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md) | Только для широковещательного собрания. |
| участники | Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md) | Только для широковещательного собрания. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
  "producers": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "contributors": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
