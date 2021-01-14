---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 139cd4a20a6097691189d1bd1f843850ba911a21
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866111"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

Пространство имен: microsoft.graph

Содержит сведения о собрании, включая URL-адрес, используемый для присоединиться к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Создание объекта onlineMeeting](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Создание собрания по сети.                                                                                    |
| [Get onlineMeeting](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **onlineMeeting.**                                        |
| [Удаление onlineMeeting](../api/onlinemeeting-delete.md)             | Нет                              | Удаление собрания по сети.                                                                                    |
| [Создание или get onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создание собрания по сети с пользовательским внешним ИД. Если собрание уже существует, извлекаете его свойства. |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | Сведения о телефонном доступе (с телефонным доступом) для собрания по сети. Только для чтения.                                                   |
| chatInfo              | [chatInfo](chatinfo.md)                       | Сведения чата, связанные с этим собранием по сети.                                                                  |
| creationDateTime      | DateTime                                      | Время создания собрания в UTC. Только для чтения.                                                                               |
| startDateTime         | DateTime                                      | Время начала собрания в UTC.                                                                                             |
| endDateTime           | DateTime                                      | Время окончания собрания в UTC.                                                                                               |
| id                    | String                                        | ИД по умолчанию, связанный с собранием по сети. Только для чтения.                                                              |
| joinWebUrl            | String                                        | URL-адрес собрания по сети. Только для чтения.                                                                             |
| participants          | [meetingParticipants](meetingparticipants.md) | Участники, связанные с онлайн-собранием.  К ним относятся организатор и участники.                       |
| subject               | String                                        | Тема собрания по сети.                                                                                         |
| videoTeleconferenceId | String                                        | ИД видеоконференции. Только для чтения.                                                                                  |
| joinInformation       | [itemBody](itembody.md)                       | Сведения о подступах к языку и языковом варианте, указанные в `Accept-Language` http-заголке запроса. Только для чтения. |
| isEntryExitAnnounced  | Логический                                       | Следует ли объявлять, когда звонят, присоединяться или уходить.                                                                     |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Указывает, какие участники могут обходить "lobby" собрания.                                                               |
| allowedPresenters     | onlineMeetingPresenters                       | Указывает, кто может быть presenter в собрании. Возможные значения перечислены в следующей таблице.                          |

### <a name="onlinemeetingpresenters-values"></a>Значения onlineMeetingPresenters

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| все           | Все — это presenter (это параметр по умолчанию).             |
| organization;       | Все в организации организатора — это организатор.          |
| roleIsPresenter    | Только участники, роль которых является presenter, являются участниками. |
| organizer          | Только организатор является организатором.                           |
| unknownFutureValue | Unknow future value.                                          |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

