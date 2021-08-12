---
title: тип ресурса участника
description: Представляет тип участника.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0e4da220f260ff6f130ac3f632ea2496d9bb24b7e5b12530d16afed2b42e94ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152343"
---
# <a name="participant-resource-type"></a>тип ресурса участника

Пространство имен: microsoft.graph

Представляет участника вызова.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                 | Описание                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [Участник списка](../api/participant-get.md)          | [participant](participant.md)                               | Извлечение списка **объектов-участников** вызова. |
| [Получение участника](../api/participant-get.md)           | [participant](participant.md)                               | Чтение свойств **объекта-участника.** |
| [Удаление участника](../api/participant-delete.md)         | Нет   | Удаление участника вызова.                  |
| [Приглашение](../api/participant-invite.md)                 | [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)                        | Приглашайте участника на вызов.              |
| [Отключение звука участника](../api/participant-mute.md)         | [muteParticipantOperation](muteparticipantoperation.md)     | Отключить участника вызова.                  |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | ID участника.                                          |
| info                 | [participantInfo](participantinfo.md)    | Сведения о участнике.                          |
| isInLobby            | Логическое                                  | `true` если участник находится в вестибюле.                          |
| isMuted              | Логическое                                  | `true` если участник отключен (клиент или сервер отключен).    |
| mediaStreams         | [коллекция mediaStream](mediastream.md) | Список потоков мультимедиа.                                   |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Сведения о том, имеет ли участник возможность записи. |

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

