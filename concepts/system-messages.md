---
title: Получение системных сообщений для Microsoft Teams с помощью API Microsoft Graph
description: Узнайте, как Microsoft Teams создает системные сообщения для событий с помощью API Microsoft Graph.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 44c5004388c848398bc3e7e83d2c63a1644886c9
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535545"
---
# <a name="get-system-messages-for-microsoft-teams-using-microsoft-graph-apis"></a>Получение системных сообщений для Microsoft Teams с помощью API Microsoft Graph

Microsoft Teams создает системные сообщения для событий, таких как добавление участников в чат, обновление имени команды и обновление описания канала. Системные сообщения позволяют звонящему получить аналитику событий, произошедших в команде, канале или чате.


Microsoft Graph предоставляет системные сообщения в рамках операций GET [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true) и [уведомлений об изменениях для чата и сообщений канала](teams-changenotifications-chatmessage.md).


Системные сообщения представлены как объекты [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true).
В этом случае для свойства **messageType** задается значение `systemEventMessage`, а свойство **eventDetail** предоставляет сведения о событии.


## <a name="supported-get-operations"></a>Поддерживаемые операции GET

Следующие операции GET поддерживают системные сообщения:

- GET /teams/{team-id}/channel/{channel-id}/messages
- GET /teams/{team-td}/channel/{channel-id}/messages/{message-id}
- GET /chats/{chat-id}/messages
- GET /chats/{chat-id}/messages/{message-id}

Дополнительные сведения см. в статье [chatMessage](/graph/api/resources/chatMessage?view=graph-rest-beta&preserve-view=true).

## <a name="supported-change-notifications"></a>Поддерживаемые уведомления об изменениях

Следующие уведомления об изменениях поддерживают системные сообщения:

- Подписка на сообщения в канале — /teams/{team-id}/channels/{channel-id}/messages
- Подписка на сообщения в чате — /chats/{chat-id}/messages

Дополнительные сведения см. в статье [Изменение уведомлений о сообщениях](teams-changenotifications-chatmessage.md).


## <a name="supported-system-message-events"></a>Поддерживаемые события системных сообщений

| Событие   |  Тип системного сообщения   | Применимо к |
|:--------|:--------------|:--------------|
| Звонок завершен | [callEndedEventMessageDetail](#call-ended) | Чат, канал |
| Запись звонка | [callRecordingEventMessageDetail](#call-recording) | Чат, канал |
| Звонок начат | [callStartedEventMessageDetail](#call-started) | Чат, канал |
| Расшифровка звонка | [callTranscriptEventMessageDetail](#call-transcript) | Чат, канал |
| Канал добавлен | [channelAddedEventMessageDetail](#channel-added) | Команда |
| Канал удален | [channelDeletedEventMessageDetail](#channel-deleted) | Команда |
| Описание канала обновлено | [channelDescriptionUpdatedEventMessageDetail](#channel-description-updated) | Канал |
| Канал переименован | [channelRenamedEventMessageDetail](#channel-renamed) | Канал |
| Канал назначен избранным | [channelSetAsFavoriteByDefaultEventMessageDetail](#channel-set-as-favorite-by-default) | Канал |
| Отменено назначение канала избранным | [channelUnsetAsFavoriteByDefaultEventMessageDetail](#channel-unset-as-favorite-by-default) | Канал |
| Чат переименован | [chatRenamedEventMessageDetail](#chat-renamed) | Чат |
| Роль участника беседы обновлена | [conversationMemberRoleUpdatedEventMessageDetail](#conversation-member-role-updated) | Канал, команда |
| Политика собраний обновлена | [meetingPolicyUpdatedEventMessageDetail](#meeting-policy-updated) | Чат |
| Участники добавлены | [membersAddedEventMessageDetail](#members-added) | Чат, канал, команда |
| Участники удалены | [membersDeletedEventMessageDetail](#members-deleted) | Чат, канал, команда |
| Участники присоединены | [membersJoinedEventMessageDetail](#members-joined) | Чат |
| Участники вышли | [membersLeftEventMessageDetail](#members-left) | Чат |
| Вкладка обновлена | [tabUpdatedEventMessageDetail](#tab-updated) | Чат, канал |
| Команда архивирована | [teamArchivedEventMessageDetail](#team-archived) | Команда |
| Команда создана | [teamCreatedEventMessageDetail](#team-created) | Команда |
| Описание команды обновлено | [teamDescriptionUpdatedEventMessageDetail](#team-description-updated) | Команда |
| Присоединение команды отключено | [teamJoiningDisabledEventMessageDetail](#team-joining-disabled) | Команда |
| Присоединение команды включено | [teamJoiningEnabledEventMessageDetail](#team-joining-enabled) | Команда |
| Команда переименована | [teamRenamedEventMessageDetail](#team-renamed) | Команда |
| Приложение Teams установлено | [teamsAppInstalledEventMessageDetail](#teams-app-installed) | Чат, канал, команда |
| Приложение Teams удалено | [teamsAppRemovedEventMessageDetail](#teams-app-removed) | Чат, канал, команда |
| Приложение Teams обновлено | [teamsAppUpgradedEventMessageDetail](#teams-app-upgraded) | Чат, канал, команда |
| Архивация команды отменена | [teamUnarchivedEventMessageDetail](#team-unarchived) | Команда |


> **Примечание.** Системные сообщения, применимые к команде, публикуются в основном канале.


## <a name="json-response-examples"></a>Примеры ответа JSON

В следующих примерах JSON представлены ответы для каждого поддерживаемого типа события.

### <a name="call-ended"></a>Звонок завершен

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callEndedEventMessageDetail",
    "callId": "9c848c0e-f906-4dfc-b22e-c68a785a587c",
    "callDuration": "PT59S",
    "callEventType": "meeting",
    "callParticipants": [{
      "participant": {
        "application": null,
        "device": null,
        "user": {
          "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
          "displayName": "Adele Vance ",
          "userIdentityType": "aadUser"
        }
      }
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-recording"></a>Запись звонка

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callRecordingEventMessageDetail",
    "callId": "c86c6052-410b-4e7c-b843-9a09f576e4d5",
    "callRecordingDisplayName": "Meeting Recording.mp4",
    "callRecordingUrl": "https://testtenant.sharepoint.com/sites/TestTeam/Shared%20Documents/General/Recordings/Meeting%20Recording.mp4?web=1",
    "callRecordingDuration": "PT40M19.26S",
    "callRecordingStatus": "success",
    "meetingOrganizer": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    },
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-started"></a>Звонок начат

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callStartedEventMessageDetail",
    "callId": "9c848c0e-f906-4dfc-b22e-c68a785a587c",
    "callEventType": "call",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="call-transcript"></a>Расшифровка звонка

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.callTranscriptEventMessageDetail",
    "callId": "5b927778-760b-429e-8c4e-65b1802dd6c9",
    "callTranscriptICalUid": "040000008200E00074C5B7101A82E00800000000002C743F89CDD601000000000000000010000000CA87F90D9372ED45A399B5D75E854EE9 ",
    "meetingOrganizer": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-added"></a>Канал добавлен

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelAddedEventMessageDetail",
    "channelId": "19:e84f079882f44fa8bebb7343b9e8921a@thread.tacv2",
    "channelDisplayName": "Standard channel",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-deleted"></a>Канал удален

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelDeletedEventMessageDetail",
    "channelId": "19:914b8c83915548c0bff588e510a6cf01@thread.tacv2",
    "channelDisplayName": "Standard channel",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-description-updated"></a>Описание канала обновлено

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "channelDescription": "Channel description updated",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-renamed"></a>Канал переименован

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "channelDisplayName": "Standard channel rename",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-set-as-favorite-by-default"></a>Канал назначен избранным по умолчанию

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="channel-unset-as-favorite-by-default"></a>Назначение канала избранным отменено по умолчанию

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
    "channelId": "19:cb9c31f1c4c446fa820a64e07cacacc9@thread.tacv2",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="chat-renamed"></a>Чат переименован

```json
{
  "id": "1615943825123",
  "replyToId": null,
  "etag": "1615943825123",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-1706:47:05.123Z",
  "lastModifiedDateTime": "2021-03-1706:47:05.123Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "channelIdentity": null,
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.chatRenamedEventMessageDetail",
    "chatId": "19:2da4c29f6d7041eca70b638b43d45437@thread.v2",
    "chatDisplayName": "Microsoft Teams Members",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="conversation-member-role-updated"></a>Роль участника беседы обновлена

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
    "conversationMemberRoles": [
      "Owner"
    ],
    "conversationMemberUser": {
      "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
      "displayName": null,
      "userIdentityType": "aadUser"
    },
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="meeting-policy-updated"></a>Политика собраний обновлена

```json
{
  "id": "1620732126822",
  "replyToId": null,
  "etag": "1620732126822",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-11T11:22:06.822Z",
  "lastModifiedDateTime": "2021-05-11T11:22:06.822Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.meetingPolicyUpdatedEventMessageDetail",
    "meetingChatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
    "meetingChatEnabled": true,
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-added"></a>Участники добавлены

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersAddedEventMessageDetail",
    "members": [{
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      },
      {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    ],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-deleted"></a>Участники удалены

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersDeletedEventMessageDetail",
    "members": [{
      "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
      "displayName": null,
      "userIdentityType": "aadUser"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-joined"></a>Участники присоединены

```json
{
  "id": "1620050140712",
  "replyToId": null,
  "etag": "1620050140712",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T13:55:40.712Z",
  "lastModifiedDateTime": "2021-05-03T13:55:40.712Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersJoinedEventMessageDetail",
    "members": [{
      "id": "2c3f5f34-ac9f-42e7-8b35-442ccac166cb",
      "displayName": "Alex (Guest)",
      "userIdentityType": "aadUser"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="members-left"></a>Участники вышли

```json
{
  "id": "1620049976741",
  "replyToId": null,
  "etag": "1620049976741",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T13:52:56.741Z",
  "lastModifiedDateTime": "2021-05-03T13:52:56.741Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:meeting_OTFkNDQzMjMtZWQyYi00ZjI4LTk1ZmUtZmI2NjBmNTFmMzg1@thread.v2",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": null,
  "channelIdentity": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.membersLeftEventMessageDetail",
    "members": [{
      "id": "ee8af8acd3184068a935a1f207865620",
      "displayName": "Alex (Guest)",
      "userIdentityType": "anonymousGuest"
    }],
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="tab-updated"></a>Вкладка обновлена

```json
{
  "id": "1616883610266",
  "replyToId": null,
  "etag": "1616883610266",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-03-28T03:50:10.266Z",
  "lastModifiedDateTime": "2021-03-28T03:50:10.266Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616883610266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616883610266&parentMessageId=1616883610266",
  "policyViolation": null,
  "from": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
    "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.tabUpdatedEventMessageDetail",
    "tabId": "tab::e82fa916-3c9a-407e-806b-0b9d8d7492c0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-archived"></a>Команда архивирована

```json
{
  "id": "1623677858199",
  "replyToId": null,
  "etag": "1623677858199",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:37:38.199Z",
  "lastModifiedDateTime": "2021-06-14T13:37:38.199Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623677858199?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623677858199&parentMessageId=1623677858199",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamArchivedEventMessageDetail",
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-created"></a>Команда создана

```json
{
  "id": "1623677858199",
  "replyToId": null,
  "etag": "1623677858199",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:37:38.199Z",
  "lastModifiedDateTime": "2021-06-14T13:37:38.199Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623677858199?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623677858199&parentMessageId=1623677858199",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamCreatedEventMessageDetail",
    "teamId": "19:715b7c2ea0894fe3a503f8958df1ef06@thread.tacv2",
    "teamDisplayName": "Test Team",
    "teamDescription": "This is a test team.",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-description-updated"></a>Описание команды обновлено

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "teamDescription": "Team description updated",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-joining-disabled"></a>Присоединение команды отключено

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamJoiningDisabledEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-joining-enabled"></a>Присоединение команды включено

```json
{
  "id": "1618907417096",
  "replyToId": null,
  "etag": "1618907417096",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-20T08:30:17.096Z",
  "lastModifiedDateTime": "2021-04-20T08:30:17.096Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618907417096?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618907417096&parentMessageId=1618907417096",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamJoiningEnabledEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-renamed"></a>Команда переименована

```json
{
  "id": "1618821548765",
  "replyToId": null,
  "etag": "1618821548765",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-04-19T08:39:08.765Z",
  "lastModifiedDateTime": "2021-04-19T08:39:08.765Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1618821548765?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1618821548765&parentMessageId=1618821548765",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamRenamedEventMessageDetail",
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "teamDisplayName": "Team rename",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "9ee3dc1b-6a70-4582-8bc5-5dd35336b6c3",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-installed"></a>Приложение Teams установлено

```json
{
  "id": "1620046494994",
  "replyToId": null,
  "etag": "1620046494994",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:54:54.994Z",
  "lastModifiedDateTime": "2021-05-03T12:54:54.994Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046494994?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046494994&parentMessageId=1620046494994",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppInstalledEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-removed"></a>Приложение Teams удалено

```json
{
  "id": "1620046597520",
  "replyToId": null,
  "etag": "1620046597520",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:56:37.52Z",
  "lastModifiedDateTime": "2021-05-03T12:56:37.52Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046597520?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046597520&parentMessageId=1620046597520",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppRemovedEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="teams-app-upgraded"></a>Приложение Teams обновлено

```json
{
  "id": "1620046597520",
  "replyToId": null,
  "etag": "1620046597520",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-05-03T12:56:37.52Z",
  "lastModifiedDateTime": "2021-05-03T12:56:37.52Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3Ad0891bf6638f48e8be186e2e92b4a554%40thread.tacv2/1620046597520?groupId=97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1620046597520&parentMessageId=1620046597520",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "97a5ecc4-300b-4c5a-9f87-ca9a4969b3e0",
    "channelId": "19:d0891bf6638f48e8be186e2e92b4a554@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamsAppUpgradedEventMessageDetail",
    "teamsAppId": "aa5fe6c5-f91c-45ed-88de-640e235ad21b",
    "teamsAppDisplayName": "Flipgrid",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "06a5b888-ad96-455e-88ef-c059ec4e4cf0",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```

### <a name="team-unarchived"></a>Архивация команды отменена

```json
{
  "id": "1623678060910",
  "replyToId": null,
  "etag": "1623678060910",
  "messageType": "systemEventMessage",
  "createdDateTime": "2021-06-14T13:41:00.91Z",
  "lastModifiedDateTime": "2021-06-14T13:41:00.91Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": null,
  "importance": "normal",
  "locale": "en-us",
  "webUrl": "https://teams.microsoft.com/l/message/19%3A318c8c65f0794971a1a9b5e3413d77de%40thread.tacv2/1623678060910?groupId=5e91c375-f755-4882-880e-f1b9322faa87&tenantId=df81db53-c7e2-418a-8803-0e68d4b88607&createdTime=1623678060910&parentMessageId=1623678060910",
  "from": null,
  "policyViolation": null,
  "body": {
    "contentType": "html",
    "content": "<systemEventMessage/>"
  },
  "channelIdentity": {
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "channelId": "19:318c8c65f0794971a1a9b5e3413d77de@thread.tacv2"
  },
  "attachments": [],
  "mentions": [],
  "reactions": [],
  "eventDetail": {
    "@odata.type": "#microsoft.graph.teamUnarchivedEventMessageDetail",
    "teamId": "5e91c375-f755-4882-880e-f1b9322faa87",
    "initiator": {
      "application": null,
      "device": null,
      "user": {
        "id": "1fb8890f-423e-4154-8fbf-db6809bc8756",
        "displayName": null,
        "userIdentityType": "aadUser"
      }
    }
  }
}
```
