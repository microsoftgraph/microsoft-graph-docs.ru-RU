---
title: Тип участника ресурса
description: Тип участника.
ms.openlocfilehash: dcb456df0c7269bab91dcf593e674307db5358b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079310"
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
| id                   | String                                   | Код участника.                                          |
| сведения о                 | [participantInfo](participantinfo.md)    | Участник участника.                          |
| isInLobby            | boolean                                  | значение true, если участник в зале ожидания                          |
| isMuted              | boolean                                  | значение true, если выключен ли участника (клиент или сервер выключен ли)    |
| mediaStreams         | [mediaStream](mediastream.md) коллекции | Список мультимедийных потоков.                                   |
| метаданные             | String                                   | Большой двоичный объект данных, предоставленных участника в списке     |
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
