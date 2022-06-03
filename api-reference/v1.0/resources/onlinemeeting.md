---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 31d0d6262c9f0784b2a609b29221a51f6e871c96
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883819"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

Пространство имен: microsoft.graph

Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Создание объекта onlineMeeting](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети.                                                                                    |
| [Получение onlineMeeting](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **onlineMeeting** .                                        |
| [Обновление](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | Обновление свойств объекта **onlineMeeting** . |
| [Удаление onlineMeeting](../api/onlinemeeting-delete.md)             | Нет                              | Удаление объекта **onlineMeeting** .                                                                                    |
| [Создание или получение onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте **объект onlineMeeting** с пользовательским внешним идентификатором. Если собрание уже существует, извлеките его свойства. |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)                       | Указывает, кто может быть выступающим на собрании. Возможные значения перечислены в следующей таблице.                          |
| allowAttendeeToEnableCamera     | Boolean                       | Указывает, могут ли участники включать камеру.                          |
| allowAttendeeToEnableMic     | Boolean                       | Указывает, могут ли участники включать микрофон.                          |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | Задает режим чата собрания. |
| allowTeamworkReactions | Boolean | Указывает, включены ли реакции Teams на собрание. |
| attendeeReport | Stream | Поток содержимого отчета участника о [трансляции Microsoft Teams](/microsoftteams/teams-live-events/what-are-teams-live-events). Только для чтения. |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | Сведения о доступе по телефону (с телефонным входом) для собрания по сети. Только для чтения.                                                   |
| broadcastSettings              | [broadcastMeetingSettings](broadcastMeetingSettings.md)                      | Параметры, связанные с трансляцией.                                                                  |
| chatInfo              | [chatInfo](chatinfo.md)                       | Сведения о чате, связанные с этим собранием по сети.                                                                  |
| creationDateTime      | DateTime                                      | Время создания собрания в формате UTC. Только для чтения.                                                                               |
| endDateTime           | DateTime                                      | Время окончания собрания в формате UTC.                                                                                               |
| id                    | Строка                                        | Идентификатор по умолчанию, связанный с собранием по сети. Только для чтения.                                                              |
| isBroadcast  | Boolean                                       | Указывает, является ли это [трансляцией Teams](/microsoftteams/teams-live-events/what-are-teams-live-events).                  |
| isEntryExitAnnounced  | Boolean                                       | Указывает, следует ли объявлять о присоединении или выходе вызывающих абонентов.                                                                     |
| joinInformation       | [itemBody](itembody.md)                       | Сведения о соединении на языке и варианте языкового стандарта, указанном в заголовке `Accept-Language` HTTP запроса. Только для чтения. |
| joinWebUrl            | Строка                                        | URL-адрес присоединения к собранию по сети. Только для чтения.                                                                             |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Указывает, какие участники могут обходить зал ожидания собрания.                                                               |
| participants          | [meetingParticipants](meetingparticipants.md) | Участники, связанные с онлайн-собранием.  К ним относятся организатор и участники.                       |
| recordAutomatically | Boolean | Указывает, следует ли записывать собрание автоматически. |
| startDateTime         | DateTime                                      | Время начала собрания в формате UTC.                                                                                             |
| subject               | String                                        | Тема собрания по сети.                                                                                         |
| videoTeleconferenceId | Строка                                        | Идентификатор видеоконференции. Только для чтения.                                                                                  |

### <a name="onlinemeetingpresenters-values"></a>Значения onlineMeetingPresenters

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| Все           | Все — выступающие (это параметр по умолчанию).             |
| organization;       | Все участники организации организатора — выступающие.          |
| roleIsPresenter    | Выступающими являются только участники, роль которых является выступающим. |
| organizer          | Выступающим является только организатор.                           |
| unknownFutureValue | Отменить будущие значения.                                          |

> [!TIP]
>
> При создании или обновлении собрания по сети с параметром **allowedPresenters** `roleIsPresenter` `presenter` добавьте полный список участников с  заданной ролью участника в тексте запроса.

### <a name="meetingchatmode-values"></a>Значения meetingChatMode

| Значение              | Описание                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| enabled            | Чат собрания включен.                                               |
| отключено           | Чат собрания отключен.                                              |
| Ограниченное            | Чат собрания включен, но только на время собрания. |
| unknownFutureValue | Неизвестное будущее значение.                                                  |

## <a name="relationships"></a>Отношения

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| attendanceReports | [Коллекция meetingAttendanceReport](meetingAttendanceReport.md) | Отчеты об участии в собрании по сети. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String",
  "isBroadcast": "Boolean",
  "broadcastSettings": {"@odata.type": "microsoft.graph.broadcastSettings"},
  "allowMeetingChat": {"@odata.type": "microsoft.graph.meetingChatMode"},
  "allowTeamworkReactions": "Boolean",
  "allowAttendeeToEnableMic": "Boolean",
  "allowAttendeeToEnableCamera": "Boolean"
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

