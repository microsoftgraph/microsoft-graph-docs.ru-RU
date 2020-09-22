---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 4da898d8db37c1bb51380609aa90d88a4b8cf5da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052665"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, в том числе URL-адрес, используемый для присоединения к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                       |
| :----------------------------------------------------------------- | :-------------------------------- | :---------------------------------------------------------------------------------------------------------------- |
| [Создание](../api/application-post-onlineMeetings.md)                | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети.                                                                                         |
| [Получение](../api/onlinemeeting-get.md)                                 | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **онлинемитинг** .                                             |
| [Создание или получение Онлинемитинг](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом. Если собрание уже существует, извлеките его свойства.      |
| [Обновление](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | Обновление свойств **startDateTime**, **endDateTime**, **subject**и **участников** собрания по сети. |
| [Удаление](../api/onlinemeeting-delete.md)                           | Нет                              | Удаление ресурса **онлинемитинг** .                                                                             |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание                                                                                                                                                                                                                                                 |
| :-------------------- | :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| аутоадмиттедусерс     | String                                        | Параметр, указывающий тип участников, которые будут автоматически разрешены в собрании по сети. Возможные значения: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Только для чтения. |
| аудиоконференЦинг     | [аудиоконференЦинг](audioconferencing.md)     | Сведения о телефонном доступе (телефонное подключение) для собрания по сети. Только для чтения.                                                                                                                                                                                    |
| chatInfo              | [chatInfo](chatinfo.md)                       | Сведения о чате, связанные с этим собранием по сети.                                                                                                                                                                                                   |
| креатиондатетиме      | DateTime                                      | Время создания собрания в формате UTC. Только для чтения.                                                                                                                                                                                                                |
| startDateTime         | DateTime                                      | Время начала собрания в формате UTC.                                                                                                                                                                                                                              |
| endDateTime           | DateTime                                      | Время окончания собрания в формате UTC.                                                                                                                                                                                                                                |
| id                    | String                                        | ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети. Только для чтения.                                                                                                                                                                                               |
| жоинвебурл            | String                                        | URL-адрес присоединения к собранию по сети. Только для чтения.                                                                                                                                                                                                              |
| participants          | [митингпартиЦипантс](meetingparticipants.md) | Участники, связанные с собранием по сети.  Сюда входят Организатор и участники.                                                                                                                                                        |
| subject               | String                                        | Тема собрания по сети.                                                                                                                                                                                                                          |
| capabilities          | Коллекция объектов string                             | Список возможностей собрания. Возможные значения: `questionAndAnswer` .                                                                                                                                                                                 |
| видеотелеконференцеид | String                                        | Идентификатор видеоконференций для видеоконференций. Только для чтения.                                                                                                                                                                                                                   |
| жоининформатион       | [itemBody](itembody.md)                       | Сведения о присоединении на языке и языковом варианте, указанным в HTTP-заголовке запроса Accept-Language. Только для чтения                                                                                                                                       |
| externalId            | String                                        | Внешний идентификатор. Настраиваемый идентификатор. Необязательное свойство.                                                                                                                                                                                                                     |
| исентрекситаннаунцед  | Boolean                                       | Указывает, следует ли объявлять, когда звонящие присоединяются или оставляют.                                                                                                                                                                                                      |
| лоббибипасссеттингс   | [лоббибипасссеттингс](lobbyBypassSettings.md) | Указывает, какие участники могут обходить зал собрания.                                                                                                                                                                                                  |
| алловедпресентерс     | онлинемитингпресентерс                       | Указывает, кто может быть докладчиком на собрании. Возможные значения перечислены ниже.                                                                                                                                                                            |

> [!IMPORTANT]
> Свойство **аутоадмиттедусерс** является устаревшим. Вместо этого используйте **лоббибипасссеттингс. Scope** для конфигураций параметров собраний.

### <a name="onlinemeetingpresenters-values"></a>значения Онлинемитингпресентерс

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| просматривающи           | "Все" — докладчик (это параметр по умолчанию).             |
| organization       | Все пользователи в Организации организатора — докладчик.          |
| ролеиспресентер    | Докладчиками являются только те участники, у которых есть роль докладчика. |
| organizer          | Только организатор является выступающим.                           |
| unknownFutureValue | Неизвестное будущее значение.                                          |

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
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "everyone | organization | roleIsPresenter | organizer | unknownFutureValue"
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


