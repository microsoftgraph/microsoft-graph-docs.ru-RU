---
title: Тип участника ресурса
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f49526824b2b6c4eb4a5065f05ab4c765d299faa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508148"
---
# <a name="participant-resource-type"></a>Тип участника ресурса

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| Метаданные             | String                                   | Большой двоичный объект данных, предоставленных участника в списке     |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Сведения о ли участник имеет возможность записи. |

## <a name="relationships"></a>Отношения
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
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/participant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
