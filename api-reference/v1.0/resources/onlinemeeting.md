---
title: Тип ресурса onlineMeeting
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 8ded2e79f8a9a2004f2ffa412b6d42e3275556b8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516096"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

Пространство имен: microsoft.graph

Содержит сведения о собрании, включая URL-адрес собрания, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Создание объекта onlineMeeting](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Создание собрания в Интернете.                                                                                    |
| [Get onlineMeeting](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Ознакомьтесь с свойствами и отношениями **объекта onlineMeeting.**                                        |
| [обновление](../api/onlinemeeting-update.md).                           | [onlineMeeting](onlinemeeting.md) | Обновление свойств объекта **onlineMeeting.** |
| [Удаление onlineMeeting](../api/onlinemeeting-delete.md)             | Нет                              | Удаление **объекта onlineMeeting.**                                                                                    |
| [Создание или доступ к onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте **объект onlineMeeting** с пользовательским внешним ID. Если собрание уже существует, извлекай его свойства. |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | onlineMeetingPresenters                       | Указывает, кто может быть презентовщиком на собрании. Возможные значения перечислены в следующей таблице.                          |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | Сведения о доступе к телефону для собрания в Интернете. Только для чтения.                                                   |
| chatInfo              | [chatInfo](chatinfo.md)                       | Сведения о чате, связанные с этой онлайн-встречей.                                                                  |
| creationDateTime      | DateTime                                      | Время создания собрания в UTC. Только для чтения.                                                                               |
| endDateTime           | DateTime                                      | Время окончания собрания в UTC.                                                                                               |
| id                    | Строка                                        | ID по умолчанию, связанный с онлайн-собранием. Только для чтения.                                                              |
| isEntryExitAnnounced  | Логический                                       | Следует ли объявлять о том, когда звонители присоединяются или уходят.                                                                     |
| joinInformation       | [itemBody](itembody.md)                       | Сведения о присоединиться в варианте языка и языка, указанные в `Accept-Language` заглавной странице HTTP запроса. Только для чтения. |
| joinWebUrl            | Строка                                        | URL-адрес присоединиться к собранию в Интернете. Только для чтения.                                                                             |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Указывает, какие участники могут обойти вестибюль собрания.                                                               |
| participants          | [meetingParticipants](meetingparticipants.md) | Участники, связанные с онлайн-собранием.  Это включает организатора и участников.                       |
| startDateTime         | DateTime                                      | Время начала собрания в UTC.                                                                                             |
| subject               | String                                        | Тема собрания в Интернете.                                                                                         |
| videoTeleconferenceId | Строка                                        | ID видеоконференции. Только для чтения.                                                                                  |

### <a name="onlinemeetingpresenters-values"></a>значения onlineMeetingPresenters

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| все           | Каждый — это презентер (это параметр по умолчанию).             |
| organization;       | Каждый в организации организатора — это презентер.          |
| roleIsPresenter    | Только участники, роль которых является презентатором, являются участниками. |
| organizer          | Только организатор — это презентер.                           |
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

