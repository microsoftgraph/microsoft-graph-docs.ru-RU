---
title: тип ресурса participant
description: Представляет тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 99f165f2f3e99ab424a318b053a060ccda8fdc1c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943719"
---
# <a name="participant-resource-type"></a>тип ресурса participant

Пространство имен: microsoft.graph

Представляет участника в вызове.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                 | Описание                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [Список участников](../api/participant-get.md)          | [participant](participant.md)                               | Получить список **объектов-участников** в вызове. |
| [Получение участника](../api/participant-get.md)           | [participant](participant.md)                               | Чтение свойств объекта **участника.** |
| [Удаление участника](../api/participant-delete.md)         | Нет   | Удаление участника в вызове.                  |
| [Приглашение](../api/participant-invite.md)                 | [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)                        | Приглашение участника на вызов.              |
| [Отключение звука участника](../api/participant-mute.md)         | [muteParticipantOperation](muteparticipantoperation.md)     | Отключить звук участника в вызове.                  |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | ИД участника.                                          |
| info                 | [participantInfo](participantinfo.md)    | Сведения об участнике.                          |
| isInLobby            | Boolean                                  | `true` если участник находится в "окле".                          |
| isMuted              | Boolean                                  | `true` если участник отключен (клиент или сервер отключен).    |
| mediaStreams         | [Коллекция mediaStream](mediastream.md) | Список потоков мультимедиа.                                   |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Сведения о том, есть ли у участника возможность записи. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

