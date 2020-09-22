---
title: Тип ресурса Онлинемитинг
description: Содержит сведения о собрании, включая URL-адрес присоединения, список участников и описание.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 1b2a87d8494876ada8c45849d2cd93142f1dc570
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056494"
---
# <a name="onlinemeeting-resource-type"></a>Тип ресурса Онлинемитинг

Пространство имен: microsoft.graph

Содержит сведения о собрании, включая URL-адрес, используемый для присоединения к собранию, список участников и описание.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
| [Создание объекта onlineMeeting](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети. |
| [Получение Онлинемитинг](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Чтение свойств и связей объекта **онлинемитинг** . |
| [Удаление Онлинемитинг](../api/onlinemeeting-delete.md) | Нет | Удаление собрания по сети. |
| [Создание или получение Онлинемитинг](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Создайте собрание по сети с пользовательским внешним ИДЕНТИФИКАТОРом. Если собрание уже существует, извлеките его свойства. |

## <a name="properties"></a>Свойства

| Свойство                  | Тип                                                   | Описание                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| аудиоконференЦинг         | [аудиоконференЦинг](audioconferencing.md)              | Сведения о телефонном доступе (телефонное подключение) для собрания по сети. Только для чтения. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | Сведения о чате, связанные с этим собранием по сети. |
| креатиондатетиме          | DateTime                                               | Время создания собрания в формате UTC. Только для чтения. |
| startDateTime             | DateTime                                               | Время начала собрания в формате UTC. |
| endDateTime               | DateTime                                               | Время окончания собрания в формате UTC. |
| id                        | String                                                 | ИДЕНТИФИКАТОР по умолчанию, связанный с собранием по сети. Только для чтения. |
| жоинвебурл                | String                                                 | URL-адрес присоединения к собранию по сети. Только для чтения.|
| participants              | [митингпартиЦипантс](meetingparticipants.md)          | Участники, связанные с собранием по сети.  Сюда входят Организатор и участники. |
| subject                   | String                                                 | Тема собрания по сети. |
| видеотелеконференцеид     | String                                                 | Идентификатор видеоконференций для видеоконференций. Только для чтения. |
| жоининформатион | [itemBody](itembody.md) | Сведения о присоединении на языке и языковом варианте, указанном в `Accept-Language` HTTP-заголовке Request. Только для чтения. |

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

