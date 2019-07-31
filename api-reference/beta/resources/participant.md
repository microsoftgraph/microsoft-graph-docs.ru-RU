---
title: Тип ресурса участника
description: Тип участника.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a903eb34191401100d9b19aa17eba6fb9f5c6617
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009218"
---
# <a name="participant-resource-type"></a>Тип ресурса участника

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип участника.

## <a name="methods"></a>Методы

| Метод                                                          | Возвращаемый тип                              | Описание                                       |
|:----------------------------------------------------------------|:-----------------------------------------|:--------------------------------------------------|
| [Получение участника](../api/participant-get.md)                    | [абонент](participant.md)            | Чтение свойств объекта **участника** .    |
| [Конфигуремиксер](../api/participant-configuremixer.md)          | [commsOperation](commsoperation.md)      | Настройка микшера звука участника.            |
| [Приглашение](../api/participant-invite.md)                          | [commsOperation](commsoperation.md)      | Приглашение участника на звонок.                 |
| [Отключение звука для участника](../api/participant-mute.md)                  | [commsOperation](commsoperation.md)      | Отключение выключения участника в вызове.                     |
| [Отключение выключения всех участников](../api/participant-muteall.md)          | [commsOperation](commsoperation.md)      | Отключение выключения всех участников собрания.         |

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | Идентификатор участника.                                          |
| info                 | [participantInfo](participantinfo.md)    | Участник участника.                          |
| Исинлобби            | boolean                                  | true, если участник находится в зале ожидания                          |
| Автозвук              | boolean                                  | true, если участник отключен (клиент или сервер выключен)    |
| Медиастреамс         | Коллекция [медиастреам](mediastream.md) | Список потоков мультимедиа.                                   |
| метаданных             | String                                   | Большой двоичный объект данных, предоставляемый участником в списке     |
| Рекордингинфо        | [Рекордингинфо](recordinginfo.md)        | Сведения о том, имеет ли участник возможность записи. |

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
  "suppressions": []
}
-->
