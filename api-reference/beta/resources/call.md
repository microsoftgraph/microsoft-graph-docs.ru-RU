---
title: Тип ресурса call
description: Ресурс **call** создается при наличии входящего вызова приложения или при создании приложением нового исходящего вызова с помощью запроса `POST` в `app/calls`.
author: ananmishr
ms.localizationpriority: high
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 67480d67339dbe331abaf71d4a722e8d8b698c55
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645475"
---
# <a name="call-resource-type"></a>Тип ресурса call

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **call** создается при наличии входящего вызова приложения или при создании приложением нового исходящего вызова с помощью запроса `POST` в `app/calls`.

Вызовы можно настраивать как одноранговые или групповые вызовы. Чтобы создать или присоединиться к групповому вызову, укажите `chatInfo` и `meetingInfo`. Если они не указаны, автоматически создается групповой вызов. Для входящих вызовов записывайте эти значения в высокодоступном хранилище, чтобы приложение повторно присоединилось к вызову в случае своего сбоя.

Хотя одно удостоверение нельзя пригласить несколько раз, приложение может присоединяться к одному собранию несколько раз. При каждой попытке приложения присоединиться должно предоставляться отдельное удостоверение, чтобы клиенты отображали их как отдельных участников.

> **Примечание.** URL-адрес для присоединения можно получить из собрания, запланированного с помощью Microsoft Teams. Извлеките данные из URL-адреса, как показано, чтобы заполнить свойства `chatInfo` и `meetingInfo`.

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
```
преобразуется в:
```http
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
| **Групповые звонки**                                                    |                                                             |                                                                            |
| [Перечисление участников](../api/call-list-participants.md)              | Коллекция [participant](participant.md)                    | Получение коллекции объектов.                                            |
| [Приглашение участников](../api/participant-invite.md)                | [commsOperation](commsoperation.md)                         | Приглашение участников в активный вызов.                                         |
| [Отключение звука всех участников](../api/participant-muteall.md)             | [commsOperation](commsoperation.md)                         | Отключение звука всех участников звонка.                                              |
| [Отключение звука участника](../api/participant-mute.md)                     | [muteParticipantOperation](muteparticipantoperation.md)     | Отключение звука участника в групповом вызове.                                           |
| [Настройка звукового микшера](../api/participant-configuremixer.md)      | [commsOperation](commsoperation.md)                         | Настройка звука в многопользовательской беседе.                                     |
| [Создание объекта audioRoutingGroup](../api/call-post-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md)                   | Создание нового объекта **audioRoutingGroup** путем публикации в коллекции audioRoutingGroups. |
| [Перечисление AudioRoutingGroups](../api/call-list-audioroutinggroups.md)  | Коллекция [audioRoutingGroup](audioroutinggroup.md)        | Получение коллекции объектов **audioRoutingGroup**.                                      |
| [Добавление представления "Большая галерея"](../api/call-addlargegalleryview.md)            | [addLargeGalleryViewOperation](addlargegalleryviewoperation.md)  | Добавление представления "Большая галерея" в вызов.                                      |
| **Интерактивный голосовой ответ**                                     |                                                             |                                                                                 |
| [PlayPrompt](../api/call-playprompt.md)                            | [playPromptOperation](playpromptoperation.md)               | Воспроизведение запроса в вызове.                                                        |
| [RecordResponse](../api/call-record.md)                            | [recordOperation](recordoperation.md)                       | Запись короткого голосового ответа звонящего.                                        |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)      | [commsOperation](commsoperation.md)                         | Отмена обработки мультимедиа.                                                        |
| [SubscribeToTone](../api/call-subscribetotone.md)                  | [commsOperation](commsoperation.md)                         | Подписка на тоны DTMF.                                                        |
| **Самостоятельные операции участников**                                    |                                                             |                                                                                 |
| [Отключение звука](../api/call-mute.md)                                        | [muteParticipantOperation](muteparticipantoperation.md)     | Отключение своего звука в вызове.                                                          |
| [Включение звука](../api/call-unmute.md)                                    | [unmuteParticipantOperation](unmuteparticipantoperation.md) | Включение своего звука в звонке.                                                        |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md)  | Нет                                                        | Начало и прекращение демонстрации экрана в звонке.                                      |
| **Запись операций**                                           |                                                             |                                              |
| [UpdateRecordingStatus](../api/call-updaterecordingstatus.md)      | [updateRecordingStatusOperation](updateRecordingStatusOperation.md)               | Обновление состояния записи.                      |
| **Операции ведения журнала**                                           |                                                             |                                              |
| [Запись в журнал данных о качестве устройств](../api/call-logteleconferencedevicequality.md)| [teleconferenceDeviceQuality](teleconferencedevicequality.md) | Запись в журнал данных о качестве устройств для видеоконференций.|

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                                                                   | Описание                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | Коллекция modality                                                                                      | Список активных модальностей. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`. Только для чтения.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | Участник, ответивший на вызов. Только для чтения.                                                                                                                                |
| callRoutes          | Коллекция [callRoute](callroute.md)                                                                   | Сведения маршрутизации о том, как был перенаправлен вызов. Только для чтения.                                                                                                                |
| callbackUri         | String                                                                                                 | URL-адрес обратного вызова, на который направляются обратные вызовы. Должно быть задано значение `https`.                                                                                                                               |
| callChainId         | String                                                                                                 | Уникальный идентификатор всех звонков участника конференции или уникальный идентификатор звонков двух участников в звонке P2P. Необходимо скопировать из `Microsoft.Graph.Call.CallChainId`. |
| callOptions            | [outgoingCallOptions](outgoingcalloptions.md)                                                         | Содержит необязательные функции для вызова.   |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | Сведения о чате. Обязательные сведения для сценариев собраний.                                                                                                                                |
| direction           | callDirection                                                                                                 | Направление вызова. Возможные значения: `incoming` или `outgoing`. Только для чтения.                                                                                            |
| id                  | String                                                                                                 | Идентификатор вызова. Только для чтения.                                                                                                                                                                        |
| incomingContext     | [incomingContext](incomingcontext.md)                                                                  | Контекст, связанный с входящим вызовом. Только для чтения. Создается сервером.                                                                                                                                |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) или [serviceHostedMediaConfig](servicehostedmediaconfig.md) | Конфигурация мультимедиа. Обязательные сведения для создания одноранговых вызовов или присоединения к собраниям.                                                                        |
| mediaState          | [callMediaState](callmediastate.md)                                                                    | Только для чтения. Состояние мультимедиа компонентов вызова. |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Содержит возможности собрания. Только для чтения.                                                                                                       |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md), [tokenMeetingInfo](tokenmeetinginfo.md) или [joinMeetingIdMeetingInfo](joinmeetingidmeetinginfo.md)            | Сведения о собрании. Обязательные сведения для сценариев собраний.                                                                                                              |
|transcription     | [callTranscriptionInfo](calltranscriptioninfo.md)                                                         | Сведения расшифровки для вызова. Только для чтения.                           |
myParticipantId     | String                                                                                                   | Только для чтения.                                                                                                                                                                        |
| requestedModalities | Коллекция modality                                                                                      | Список запрошенных модальностей. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | Сведения о результате. Например, может содержать причину прекращения. Только для чтения.                                                                                                        |
| ringingTimeoutInSeconds | Int32                                                                                              | Время ожидания звонков в секундах для исходящих одноранговых вызовов. Максимальное значение для этого атрибута составляет 115 секунд.                                                                                        |
| routingPolicies     | Коллекция routingPolicy                                                                                      | Это свойство применимо только к одноранговым вызовам. Возможные значения: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`, `preferSkypeForBusiness`, `unknownFutureValue`.                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | Создатель вызова.                                                                                                                                                                         |
| state               | callState                                                                                                 | Состояние вызова. Возможные значения: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Только для чтения.                          |
| subject             | String                                                                                                 | Тема беседы.                                                                                                                                                                    |
| targets             | Коллекция [invitationParticipantInfo](participantinfo.md)                                             | Целевые объекты вызова. Обязательные сведения для создания одноранговых вызовов.                                                                                                            |
| tenantId            | String                                                                                                 | Только для чтения. `tenantId` в Azure Active Directory.                                                                                                                        |
| terminationReason   | String                                                                                                 | Только для чтения.                                                                                                                                                                       |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Только для чтения.                                                                                                                                                                        |

## <a name="relationships"></a>Связи

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | Коллекция [audioRoutingGroup](audioroutinggroup.md) | Только для чтения. Допускается значение null.                                                |
| operations          | Коллекция [commsOperation](commsoperation.md)       | Только для чтения. Допускается значение null.                                                |
| participants        | Коллекция [participant](participant.md)             | Только для чтения. Допускается значение null.                                                |
| contentSharingSessions        | Коллекция [contentSharingSession](contentsharingsession.md)             | Только для чтения. Допускается значение null.                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "activeModalities",
    "answeredBy",
    "callRoutes",
    "callChainId",
    "callOptions",
    "chatInfo",
    "contentSharingSessions",
    "direction",
    "id",
    "incomingContext",
    "mediaState",
    "meetingCapability",
    "meetingInfo",
    "transcription",
    "myParticipantId",
    "replacesContext",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "source",
    "subject",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "activeModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "answeredBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "#microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "callChainId": "String",
  "callOptions": {"@odata.type": "#microsoft.graph.outgoingCallOptions"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "contentSharingSessions": [{ "@odata.type": "microsoft.graph.contentSharingSession" }],
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "incomingContext": {"@odata.type": "#microsoft.graph.incomingContext"},
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "mediaState": {"@odata.type": "#microsoft.graph.callMediaState"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "transcription": {"@odata.type": "#microsoft.graph.callTranscriptionInfo"},
  "myParticipantId": "String",
  "replacesContext": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding | preferSkypeForBusiness"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
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


