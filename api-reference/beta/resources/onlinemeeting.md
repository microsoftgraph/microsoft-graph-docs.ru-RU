---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 888b5d7d60a72ed95cb3e3f6cbb1b6e5407919ab
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962368"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Создание объекта onlineMeeting](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети. |
| [Получение Онлинемитинг](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **онлинемитинг** . |
| [Создание или получение Онлинемитинг](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом. Если собрание уже существует, извлеките его значение. |

## <a name="properties"></a>Свойства

| Свойство                  | Тип                                                   | Описание                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| аутоадмиттедусерс         | String                                                 | Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети. Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Только для чтения.|
| аудиоконференЦинг         | [аудиоконференЦинг](audioconferencing.md)              | Сведения о телефонном доступе (телефонное подключение) для собрания по сети. Только для чтения. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | Сведения о чате, связанные с этим собранием по сети. |
| креатиондатетиме          | DateTime                                               | Время создания собрания в формате UTC. Только для чтения. |
| startDateTime             | DateTime                                               | Время начала собрания в формате UTC. |
| endDateTime               | DateTime                                               | Время окончания собрания в формате UTC. |
| id                        | Строка                                                 | ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети. Только для чтения. |
| жоинвебурл                   | String                                                 | URL-адрес присоединения к собранию по сети. Только для чтения.|
| participants              | [митингпартиЦипантс](meetingparticipants.md)          | Участники, связанные с собранием по сети.  Сюда входят Организатор и участники. |
| subject                   | String                                                 | Тема собрания по сети. |
| capabilities              | Коллекция строк                                      | Список возможностей собрания. Возможные значения: `questionAndAnswer`. |
| видеотелеконференцеид     | String                                                 | Идентификатор видеоконференций для видеоконференций. Только для чтения. |
| externalId                | String                                                 | Внешний идентификатор. Настраиваемый идентификатор. Необязательный параметр. |

### <a name="autoadmittedusers-values"></a>значения Аутоадмиттедусерс
| Значение | Описание  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| organizer | Только организатор собрания додается непосредственно.  Все остальные ожидают, пока организатор не выйдет.  |
| инвитедусерсинкомпани | Организатор собрания и пользователи в той же компании, приглашенные организатором, напрямую присоединяются к собранию.  Все остальные ожидают, пока не станет допущен.  |
| еверйонеинкомпани | Все пользователи в той же организации, что и организатор, напрямую присоединяются к собранию.  Федеративные анонимные пользователи ожидают, пока не допустить ожидания.  |
| еверйонеинсамеандфедератедкомпани |  Все пользователи в той же организации, что и организатор и Федеративные компании, присоединяются к собранию напрямую.  Анонимные пользователи ждут ожидания в зале ожидания.  |
| просматривающи | Разрешен любой пользователь, что означает, что все пользователи (включая анонимных пользователей) могут присоединиться к собранию напрямую, не дожидаясь ожидания в "зале ожидания".  |


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
  "autoAdmittedUsers": "everyone | everyoneInSameAndFederatedCompany | everyoneInCompany | invitedUsersInCompany | organizer",
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
