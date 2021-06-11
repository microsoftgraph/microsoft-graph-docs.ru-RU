---
title: тип ресурса meetingParticipants
description: Участники собрания.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ee5cf115a80c642f5442230d7111dfaeffca930
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896622"
---
# <a name="meetingparticipants-resource-type"></a>тип ресурса meetingParticipants

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Участники собрания.

## <a name="properties"></a>Свойства

| Свойство                  | Тип                                                           | Описание                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| attendees                 | [коллекция meetingParticipantInfo](meetingparticipantinfo.md) | Сведения участников собрания. |
| organizer                 | [meetingParticipantInfo](meetingparticipantinfo.md)            | Сведения организатора собрания. |
| производители (неподготовленные)    | [коллекция meetingParticipantInfo](meetingparticipantinfo.md) | Только для собрания трансляции.           |
| вкладчики (неподготовленные) | [коллекция meetingParticipantInfo](meetingparticipantinfo.md) | Только для собрания трансляции.           |

> [!CAUTION]
> Свойства **производителей** и **авторов** неоценимы. Все участники собрания возвращаются в **коллекцию участников.** Используйте **свойство role** [meetingParticipantInfo](meetingparticipantinfo.md) для определения роли собрания участника.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
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


