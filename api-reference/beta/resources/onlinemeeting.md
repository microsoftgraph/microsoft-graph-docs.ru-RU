---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: fedfb6a7558e081bb333c1fc6f579f2600137e9c
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866230"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, включая URL-адрес, используемый для присоединиться к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                       |
| :----------------------------------------------------------------- | :-------------------------------- | :---------------------------------------------------------------------------------------------------------------- |
| [Создание](../api/application-post-onlineMeetings.md)                | [onlineMeeting](onlinemeeting.md) | Создание собрания по сети.                                                                                         |
| [Get](../api/onlinemeeting-get.md)                                 | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **onlineMeeting.**                                             |
| [Создание или get onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создание собрания по сети с пользовательским внешним ИД. Если собрание уже существует, извлекаете его свойства.      |
| [обновление](../api/onlinemeeting-update.md).                           | [onlineMeeting](onlinemeeting.md) | Обновление свойств **startDateTime,** **endDateTime**, **subject** и **участников** собрания по сети. |
| [удаление](../api/onlinemeeting-delete.md);                           | Нет                              | Удаление ресурса **onlineMeeting.**                                                                             |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание                                                                                                                                                                                                                                                 |
| :-------------------- | :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| autoAdmittedUsers     | String                                        | Параметр, который определяет тип участников, которые будут автоматически разрешены в собрании по сети. Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Только для чтения. |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | Сведения о телефонном доступе (с телефонным доступом) для собрания по сети. Только для чтения.                                                                                                                                                                                    |
| chatInfo              | [chatInfo](chatinfo.md)                       | Сведения чата, связанные с этим собранием по сети.                                                                                                                                                                                                   |
| creationDateTime      | DateTime                                      | Время создания собрания в UTC. Только для чтения.                                                                                                                                                                                                                |
| startDateTime         | DateTime                                      | Время начала собрания в UTC.                                                                                                                                                                                                                              |
| endDateTime           | DateTime                                      | Время окончания собрания в UTC.                                                                                                                                                                                                                                |
| id                    | String                                        | ИД по умолчанию, связанный с собранием по сети. Только для чтения.                                                                                                                                                                                               |
| joinWebUrl            | String                                        | URL-адрес собрания по сети. Только для чтения.                                                                                                                                                                                                              |
| participants          | [meetingParticipants](meetingparticipants.md) | Участники, связанные с онлайн-собранием.  К ним относятся организатор и участники.                                                                                                                                                        |
| subject               | String                                        | Тема собрания по сети.                                                                                                                                                                                                                          |
| capabilities          | Коллекция объектов string                             | Список возможностей собраний. Возможные значения: `questionAndAnswer` .                                                                                                                                                                                 |
| videoTeleconferenceId | String                                        | ИД видеоконференции. Только для чтения.                                                                                                                                                                                                                   |
| joinInformation       | [itemBody](itembody.md)                       | Сведения о подступах к языку и языковом варианте, указанные в HTTP-заголке HTTP-запроса "Accept-Language". Только для чтения                                                                                                                                       |
| externalId            | String                                        | Внешний ИД. Настраиваемый ИД. Необязательный.                                                                                                                                                                                                                     |
| isEntryExitAnnounced  | Логический                                       | Следует ли объявлять, когда звонят, присоединяться или уходить.                                                                                                                                                                                                      |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Указывает, какие участники могут обходить "lobby" собрания.                                                                                                                                                                                                  |
| allowedPresenters     | onlineMeetingPresenters                       | Указывает, кто может быть presenter в собрании. Возможные значения: `everyone` `organization` , и `roleIsPresenter` `organizer` `unknownFutureValue` .                                                                                                    |
| isBroadcast           | Логический                                       | Указывает, является ли это трансляцией.                                                                                                                                                                                                                   |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | Параметры, связанные с трансляцией*                                                                                                                                                                                                                    |
| attendeeReport        | Поток                                        | Поток содержимого отчета об участниках трансляции. Только для чтения.                                                                                                                                                                                       |
| recording             | Поток                                        | Поток содержимого записи трансляции. Только для чтения.                                                                                                                                                                                             |
| alternativeRecording  | Поток                                        | Поток содержимого альтернативной записи трансляции. Только для чтения.                                                                                                                                                                                 |

> [!IMPORTANT]
> Свойство **autoAdmittedUsers** устарело. Вместо **этого используйте lobbyBypassSettings.scope** для настройки вариантов собраний.
> 
> *\Creating live events with the **broadcastSettings** property is in Beta, with important limitations. Дополнительные сведения можно найти [в broadcastSettings.](broadcastMeetingSettings.md)

### <a name="onlinemeetingpresenters-values"></a>Значения onlineMeetingPresenters

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| все           | Все — это presenter (это параметр по умолчанию).             |
| organization;       | Все в организации организатора — это организатор.          |
| roleIsPresenter    | Только участники, роль которых является presenter, являются участниками. |
| organizer          | Только организатор является организатором.                           |
| unknownFutureValue | Неизвестное будущее значение.                                         |

**Примечание.** Если для **свойства allowedPresenters** установлено значение , укажите роль каждого участника собрания, используя свойство role в `roleIsPresenter` [meetingParticipantInfo.](../resources/meetingparticipantinfo.md) 

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "externalId"
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
  "capabilities": [ "questionAndAnswer" ],
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String",
  "isBroadcast": "Boolean",
  "broadcastSettings": {"@odata.type": "#microsoft.graph.broadcastSettings"}
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


