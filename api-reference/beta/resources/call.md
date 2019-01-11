---
title: Тип ресурса звонка
description: При наличии входящего звонка для приложения или приложение создает новый исходящих вызовов с помощью создается ресурс **вызова** `POST` на `app/calls`.
author: VinodRavichandran
localization_priority: Priority
ms.openlocfilehash: d2748b410352effb7119a569bdf48c86f2f7c2ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810705"
---
# <a name="call-resource-type"></a>Тип ресурса звонка

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

При наличии входящего звонка для приложения или приложение создает новый исходящих вызовов с помощью создается ресурс **вызова** `POST` на `app/calls`.

Звонки можно настроить как peer-to-peer или многопользовательских звонков. Для создания или выполняется присоединение многопользовательских звонков, укажите `chatInfo` и `meetingInfo`. Если они не заданы, новое собрание специального создается автоматически. Для входящего звонка, запишите эти значения в банке высокой доступностью, чтобы приложение для повторного подключения вызова в случае сбоя приложения.

Несмотря на то, что же идентификатор не удается пригласить несколько раз, приложение может присоединиться к одной собраний несколько раз. Каждый раз, соединения приложения различных вызовов `id` предоставляется для этого вызова к собранию. Рекомендуется использовать разные удостоверения, чтобы присоединиться к собранию в порядке для клиентов, чтобы они отображаются как разные участников.

## <a name="methods"></a>Методы

| Метод                                                            | Возвращаемый тип                                       | Описание                                  |
|:------------------------------------------------------------------|:--------------------------------------------------|:---------------------------------------------|
| [Начало звонка](../api/call-get.md)                                    | [звонок](call.md)                                   | Чтение свойств объекта **вызова** .      |
| [удаление](../api/call-delete.md);                                   |                                                   | DELETE или сигнала отбоя активных **вызовов**.        |
| **Обработка звонков**                                                 |                                                   |                                              |
| [Ответ](../api/call-answer.md)                                   |                                                   | Ответ на входящий звонок.                     |
| [Reject](../api/call-reject.md)                                   |                                                   | Отклонение входящего звонка.                     |
| [Redirect](../api/call-redirect.md)                               |                                                   | Перенаправление входящего звонка.                   |
| [Transfer](../api/call-transfer.md)                               |                                                   | Переключение звонка                              |
| **Несколько производителей**                                                   |                                                   |                                              |
| [Список участников](../api/call-list-participants.md)             | [участник](participant.md) семейства сайтов          | Получите коллекцию объектов участников.         |
| [Приглашение участников](../api/participant-invite.md)               | [commsOperation](commsoperation.md)               | Приглашение участников активного вызова.      |
| [Отключение всех участников](../api/participant-muteall.md)            | [commsOperation](commsoperation.md)               | Отключение всех участников в вызове.           |
| [Настройка звукового микшера](../api/participant-configuremixer.md)     | [commsOperation](commsoperation.md)               | Настройка звука в многосторонней беседе.  |
| [Создание audioRoutingGroup](../api/call-post-audioroutinggroups.md)| [audioRoutingGroup](audioroutinggroup.md)         | Создайте новый audioRoutingGroup, отправку сообщений в коллекцию audioRoutingGroups. |
| [Список audioRoutingGroups](../api/call-list-audioroutinggroups.md) | [audioRoutingGroup](audioroutinggroup.md) коллекции|Получите коллекцию объектов audioRoutingGroup.  |
| **Интерактивного речевого взаимодействия**                                    |                                                   |                                              |
| [PlayPrompt](../api/call-playprompt.md)                           | [playPromptOperation](playpromptoperation.md)     | Воспроизведение приглашения в вызове.                     |
| [Record](../api/call-record.md)                                   | [recordOperation](recordoperation.md)             | Запишите вызова.                             |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md)     | [commsOperation](commsoperation.md)               | Отмена обработки мультимедиа.                     |
| [SubscribeToTone](../api/call-subscribetotone.md)                 | [commsOperation](commsoperation.md)               | Подпишитесь на тоновых сигналов DTMF.                     |
| **Собственный участников операций**                                   |                                                   |                                              |
| [Отключить звук](../api/call-mute.md)                                       | [commsOperation](commsoperation.md)               | Отключить звук self в вызове.                       |
| [Включение звука](../api/call-unmute.md)                                   | [commsOperation](commsoperation.md)               | Включение звука self в вызове.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | [commsOperation](commsoperation.md)               | Обновление метаданных для самообслуживания в списке.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) |                                                   | Запуск и остановка совместного использования экрана в вызове                                             |

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                                                                   | Описание                                                                                                                                                                                         |
| :------------------ | :------------------------------------------------------------------------------------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| activeModalities    | Коллекция строк                                                                                      | Список активных модальности. Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`. Только для чтения. Сервер, созданный.                                                    |
| answeredBy          | [participantInfo](participantinfo.md)                                                                  | Участник, ответить на звонок. Только для чтения. Сервер, созданный.                                                                                                                                |
| callRoutes          | [callRoute](callroute.md) коллекции                                                                   | Сведения о маршрутизации на как была перенаправлена вызова. Только для чтения. Сервер, созданный.                                                                                                                |
| callbackUri         | Строка                                                                                                 | Идентификатор обратного вызова или подписки, на котором будет доставлено обратных вызовов.                                                                                                                               |
| chatInfo            | [chatInfo](chatinfo.md)                                                                                | Сведения о чата.                                                                                                                                                                               |
| Направление           | Строка                                                                                                 | Направление вызова. Возможное значение — `incoming` или `outgoing`. Только для чтения. Сервер, созданный.                                                                                            |
| id                  | Строка                                                                                                 | Только для чтения. Сервер, созданный.                                                                                                                                                                        |
| mediaConfig         | [appHostedMediaConfig](apphostedmediaconfig.md) или [serviceHostedMediaConfig](servicehostedmediaconfig.md) | Конфигурация мультимедиа.                                                                                                                                                                        |
| meetingCapability   | [meetingCapability](meetingcapability.md)                                                              | Содержит возможности собрания.                                                                                                                                                             |
| meetingInfo         | [organizerMeetingInfo](organizermeetinginfo.md) или [tokenMeetingInfo](tokenmeetinginfo.md)             | Сведения о собрании.                                                                                                                                                                            |
| myParticipantId     | Строка                                                                                                 | Только для чтения. Сервер, созданный.                                                                                                                                                                        |
| requestedModalities | Коллекция String                                                                                      | Список запрошенные модальности. | Возможные значения: `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.                                                                            |
| resultInfo          | [resultInfo](resultinfo.md)                                                                            | Сведения о результатов. Например может содержать причину завершения. Только для чтения. Сервер, созданный.                                                                                                       |
| ringingTimeoutInSeconds | Int32                                                                                              | Время ожидания для исходящих звонков для одноранговых звонков                                                                                                                                                     |
| routingPolicies     | Коллекция String                                                                                      | Возможные значения: `none`, `noMissedCall`, `disableForwardingExceptPhone`, `disableForwarding`.                                                                                                   |
| source              | [participantInfo](participantinfo.md)                                                                  | Инициатор вызова.                                                                                                                                                                         |
| state               | Строка                                                                                                 | Состоянии вызова. Возможные значения: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`. Только для чтения. Сервер, созданный.                         |
| subject             | Строка                                                                                                 | Тема беседы.                                                                                                                                                                    |
| целевые значения             | [participantInfo](participantinfo.md) коллекции                                                       | Целевые значения вызова.                                                                                                                                                                            |
| tenantId            | Строка                                                                                                 | tenantId в Azure Active Directory.                                                                                                                                                                 |
| terminationReason   | Строка                                                                                                 | Только для чтения. Сервер, созданный.                                                                                                                                                                        |
| toneInfo            | [toneInfo](toneinfo.md)                                                                                | Только для чтения. Сервер, созданный.                                                                                                                                                                        |

> Примечание: Свойства помечены как `Server generated` игнорируются при обработке `POST` на `app/calls`.

## <a name="relationships"></a>Связи

| Связь        | Тип                                                 | Описание                                                         |
|:--------------------|:-----------------------------------------------------|:--------------------------------------------------------------------|
| audioRoutingGroups  | [audioRoutingGroup](audioroutinggroup.md) коллекции | Только для чтения. Допускается значение null.                                                |
| operations          | [commsOperation](commsoperation.md) коллекции       | Только для чтения. Допускается значение null.                                                |
| participants        | [участник](participant.md) семейства сайтов             | Только для чтения. Допускается значение null.                                                |

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

> **Примечание:** Вы найдете присоединения к URL-адрес из собрания, запланированные с группами Майкрософт. Порядок извлечения данных из URL-адреса и заливки `chatInfo` и `meetingInfo`.

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
<!-- {
  "type": "#page.annotation",
  "description": "call resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
