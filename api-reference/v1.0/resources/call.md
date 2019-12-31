---
title: Тип ресурса call
description: Ресурс **call** создается при наличии входящего вызова приложения или при создании приложением нового исходящего вызова с помощью запроса `POST` в `app/calls`.
author: ananmishr
localization_priority: Priority
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f97360875af2241df3d78108d9c7447bfa6b6975
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913473"
---
# <a name="call-resource-type"></a>Тип ресурса call

Ресурс **call** создается при наличии входящего вызова приложения или при создании приложением нового исходящего вызова с помощью запроса `POST` в `app/calls`.

Вызовы можно настраивать как одноранговые или групповые вызовы. Чтобы создать или присоединиться к групповому вызову, укажите `chatInfo` и `meetingInfo`. Если они не указаны, автоматически создается групповой вызов. Для входящих вызовов записывайте эти значения в высокодоступном хранилище, чтобы приложение повторно присоединилось к вызову в случае своего сбоя.

Хотя одно удостоверение нельзя пригласить несколько раз, приложение может присоединяться к одному собранию несколько раз. При каждой попытке приложения присоединиться должно предоставляться отдельное удостоверение, чтобы клиенты отображали их как отдельных участников.

> **Примечание.** URL-адрес для присоединения можно получить из собрания, запланированного с помощью Microsoft Teams. Извлеките данные из URL-адреса, как показано, чтобы заполнить свойства `chatInfo` и `meetingInfo`.
```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
```
преобразуется в:
```
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

## <a name="methods"></a>Методы

| Метод                                                             | Возвращаемый тип                                                 | Описание                                                                     |
|:-------------------------------------------------------------------|:------------------------------------------------------------|:--------------------------------------------------------------------------------|
| [получение](../api/call-get.md);                                     | [call](call.md)                                             | Чтение свойств объекта **call**.                                         |
| [Удаление](../api/call-delete.md)                                    | Нет                                                            | Удаление или разрыв активного **вызова**.                                           |
| [KeepAlive](../api/call-keepalive.md)                             | Нет                                                  | Проверка, что вызов остается активным.
| **Обработка вызовов**                                                  |                                                        |                                                                                 |
| [Ответ](../api/call-answer.md)                                    | Нет                                                            | Ответ на входящий вызов.                                                        |
| [Reject](../api/call-reject.md)                                    | Нет                                                            | Отклонение входящего вызова.                                                        |
| [Redirect](../api/call-redirect.md)                                | Нет                                                            | Перенаправление входящего вызова.                                                      |
| [Перевод](../api/call-transfer.md)                                | Нет                                                            | Переключение звонка                                                                 |
| **Групповые звонки**                                                    |                                                             |                                                                                 |
| [Перечисление участников](../api/call-list-participants.md)              | Коллекция [participant](participant.md)                    | Получение коллекции объектов.                                            |
| [Приглашение участников](../api/participant-invite.md)                | [commsOperation](commsoperation.md)                         | Приглашение участников в активный вызов.                                         |
| [Отключение звука участника](../api/participant-mute.md)                     | [muteParticipantOperation](muteparticipantoperation.md)     | Отключение звука участника в групповом вызове.                                           |
| **Интерактивный голосовой ответ**                                     |                                                             |                                                                                 |
| [PlayPrompt](../api/call-playprompt.md)                            | [playPromptOperation](playpromptoperation.md)               | Воспроизведение запроса в вызове.                                                        |
| [RecordResponse](../api/call-record.md)                            | [recordOperation](recordoperation.md)                       | Запись короткого голосового ответа звонящего.                                        |
| [SubscribeToTone](../api/call-subscribetotone.md)                  | [commsOperation](commsoperation.md)                         | Подписка на тоны DTMF.                                                        |
| **Самостоятельные операции участников**                                    |                                                             |                                                                                 |
| [Отключение звука](../api/call-mute.md)                                        | [muteParticipantOperation](muteparticipantoperation.md)     | Отключение своего звука в вызове.                                                          |
| [Включение звука](../api/call-unmute.md)                                    | [unmuteParticipantOperation](unmuteparticipantoperation.md) | Включение своего звука в звонке.                                                        |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md)  | Нет                                                        | Начало и прекращение демонстрации экрана в звонке.                                      |

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                                                                   | Описание                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| callbackUri         | String                                                                                                 | URL-адрес обратного вызова, на который направляются обратные вызовы. Должно быть задано значение `https`.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | Сведения о чате. Сведения, необходимые для присоединения к собранию.                                                                                                                              |
| direction           | String                                                                                                 | Направление вызова. Возможные значения: `incoming` или `outgoing`. Только для чтения.                                                                                            |
| id                  | String                                                                                                 | Идентификатор вызова. Только для чтения.                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) или [serviceHostedMediaConfig](servicehostedmediaconfig.md) | Настройка мультимедиа. Обязательно.                                                                        |
| mediaState          | [callMediaState](callmediastate.md)                                                                    | Только для чтения. Состояние мультимедиа компонентов вызова. |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) или [tokenMeetingInfo](tokenmeetinginfo.md)             | Сведения о собрании, необходимые для присоединения к собранию.                                                                                                            |
| myParticipantId     | String                                                                                                 | Только для чтения.                                                                                                                                                                        |
| requestedModalities | Коллекция String                                                                                      | Список запрошенных модальностей. | Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | Сведения о результате. Например, может содержать причину прекращения. Только для чтения.                                                                                                        |
| source              | [participantInfo](participantinfo.md)                                                                  | Создатель вызова.                                                                                                                                                                         |
| state               | String                                                                                                 | Состояние вызова. Возможные значения: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Только для чтения.                          |
| subject             | String                                                                                                 | Тема беседы.                                                                                                                                                                    |
| targets             | Коллекция [invitationParticipantInfo](participantinfo.md)                                             | Целевые объекты вызова. Обязательные сведения для создания одноранговых вызовов.                                                                                                            |
toneInfo            | [toneInfo](toneinfo.md)                                                                                | Только для чтения.                                                                                                                                                                        |

## <a name="relationships"></a>Отношения

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| operations          | Коллекция [commsOperation](commsoperation.md)       | Только для чтения. Допускается значение null.                                                |
| participants        | Коллекция [participant](participant.md)             | Только для чтения. Допускается значение null.                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatInfo",
    "direction",
    "id",
    "incomingContext",
    "mediaState",
    "meetingInfo",
    "myParticipantId",
    "replacesContext",
    "resultInfo",
    "state",
    "source",
    "subject",
    "targets",
    "toneInfo"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "mediaState": {"@odata.type": "#microsoft.graph.callMediaState"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "replacesContext": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
