---
title: Тип ресурса МитингпартиЦипантс
description: Участники собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d40479390703f50ac87b7c3196aa4d5bc55bc8a
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792767"
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
| Авторы | Коллекция [митингпартиЦипантинфо](meetingparticipantinfo.md) | Только для широковещательного собрания. |

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
