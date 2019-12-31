---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3bcce64ab900dae7c7f13d7da0c3d34d164fd35d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913522"
---
# <a name="meetingparticipants-resource-type"></a>Тип ресурса МитингпартиЦипантс

Участники собрания.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| attendees | Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md) |  |
| organizer | [митингпартиЦипантинфо](meetingparticipantinfo.md) |  |

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
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
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
