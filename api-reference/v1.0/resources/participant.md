---
title: Тип ресурса участника
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f20bd68cbd4669c002edb37c2ab5fb0a7340dba4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866260"
---
# <a name="participant-resource-type"></a>Тип ресурса участника

Тип участника.

## <a name="methods"></a>Методы

| Метод                                                 | Возвращаемый тип                                                 | Описание                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [Получение участника](../api/participant-get.md)           | [participant](participant.md)                               | Чтение свойств объекта **участника** . |
| [Приглашение](../api/participant-invite.md)                 | [инвитепартиЦипантсоператион](../resources/inviteparticipantsoperation.md)                        | Приглашение участника на звонок.              |
| [Отключение звука участника](../api/participant-mute.md)         | [muteParticipantOperation](muteparticipantoperation.md)     | Отключение выключения участника в вызове.                  |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | Идентификатор участника.                                          |
| info                 | [participantInfo](participantinfo.md)    | Участник участника.                          |
| исинлобби            | Логический                                  | `true`Если участник находится в "зале ожидания".                          |
| Автозвук              | Логический                                  | `true`Если участник отключен (клиент или сервер выключен).    |
| медиастреамс         | Коллекция [медиастреам](mediastream.md) | Список потоков мультимедиа.                                   |

## <a name="relationships"></a>Отношения
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
