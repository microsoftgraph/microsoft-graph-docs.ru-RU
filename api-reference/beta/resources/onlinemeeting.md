---
title: Тип ресурса Онлинемитинг
description: Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cd3615f82a4e88d6dc0b07c12ba72e39726e755f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009358"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сбор сведений о собрании, в том числе URL-адреса присоединения, списка участников и описания.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Получение Онлинемитинг](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта Онлинемитинг. |

## <a name="properties"></a>Свойства

| Свойство                  | Тип                                                   | Описание                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | Уровень доступа, который управляет допуском собрания по сети. Возможные значения: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`. |
| АудиоконференЦинг         | [АудиоконференЦинг](audioconferencing.md)              | Представляет сведения о доступе к телефонии для Онлинемитинг. |
| Канцеледдатетиме          | DateTime                                               | Время, когда собрание было отменено. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | Чат, связанный с этим собранием. |
| Креатиондатетиме          | DateTime                                               | Время создания собрания. Только для чтения.
| endDateTime               | DateTime                                               | Время окончания собрания. |
| Ентрекситаннаунцемент     | Boolean                                                | Состояние объявления о присутствии для собрания по сети. Если объявления о присутствии включены, собрание по сети будет объявлять об именах участников, которые присоединяются к собранию с помощью звука. |
| expirationDateTime        | DateTime                                               | Дата и время, по истечении которого собрание по сети может быть удалено в формате UTC. День и время должны находиться в пределах одного года до и десяти лет после текущей даты и времени на сервере. |
| id                        | Строка                                                 | Идентификатор, связанный с собранием по сети. Используется в запросе GET HTTP в качестве идентификатора. Только для чтения. Создается сервером. |
| isCancelled               | Boolean                                                | Указывает, было ли собрание отменено. |
| Жоинурл                   | String                                                 | URL-адрес, используемый при присоединении собрания по сети из Интернета. |
| Митингтипе               | String                                                 | Возможные `meetNow`значения:, `scheduled`, `recurring`, `broadcast` (Примечание: [CREATE онлинемитинг](../api/application-post-onlinemeetings.md) поддерживает `meetNow`только). |
| participants              | [МитингпартиЦипантс](meetingparticipants.md)          | Участники, связанные с собранием по сети.  Сюда входят Организатор и участники. |
| startDateTime             | DateTime                                               | Время начала собрания. |
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