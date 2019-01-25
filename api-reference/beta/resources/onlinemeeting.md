---
title: Тип ресурса onlineMeeting
description: Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519600"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса onlineMeeting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сбор сведений о собрании, включая присоединения к URL-адрес, в список участников и описание.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Получение onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойства и связи объекта onlineMeeting. |

## <a name="properties"></a>Свойства

| Свойство                  | Тип                                                   | Описание                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| AccessLevel               | String                                                 | Уровень доступа, который управляет допуска на собрание по сети. Возможные значения: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`. |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | Представляет телефона данные для доступа к onlineMeeting. |
| canceledDateTime          | DateTime                                               | Время, когда приглашение на собрание было отменено. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | Chat, связанного с этого собрания. |
| creationDateTime          | DateTime                                               | Время создания собрания. Только для чтения.
| endDateTime               | DateTime                                               | Время окончания собрания. |
| entryExitAnnouncement     | Логическое                                                | Состояние присутствия объявлений для собрания по сети. При включении извещения присутствия собрание по сети объявлять имена participantswho join в собрании по аудио. |
| expirationDateTime        | DateTime                                               | Абсолютный по Гринвичу (UTC) даты и времени, после которого можно удалить собрание по сети. Даты и времени должны быть от одного года до до десять лет после текущей датой и временем на сервере. |
| id                        | String                                                 | Идентификатор, связанный с собрания по сети. Используется в начало HTTP-запросов в качестве идентификатора. Только для чтения. Сервер, созданный. |
| isCancelled               | Boolean                                                | Приглашение на собрание была ли отменена. |
| joinUrl                   | String                                                 | URL-адрес, используемый при собрание по сети, связанное с веб. |
| meetingType               | String                                                 | Возможные значения: `meetNow`, `scheduled`, `recurring`. |
| participants              | [meetingParticipants](meetingparticipants.md)          | Участники, связанные с собрания по сети.  Сюда входят Организатор и участники. |
| startDateTime             | DateTime                                               | Запустите время собрания. |
| subject                   | String                                                 | Тема собрания по сети. |

## <a name="relationships"></a>Отношения
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
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
