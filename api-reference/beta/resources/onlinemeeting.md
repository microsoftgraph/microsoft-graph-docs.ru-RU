---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 7280fd64c5494897a8449e5894e8672af15b66f8
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635203"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о собрании, в том числе URL-адрес, используемый для присоединения к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                       |
| :----------------------------------------------------------------- | :-------------------------------- | :---------------------------------------------------------------------------------------------------------------- |
| [Создание](../api/application-post-onlineMeetings.md)                | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети.                                                                                         |
| [получение](../api/onlinemeeting-get.md);                                 | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **онлинемитинг** .                                             |
| [Создание или получение Онлинемитинг](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом. Если собрание уже существует, извлеките его свойства.      |
| [обновление](../api/onlinemeeting-update.md).                           | [onlineMeeting](onlinemeeting.md) | Обновление свойств **startDateTime**, **endDateTime**, **subject**и **участников** собрания по сети. |
| [удаление](../api/onlinemeeting-delete.md);                           | Нет                              | Удаление ресурса **онлинемитинг** .                                                                             |

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
| capabilities          | Коллекция String                             | Список возможностей собрания. Возможные значения: `questionAndAnswer` .                                                                                                                                                                                 |
| видеотелеконференцеид | String                                        | Идентификатор видеоконференций для видеоконференций. Только для чтения.                                                                                                                                                                                                                   |
| жоининформатион       | [itemBody](itembody.md)                       | Сведения о присоединении на языке и языковом варианте, указанным в HTTP-заголовке запроса Accept-Language. Только для чтения                                                                                                                                       |
| externalId            | String                                        | Внешний идентификатор. Настраиваемый идентификатор. Необязательный параметр.                                                                                                                                                                                                                     |
| исентрекситаннаунцед  | Логический                                       | Указывает, следует ли объявлять, когда звонящие присоединяются или оставляют.                                                                                                                                                                                                      |
| лоббибипасссеттингс   | [лоббибипасссеттингс](lobbyBypassSettings.md) | Указывает, какие участники могут обходить зал собрания.                                                                                                                                                                                                  |
| алловедпресентерс     | онлинемитингпресентерс                       | Указывает, кто может быть докладчиком на собрании. Возможные значения: `everyone` , `organization` , `roleIsPresenter` , `organizer` и `unknownFutureValue` .                                                                                                                                                                            |

> [!IMPORTANT]
> Свойство **аутоадмиттедусерс** является устаревшим. Вместо этого используйте **лоббибипасссеттингс. Scope** для конфигураций параметров собраний.

### <a name="onlinemeetingpresenters-values"></a>значения Онлинемитингпресентерс

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| просматривающи           | "Все" — докладчик (это параметр по умолчанию).             |
| organization;       | Все пользователи в Организации организатора — докладчик.          |
| ролеиспресентер    | Докладчиками являются только те участники, у которых есть роль докладчика. |
| organizer          | Только организатор является выступающим.                           |
| unknownFutureValue | Неизвестное будущее значение.                                          |

**Note**: Если для параметра **алловедпресентерс** задано значение `roleIsPresenter` , укажите роль собрания каждого участника собрания с помощью свойства **Role** в [митингпартиЦипантинфо](../resources/meetingparticipantinfo.md).

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


