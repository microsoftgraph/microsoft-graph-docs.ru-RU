---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: e01ba9afac4e67c5442696e55246b92d1be65da7
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645444"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.

Этот ресурс поддерживает подписку на уведомления [об изменениях](/graph/webhooks). [Дополнительные сведения см. в статье "Подписка на собрания по](/graph/changenotifications-for-onlinemeeting) сети".

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип |Описание |
| ------ | ----------- | ---------- |
| [Создание](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети. |
| [Получение](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **onlineMeeting** . |
| [Обновление](../api/onlinemeeting-update.md) | [onlineMeeting](onlinemeeting.md) | Обновление свойств объекта **onlineMeeting** . |
| [Удаление](../api/onlinemeeting-delete.md) | Нет | Удаление объекта **onlineMeeting** . |
| [Создание или получение onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети с пользовательским внешним идентификатором. Если собрание уже существует, извлеките его свойства. |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание    |
| :-------------------- | :-------------------------------------------- | :------------------------------------ |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)| Указывает, кто может быть выступающим на собрании. |
| allowAttendeeToEnableCamera | Логическое | Указывает, могут ли участники включать камеру. |
| allowAttendeeToEnableMic | Логическое | Указывает, могут ли участники включать микрофон. |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | Задает режим чата собрания. |
| allowTeamworkReactions | Логическое | Указывает, включены ли реакции Teams на собрание. |
| alternativeRecording  | Stream | Поток содержимого альтернативной записи [трансляции Microsoft Teams](/microsoftteams/teams-live-events/what-are-teams-live-events). Только для чтения. |
| attendeeReport        | Stream | Поток содержимого отчета участника о [трансляции Teams](/microsoftteams/teams-live-events/what-are-teams-live-events). Только для чтения.   |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | Сведения о доступе по телефону (с телефонным входом) для собрания по сети. Только для чтения. |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | Параметры, связанные с трансляцией.      |
| chatInfo              | [chatInfo](chatinfo.md) | Сведения о чате, связанные с этим собранием по сети.  |
| creationDateTime      | DateTime | Время создания собрания в формате UTC. Только для чтения.     |
| endDateTime           | DateTime | Время окончания собрания в формате UTC.   |
| externalId            | String | Внешний идентификатор. Пользовательский идентификатор. Необязательное.      |
| id | String | Идентификатор по умолчанию, связанный с собранием по сети. Только для чтения.    |
| isBroadcast | Логическое | Указывает, является ли это [трансляцией Teams](/microsoftteams/teams-live-events/what-are-teams-live-events). |
| isEntryExitAnnounced  | Логический | Указывает, следует ли объявлять о присоединении или выходе вызывающих абонентов. |
| joinWebUrl | String | URL-адрес присоединения к собранию по сети. Только для чтения. |
| joinInformation | [itemBody](itembody.md) | Сведения о соединении на языке и варианте языкового стандарта, указанные в заголовке HTTP запроса Accept-Language. Только для чтения. |
| joinMeetingIdSettings | [joinMeetingIdSettings](joinmeetingidsettings.md) | Указывает **joinMeetingId**, секретный код собрания и требование секретного кода. |
| lobbyBypassSettings | [lobbyBypassSettings](lobbyBypassSettings.md) | Указывает, какие участники могут обходить зал ожидания собрания. |
| participants | [meetingParticipants](meetingparticipants.md) | Участники, связанные с онлайн-собранием. К ним относятся организатор и участники. |
| recordAutomatically | Логическое | Указывает, следует ли записывать собрание автоматически. |
| Записи | Stream | Поток содержимого записи трансляции [Teams](/microsoftteams/teams-live-events/what-are-teams-live-events). Только для чтения. |
| startDateTime | DateTime | Время начала собрания в формате UTC. |
| subject | String | Тема собрания по сети. |
| videoTeleconferenceId | String | Идентификатор видеоконференции. Только для чтения. |
| autoAdmittedUsers (не рекомендуется) | String | Параметр, указывающий тип участников, которые будут автоматически разрешены в онлайн-собрании. Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Только для чтения. |
| возможности (нерекомендуемые) | Коллекция meetingCapabilities | Список возможностей собраний. Возможные значения: `questionAndAnswer`,`unknownFutureValue`. |

> [!CAUTION]
>
>- Свойство **autoAdmittedUsers** является устаревшим. Используйте свойство **области** [lobbyBypassSettings](lobbyBypassSettings.md) .
>- Свойство **capabilities** является устаревшим. Используйте свойство **isQuestionAndAnswerEnabled** [объекта broadcastMeetingSettings](broadcastMeetingSettings.md) .

### <a name="onlinemeetingpresenters-values"></a>Значения onlineMeetingPresenters

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| Все           | Все — выступающие (это параметр по умолчанию).             |
| organization;       | Все участники организации организатора — выступающие.          |
| roleIsPresenter    | Выступающими являются только участники, роль которых является выступающим. |
| organizer          | Выступающим является только организатор.                           |
| unknownFutureValue | Неизвестное будущее значение.                                         |

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

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| attendanceReports | [Коллекция meetingAttendanceReport](meetingAttendanceReport.md) | Отчеты об участии в собрании по сети. Только для чтения. |
| Регистрации | [meetingRegistrationBase](meetingregistrationbase.md) | Регистрация, включенная для собрания по сети. Для одного собрания по сети может быть включена только одна регистрация.|
| meetingAttendanceReport (не рекомендуется) | [meetingAttendanceReport](meetingAttendanceReport.md) | Отчет об участии в последнем онлайн-сеансе собрания. Только для чтения. |

> [!TIP]
>
>- Свойство **meetingAttendanceReport** является устаревшим. Он останется в бета-версии для обеспечения обратной совместимости. В дальнейшем используйте свойство **attendanceReports** для получения отчетов об участии в собрании по сети.
>- Тип **регистрации может** быть [meetingRegistration](meetingregistration.md) или [externalMeetingRegistration](externalmeetingregistration.md), которые наследуются от [meetingRegistrationBase](meetingregistrationbase.md).

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
  "allowAttendeeToEnableCamera": "Boolean",
  "allowAttendeeToEnableMic": "Boolean",
  "allowedPresenters": "String",
  "allowMeetingChat": {"@odata.type": "microsoft.graph.meetingChatMode"},
  "allowTeamworkReactions": "Boolean",
  "audioConferencing": {"@odata.type": "microsoft.graph.audioConferencing"},
  "broadcastSettings": {"@odata.type": "microsoft.graph.broadcastSettings"},
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",  
  "isBroadcast": "Boolean",
  "isEntryExitAnnounced": "Boolean",
  "joinMeetingIdSettings": {"@odata.type": "microsoft.graph.joinMeetingIdSettings"},
  "joinWebUrl": "String",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
  "participants": {"@odata.type": "microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",  
  "subject": "String",
  "videoTeleconferenceId": "String"
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
