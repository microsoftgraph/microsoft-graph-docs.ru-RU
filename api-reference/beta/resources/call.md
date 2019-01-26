---
title: Тип ресурса call
description: Ресурс **call** создается при наличии входящего вызова приложения или при создании приложением нового исходящего вызова с помощью запроса `POST` в `app/calls`.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: c66ab2f29ee44d76ed0ee300743f50cb0debdd16
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510717"
---
# <a name="call-resource-type"></a>Тип ресурса call

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **call** создается при наличии входящего вызова приложения или при создании приложением нового исходящего вызова с помощью запроса `POST` в `app/calls`.

Вызовы можно настраивать как одноранговые или многопользовательские вызовы. Чтобы создать или присоединиться к многопользовательскому вызову, укажите `chatInfo` и `meetingInfo`. Если они не указаны, автоматически создается незапланированное собрание. Для входящих вызовов записывайте эти значения в высокодоступном хранилище, чтобы приложение повторно присоединилось к вызову в случае своего сбоя.

Хотя одно удостоверение нельзя пригласить несколько раз, приложение может присоединяться к одному собранию несколько раз. При каждом присоединении приложения предусматривается отдельный вызов `id` для этого вызова собрания. Рекомендуется использовать отдельные удостоверения для присоединения к собранию, чтобы клиенты отображали их в виде отдельных участников.

## <a name="methods"></a>Методы

| Метод                                                            | Возвращаемый тип                                       | Описание                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Получение вызова](../api/call-get.md)                                    | [call](call.md)                                   | Чтение свойств объекта **call**.      |
| [Удаление](../api/call-delete.md)                                   |                                                   | Удаление или разрыв активного **вызова**.        |
| **Обработка вызовов**                                                 |                                                   |                                              |
| [Ответ](../api/call-answer.md)                                   |                                                   | Ответ на входящий вызов.                     |
| [Отклонение](../api/call-reject.md)                                   |                                                   | Отклонение входящего вызова.                     |
| [Перенаправление](../api/call-redirect.md)                               |                                                   | Перенаправление входящего вызова.                   |
| [Перевод](../api/call-transfer.md)                               |                                                   | Перевод вызова                              |
| **Многопользовательский**                                                   |                                                   |                                              |
| [Перечисление участников](../api/call-list-participants.md)             | Коллекция [participant](participant.md)          | Получение коллекции объектов.         |
| [Приглашение участников](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | Приглашение участников в активный вызов.      |
| [Отключение звука всех участников](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | Отключение звука всех участников вызова.           |
| [Настройка звукового микшера](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | Настройка звука в многопользовательской беседе.  |
| [Создание объекта audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | Создание нового объекта audioRoutingGroup путем публикации в коллекции audioRoutingGroups. |
| [Перечисление AudioRoutingGroups](../api/call-list-audioroutinggroups.md) | Коллекция [audioRoutingGroup](audioroutinggroup.md)|Получение коллекции объектов audioRoutingGroup.  |
| **Интерактивный голосовой ответ**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | Воспроизведение запроса в вызове.                     |
| [Запись](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | Запись вызова.                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | Отмена обработки мультимедиа.                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | Подписка на тоны DTMF.                     |
| **Самостоятельные операции участников**                                   |                                                   |                                              |
| [Отключение звука](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | Отключение своего звука в вызове.                       |
| [Включение звука](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | Включение своего звука в вызове.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | Обновление метаданных для себя в списке.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | Начало и прекращение предоставления общего доступа к экрану в вызове                                             |

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                                                                   | Описание                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | Коллекция String                                                                                      | Список активных модальностей. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`. Только для чтения. Создается сервером.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | Участник, ответивший на вызов. Только для чтения. Создается сервером.                                                                                                                                |
| callRoutes          | Коллекция [callRoute](callroute.md)                                                                   | Сведения маршрутизации о том, как был перенаправлен вызов. Только для чтения. Создается сервером.                                                                                                                |
| callbackUri         | String                                                                                                 | Идентификатор обратного вызова или подписки, для которой будут предоставляться обратные вызовы.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | Сведения о чате.                                                                                                                                                                               |
| direction           | String                                                                                                 | Направление вызова. Возможные значения: `incoming` или `outgoing`. Только для чтения. Создается сервером.                                                                                            |
| id                  | String                                                                                                 | Только для чтения. Создается сервером.                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) или [serviceHostedMediaConfig](servicehostedmediaconfig.md) | Настройка мультимедиа.                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Содержит возможности собрания.                                                                                                                                                             |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) или [tokenMeetingInfo](tokenmeetinginfo.md)             | Сведения о собрании.                                                                                                                                                                            |
| myParticipantId     | String                                                                                                 | Только для чтения. Создается сервером.                                                                                                                                                                        |
| requestedModalities | Коллекция String                                                                                      | Список запрошенных модальностей. | Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | Сведения о результате. Например, может содержать причину прекращения. Только для чтения. Создается сервером.                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | Время ожидания звонков для исходящих одноранговых вызовов                                                                                                                                                     |
| routingPolicies     | Коллекция String                                                                                      | Возможные значения: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`.                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | Создатель вызова.                                                                                                                                                                         |
| state               | String                                                                                                 | Состояние вызова. Возможные значения: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Только для чтения. Создается сервером.                         |
| subject             | String                                                                                                 | Тема беседы.                                                                                                                                                                    |
| targets             | Коллекция [participantInfo](participantinfo.md)                                                       | Целевые объекты вызова.                                                                                                                                                                            |
| tenantId            | String                                                                                                 | tenantId в Azure Active Directory.                                                                                                                                                                 |
| terminationReason   | String                                                                                                 | Только для чтения. Создается сервером.                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Только для чтения. Создается сервером.                                                                                                                                                                        |

> Примечание. Свойства, помеченные как `Server generated`, игнорируются при обработке запроса `POST` в `app/calls`.

## <a name="relationships"></a>Связи

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | Коллекция [audioRoutingGroup](audioroutinggroup.md) | Только для чтения. Допускается значение null.                                                |
| operations          | Коллекция [commsOperation](commsoperation.md)       | Только для чтения. Допускается значение null.                                                |
| participants        | Коллекция [participant](participant.md)             | Только для чтения. Допускается значение null.                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "activeModalities",
    "answeredBy",
    "callRoutes",
    "chatInfo",
    "direction",
    "id",
    "meetingCapability",
    "meetingInfo",
    "myParticipantId",
    "resultInfo",
    "ringingTimeoutInSeconds",
    "routingPolicies",
    "state",
    "targets",
    "tenantId",
    "terminationReason",
    "toneInfo"
  ],
  "@odata.type": "microsoft.graph.call"
}-->
```json
{
  "activeModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "answeredBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "callRoutes": [{"@odata.type": "#microsoft.graph.callRoute"}],
  "callbackUri": "String",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "direction": "incoming | outgoing",
  "id": "String (identifier)",
  "mediaConfig": {"@odata.type": "#microsoft.graph.mediaConfig"},
  "meetingCapability": {"@odata.type": "#microsoft.graph.meetingCapability"},
  "meetingInfo": {"@odata.type": "#microsoft.graph.meetingInfo"},
  "myParticipantId": "String",
  "requestedModalities": ["unknown | audio | video | videoBasedScreenSharing | data"],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "ringingTimeoutInSeconds": 1024,
  "routingPolicies": ["none | noMissedCall | disableForwardingExceptPhone | disableForwarding"],
  "source": {"@odata.type": "#microsoft.graph.participantInfo"},
  "state": "incoming | establishing | ringing | established | hold | transferring | transferAccepted | redirecting | terminating | terminated",
  "subject": "String",
  "targets": [{"@odata.type": "#microsoft.graph.participantInfo"}],
  "tenantId": "String",
  "terminationReason": "String",
  "toneInfo": {"@odata.type": "#microsoft.graph.toneInfo"}
}
```

> **Примечание.** URL-адрес для присоединения можно найти в собрании, запланированном с помощью Microsoft Teams. Ниже показано, как извлечь данные из URL-адреса и заполнить `chatInfo` и `meetingInfo`.

```http
https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%224b444206-207c-42f8-92a6-e332b41c88a2%22%7d
decodes to:
https://teams.microsoft.com/l/meetup-join/19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context={"Tid":"72f988bf-86f1-41af-91ab-2d7cd011db47","Oid":"4b444206-207c-42f8-92a6-e332b41c88a2"}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.call",
  truncated: true
}-->
```json
{
  "chatInfo": {
    "threadId": "19:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "id": "4b444206-207c-42f8-92a6-e332b41c88a2"
      }
    }
  }
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
  "suppressions": [
    "Error: /api-reference/beta/resources/call.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
