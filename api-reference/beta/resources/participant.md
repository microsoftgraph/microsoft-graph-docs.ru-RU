---
title: Тип участника ресурса
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d6a4474525086fb1e8aefe00ad37acaf6511e9f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938334"
---
# <a name="participant-resource-type"></a>Тип участника ресурса

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Тип участника.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип                              | Описание                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [Получение участников](../api/participant-get.md)                    | [Участник](participant.md)            | Чтение свойств объекта **участника** .    |
| [ConfigureMixer](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | Настройка участников аудиомикшеру.            |
| [Приглашение](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | Приглашение участников к звонку.                 |
| [Отключить участников](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | Отключение микрофона участника в ходе вызова.                     |
| [Отключение всех участников](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | Отключение всех участников собрания.         |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | Строка                                   | Код участника.                                          |
| сведения о                 | [participantInfo](participantinfo.md)    | Участник участника.                          |
| isInLobby            | boolean                                  | значение true, если участник в зале ожидания                          |
| isMuted              | boolean                                  | значение true, если выключен ли участника (клиент или сервер выключен ли)    |
| mediaStreams         | [mediaStream](mediastream.md) коллекции | Список мультимедийных потоков.                                   |
| метаданные             | Строка                                   | Большой двоичный объект данных, предоставленных участника в списке     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Сведения о ли участник имеет возможность записи. |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

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
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ],
  "metadata": "String",
  "recordingInfo": { "@odata.type": "#microsoft.graph.recordingInfo" }
}
```

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "en-US",
    "region": "westus"
  },
  "isInLobby": false,
  "isMuted": false,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
