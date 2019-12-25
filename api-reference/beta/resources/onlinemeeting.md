---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: e7cae71f220a2a519908e3af890029a2da555577
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866688"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Создание Онлинемитинг](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети. |
| [Получение Онлинемитинг](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **онлинемитинг** . |

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
