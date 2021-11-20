---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 4002e66e9362c52f1a062460ac1ebf64e855c85a
ms.sourcegitcommit: 1cf7a82df17afc6291e2c93d8b2c277bf3382e6a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2021
ms.locfileid: "61130145"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, включая URL-адрес собрания, список участников и описание.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип |Описание |
| ------ | ----------- | ---------- |
| [Создание](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Создание собрания в Интернете. |
| [Получение](../api/onlinemeeting-get.md); | [onlineMeeting](onlinemeeting.md) | Ознакомьтесь с свойствами и отношениями **объекта onlineMeeting.** |
| [Обновление](../api/onlinemeeting-update.md) | [onlineMeeting](onlinemeeting.md) | Обновление свойств объекта **onlineMeeting.** |
| [Удаление](../api/onlinemeeting-delete.md) | Нет | Удаление **объекта onlineMeeting.** |
| [Создание или доступ к onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте онлайн-собрание с пользовательским внешним ИД. Если собрание уже существует, извлекай его свойства. |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание    |
| :-------------------- | :-------------------------------------------- | :------------------------------------ |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)| Указывает, кто может быть презентовщиком на собрании. |
| allowAttendeeToEnableCamera | Логический | Указывает, могут ли участники включить камеру. |
| allowAttendeeToEnableMic | Логический | Указывает, могут ли участники включить микрофон. |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | Указывает режим чата собраний. |
| allowTeamworkReactions | Логический | Указывает, Teams для собрания включены Teams реакции. |
| alternativeRecording  | Stream | Поток контента альтернативной записи события [Microsoft Teams в прямом эфире](/microsoftteams/teams-live-events/what-are-teams-live-events). Только для чтения. |
| attendeeReport        | Stream | Поток контента отчета участника о событии [Teams в прямом эфире.](/microsoftteams/teams-live-events/what-are-teams-live-events) Только для чтения.   |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | Сведения о доступе к телефону для собрания в Интернете. Только для чтения. |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | Параметры, связанных с живым событием.      |
| chatInfo              | [chatInfo](chatinfo.md) | Сведения о чате, связанные с этой онлайн-встречей.  |
| creationDateTime      | Даты и время | Время создания собрания в UTC. Только для чтения.     |
| endDateTime           | Даты и время | Время окончания собрания в UTC.   |
| externalId            | String | Внешний ID. Пользовательский ID. Необязательный параметр.      |
| id | String | ID по умолчанию, связанный с онлайн-собранием. Только для чтения.    |
| isBroadcast | Логический | Указывает, является ли это событие [Teams в прямом эфире](/microsoftteams/teams-live-events/what-are-teams-live-events). |
| isEntryExitAnnounced  | Логический | Указывает, следует ли объявлять, когда звонители присоединяются или уходят. |
| joinWebUrl | Строка | URL-адрес присоединиться к собранию в Интернете. Только для чтения. |
| joinInformation | [itemBody](itembody.md) | Сведения о присоединиться в варианте языка и языка, указанном в заглавной странице HTTP-запроса "Accept-Language". Только для чтения. |
| lobbyBypassSettings | [lobbyBypassSettings](lobbyBypassSettings.md) | Указывает, какие участники могут обойти вестибюль собрания. |
| participants | [meetingParticipants](meetingparticipants.md) | Участники, связанные с онлайн-собранием. Это включает организатора и участников. |
| recordAutomatically | Логический | Указывает, следует ли записывать собрание автоматически. |
| запись | Stream | Поток контента записи события Teams [в прямом эфире](/microsoftteams/teams-live-events/what-are-teams-live-events). Только для чтения. |
| startDateTime | Даты и время | Время начала собрания в UTC. |
| subject | String | Тема собрания в Интернете. |
| videoTeleconferenceId | Строка | ID видеоконференции. Только для чтения. |
| autoAdmittedUsers (обесценив) | Строка | Параметр, который указывает тип участников, которые будут автоматически допущены к собранию в Интернете. Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Только для чтения. |
| возможности (неподготовленные) | коллекция meetingCapabilities | Список возможностей собраний. Возможные значения: `questionAndAnswer` , `unknownFutureValue` . |

> [!CAUTION]
>
>- Свойство **autoAdmittedUsers** обесценилось. Вместо этого **используйте** свойство [области lobbyBypassSettings.](lobbyBypassSettings.md)
>- Свойство **возможностей** неоценимо. Используйте **свойство isQuestionAndAnswerEnabled** [для broadcastMeetingSettings.](broadcastMeetingSettings.md)

### <a name="onlinemeetingpresenters-values"></a>значения onlineMeetingPresenters

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| все           | Каждый — это презентер (это параметр по умолчанию).             |
| organization       | Каждый в организации организатора — это презентер.          |
| roleIsPresenter    | Только участники, роль которых является презентатором, являются участниками. |
| organizer          | Только организатор — это презентер.                           |
| unknownFutureValue | Неизвестное будущее значение.                                         |

> [!TIP]
>
>- При создании или обновлении собрания  в Интернете со значением разрешенныхпрецентов, заданных, включаем полный список участников с заданными участниками роли, заданными в тексте `roleIsPresenter`   `presenter` запроса.
>- При создании или обновлении собрания  в Интернете со значением разрешенныхпрецентов, установленных для других значений, чем , роль участников будет показываться, как в `roleIsPresenter` теле  `null` ответа.

### <a name="meetingchatmode-values"></a>значения meetingChatMode

| Значение              | Описание                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| enabled            | Включен чат собраний.                                               |
| отключено           | Чат собраний отключен.                                              |
| ограниченный            | Чат собрания включен, но только на время собрания. |
| unknownFutureValue | Неизвестное будущее значение.                                                  |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| attendanceReports | [коллекция meetingAttendanceReport](meetingAttendanceReport.md) | Отчеты о посещаемости собрания в Интернете. Только для чтения. |
| регистрация | [meetingRegistration](meetingregistration.md) | Регистрация, включенная для собрания в Интернете. На одном собрании в Интернете может быть включена только одна регистрация.|
| meetingAttendanceReport (обесценена) | [meetingAttendanceReport](meetingAttendanceReport.md) | Отчет о посещаемости последнего сеанса собраний в Интернете. Только для чтения. |

> [!TIP]
> Свойство **meetingAttendanceReport** отстает. Он будет оставаться в бета-версии для обратной совместимости. В будущем используйте **свойство attendanceReports** для получения отчетов о посещаемости собрания в Интернете.

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
