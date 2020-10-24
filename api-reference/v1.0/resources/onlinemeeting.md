---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 9f986bf0bd7871185673759a6e98e80d5d10b4b7
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741931"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

Пространство имен: microsoft.graph

Содержит сведения о собрании, в том числе URL-адрес, используемый для присоединения к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                       | Описание                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Создание объекта onlineMeeting](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети.                                                                                    |
| [Получение Онлинемитинг](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **онлинемитинг** .                                        |
| [Удаление Онлинемитинг](../api/onlinemeeting-delete.md)             | Нет                              | Удаление собрания по сети.                                                                                    |
| [Создание или получение Онлинемитинг](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом. Если собрание уже существует, извлеките его свойства. |

## <a name="properties"></a>Свойства

| Свойство              | Тип                                          | Описание                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| аудиоконференЦинг     | [аудиоконференЦинг](audioconferencing.md)     | Сведения о телефонном доступе (телефонное подключение) для собрания по сети. Только для чтения.                                                   |
| chatInfo              | [chatInfo](chatinfo.md)                       | Сведения о чате, связанные с этим собранием по сети.                                                                  |
| креатиондатетиме      | DateTime                                      | Время создания собрания в формате UTC. Только для чтения.                                                                               |
| startDateTime         | DateTime                                      | Время начала собрания в формате UTC.                                                                                             |
| endDateTime           | DateTime                                      | Время окончания собрания в формате UTC.                                                                                               |
| id                    | String                                        | ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети. Только для чтения.                                                              |
| жоинвебурл            | String                                        | URL-адрес присоединения к собранию по сети. Только для чтения.                                                                             |
| participants          | [митингпартиЦипантс](meetingparticipants.md) | Участники, связанные с собранием по сети.  Сюда входят Организатор и участники.                       |
| subject               | String                                        | Тема собрания по сети.                                                                                         |
| видеотелеконференцеид | String                                        | Идентификатор видеоконференций для видеоконференций. Только для чтения.                                                                                  |
| жоининформатион       | [itemBody](itembody.md)                       | Сведения о присоединении на языке и языковом варианте, указанном в `Accept-Language` HTTP-заголовке Request. Только для чтения. |
| исентрекситаннаунцед  | Логический                                       | Указывает, следует ли объявлять, когда звонящие присоединяются или оставляют.                                                                     |
| лоббибипасссеттингс   | [лоббибипасссеттингс](lobbyBypassSettings.md) | Указывает, какие участники могут обходить зал собрания.                                                                 |
| алловедпресентерс     | онлинемитингпресентерс                       | Указывает, кто может быть докладчиком на собрании. Возможные значения перечислены в следующей таблице.                                           |

### <a name="onlinemeetingpresenters-values"></a>значения Онлинемитингпресентерс

| Значение              | Описание                                                   |
| ------------------ | ------------------------------------------------------------- |
| просматривающи           | "Все" — докладчик (это параметр по умолчанию).             |
| organization;       | Все пользователи в Организации организатора — докладчик.          |
| ролеиспресентер    | Докладчиками являются только те участники, у которых есть роль докладчика. |
| organizer          | Только организатор является выступающим.                           |
| unknownFutureValue | Неизвестное будущее значение.                                          |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

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

