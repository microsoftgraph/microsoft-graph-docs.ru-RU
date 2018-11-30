---
title: Тип ресурса onlineMeeting
description: Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.
ms.openlocfilehash: 73e45f7f2c04df469f2c2fb0faf1c8a0f8680a64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075753"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Получение onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойства и связи объекта onlineMeeting. |

## <a name="properties"></a>Свойства

| Свойство                  | Тип                                                   | Description                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | Уровень доступа, который управляет допуска на собрание по сети. Возможные значения: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`. |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | Представляет телефона данные для доступа к onlineMeeting. |
| canceledDateTime          | DateTime                                               | Время, когда приглашение на собрание было отменено. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | Chat, связанного с этого собрания. |
| creationDateTime          | DateTime                                               | Время создания собрания. Только для чтения.
| endDateTime               | DateTime                                               | Время окончания собрания. |
| entryExitAnnouncement     | Логический                                                | Состояние присутствия объявлений для собрания по сети. При включении извещения присутствия собрание по сети объявлять имена participantswho join в собрании по аудио. |
| expirationDateTime        | DateTime                                               | Абсолютный по Гринвичу (UTC) даты и времени, после которого можно удалить собрание по сети. Даты и времени должны быть от одного года до до десять лет после текущей датой и временем на сервере. |
| id                        | String                                                 | Идентификатор, связанный с собрания по сети. Используется в начало HTTP-запросов в качестве идентификатора. Только для чтения. Сервер, созданный. |
| isCancelled               | Boolean                                                | Приглашение на собрание была ли отменена. |
| joinUrl                   | String                                                 | URL-адрес, используемый при собрание по сети, связанное с веб. |
| meetingType               | String                                                 | Возможные значения: `meetNow`, `scheduled`, `recurring`,`broadcast` |
| participants              | [meetingParticipants](meetingparticipants.md)          | Участники, связанные с собрания по сети.  Сюда входят Организатор и участники. |
| startDateTime             | DateTime                                               | Запустите время собрания. |
| subject                   | String                                                 | Тема собрания по сети. |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
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
