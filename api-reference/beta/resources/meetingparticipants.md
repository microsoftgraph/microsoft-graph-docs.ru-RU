---
title: тип ресурса meetingParticipants
description: Участники собрания.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 93ca3d73518f9739cc3115c80efd2aec551629b5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944165"
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


