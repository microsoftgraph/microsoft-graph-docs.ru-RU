---
title: Тип ресурса Онлинемитинг
description: Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-cloud communications
doc_type: resourcePageType
ms.openlocfilehash: 5cc62c4caa564aa071ffc6b206d5494814b0cb53
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969803"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Создание Онлинемитинг](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети. |
| [Получение Онлинемитинг](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **онлинемитинг** . |

## <a name="properties"></a>Свойства

| Свойство                  | Тип                                                   | Описание                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| аутоадмиттедусерс         | String                                                 | Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети. Только для чтения. `everyone`Возможные значения: `everyoneInSameAndFederatedCompany`,, `everyoneInCompany`,, `invitedUsersInCompany``organizer`|
| аудиоконференЦинг         | [аудиоконференЦинг](audioconferencing.md)              | Сведения о телефонном доступе (телефонное подключение) для собрания по сети. Только для чтения. |
| канцеледдатетиме          | DateTime                                               | Время в формате UTC, когда собрание было отменено. Только для чтения. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | Сведения о чате, связанные с этим собранием по сети. |
| креатиондатетиме          | DateTime                                               | Время создания собрания в формате UTC. Только для чтения. |
| startDateTime             | DateTime                                               | Время начала собрания в формате UTC. |
| endDateTime               | DateTime                                               | Время окончания собрания в формате UTC. |
| id                        | Строка                                                 | ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети. Только для чтения. |
| Отменено                | Логический                                                | Указывает, было ли собрание отменено. Только для чтения. |
| жоинурл                   | String                                                 | URL-адрес присоединения к собранию по сети. Только для чтения.|
| Передача               | Логический                                                | Флаг, определяющий, является ли собрание широковещательным. |
| participants              | [митингпартиЦипантс](meetingparticipants.md)          | Участники, связанные с собранием по сети.  Сюда входят Организатор и участники. |
| subject                   | String                                                 | Тема собрания по сети. |
| capabilities              | Коллекция String                                      | Список возможностей собрания. Возможные значения: `questionAndAnswer`. |
| видеотелеконференцеид     | String                                                 | Идентификатор телеконференций видеио. Только для чтения. |

### <a name="autoadmittedusers-values"></a>значения Аутоадмиттедусерс
| Значение | Описание  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| organizer | Только организатор собрания додается непосредственно.  Все остальные ожидают, пока организатор не выйдет в "зале ожидания".  |
| инвитедусерсинкомпани | Организатор собрания и пользователи в той же компании, приглашенные организатором, напрямую присоединяются к собранию.  Все остальные ожидают, пока не станет допущен.  |
| еверйонеинкомпани | Все пользователи в той же организации, что и организатор, напрямую присоединяются к собранию. Федеративные анонимные пользователи ожидают, пока не допустить ожидания.  |
| еверйонеинсамеандфедератедкомпани |  Все пользователи в той же организации, что и организатор и Федеративные компании, присоединяются к собранию напрямую.  Анонимные пользователи ждут ожидания в зале ожидания.  |
| просматривающи | Разрешен любой пользователь. Все пользователи (включая анонимных пользователей) могут присоединяться к собранию напрямую, не дожидаясь ожидания в "зале ожидания".  |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

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
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCanceled": false,
  "joinUrl": "String",
  "isBroadcast": false,
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
