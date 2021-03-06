---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: db18746a74db9ebc9f6eb19ed55ae3e7b019a77f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515863"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, включая URL-адрес собрания, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                       |
| :----------------------------------------------------------------- | :-------------------------------- | :---------------------------------------------------------------------------------------------------------------- |
| [Создание](../api/application-post-onlineMeetings.md)                | [onlineMeeting](onlinemeeting.md) | Создание собрания в Интернете.                                                                                         |
| [получение](../api/onlinemeeting-get.md);                                 | [onlineMeeting](onlinemeeting.md) | Ознакомьтесь с свойствами и отношениями **объекта onlineMeeting.**                                             |
| [обновление](../api/onlinemeeting-update.md).                           | [onlineMeeting](onlinemeeting.md) | Обновление свойств объекта **onlineMeeting.** |
| [удаление](../api/onlinemeeting-delete.md);                           | Нет                              | Удаление **объекта onlineMeeting.**                                                                             |
| [Создание или доступ к onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте онлайн-собрание с пользовательским внешним ИД. Если собрание уже существует, извлекай его свойства.      |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание                                                                                                                                                                                                                                                 |
| :-------------------- | :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | onlineMeetingPresenters                       | Указывает, кто может быть презентовщиком на собрании. Возможные значения `everyone` : , , , и `organization` `roleIsPresenter` `organizer` `unknownFutureValue` .                                                                                                    |
| alternativeRecording  | Stream                                        | Поток контента альтернативной записи живого события. Только для чтения.                                                                                                                                                                                 |
| attendeeReport        | Stream                                        | Поток контента отчета участника о событии в прямом эфире. Только для чтения.                                                                                                                                                                                       |
| autoAdmittedUsers     | String                                        | Параметр, который указывает тип участников, которые будут автоматически допущены к собранию в Интернете. Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Только для чтения. |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | Сведения о доступе к телефону для собрания в Интернете. Только для чтения.                                                                                                                                                                                    |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | Параметры, связанные с живым событием*                                                                                                                                                                                                                    |
| chatInfo              | [chatInfo](chatinfo.md)                       | Сведения о чате, связанные с этой онлайн-встречей.                                                                                                                                                                                                   |
| creationDateTime      | DateTime                                      | Время создания собрания в UTC. Только для чтения.                                                                                                                                                                                                                |
| capabilities          | Коллекция String                             | Список возможностей собраний. Возможные значения: `questionAndAnswer` .                                                                                                                                                                                 |
| endDateTime           | DateTime                                      | Время окончания собрания в UTC.                                                                                                                                                                                                                                |
| externalId            | String                                        | Внешний ID. Пользовательский ID. Необязательный атрибут.                                                                                                                                                                                                                     |
| id                    | String                                        | ID по умолчанию, связанный с онлайн-собранием. Только для чтения.                                                                                                                                                                                               |
| isBroadcast           | Boolean                                       | Указывает, является ли это событием в прямом эфире.                                                                                                                                                                                                                   |
| isEntryExitAnnounced  | Boolean                                       | Следует ли объявлять о том, когда звонители присоединяются или уходят.                                                                                                                                                                                                      |
| joinWebUrl            | String                                        | URL-адрес присоединиться к собранию в Интернете. Только для чтения.                                                                                                                                                                                                              |
| joinInformation       | [itemBody](itembody.md)                       | Сведения о присоединиться в варианте языка и языка, указанном в заглавной странице HTTP-запроса "Accept-Language". Только для чтения                                                                                                                                       |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Указывает, какие участники могут обойти вестибюль собрания.                                                                                                                                                                                                  |
| participants          | [meetingParticipants](meetingparticipants.md) | Участники, связанные с онлайн-собранием.  Это включает организатора и участников.                                                                                                                                                        |
| запись             | Stream                                        | Поток контента записи живого события. Только для чтения.                                                                                                                                                                                             |
| startDateTime         | DateTime                                      | Время начала собрания в UTC.                                                                                                                                                                                                                              |
| subject               | String                                        | Тема собрания в Интернете.                                                                                                                                                                                                                          |
| videoTeleconferenceId | String                                        | ID видеоконференции. Только для чтения.                                                                                                                                                                                                                   |

> [!IMPORTANT]
> Свойство **autoAdmittedUsers** устарело. Используйте **lobbyBypassSettings.scope** вместо конфигураций вариантов собраний.
> 
> *\Создание событий в прямом эфире с **свойством broadcastSettings** находится в бета-версии с важными ограничениями. Дополнительные сведения можно получить [в broadcastSettings.](broadcastMeetingSettings.md)

### <a name="onlinemeetingpresenters-values"></a>значения onlineMeetingPresenters

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| все           | Каждый — это презентер (это параметр по умолчанию).             |
| organization;       | Каждый в организации организатора — это презентер.          |
| roleIsPresenter    | Только участники, роль которых является презентатором, являются участниками. |
| organizer          | Только организатор — это презентер.                           |
| unknownFutureValue | Неизвестное будущее значение.                                         |

**Примечание.** Если установлено значение **allowedPresenters,** укажите роль собрания каждого участника собрания, используя свойство role в `roleIsPresenter` [meetingParticipantInfo](../resources/meetingparticipantinfo.md). 

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
  "capabilities": [ "questionAndAnswer" ],
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String",
  "isBroadcast": "Boolean",
  "broadcastSettings": {"@odata.type": "microsoft.graph.broadcastSettings"}
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


