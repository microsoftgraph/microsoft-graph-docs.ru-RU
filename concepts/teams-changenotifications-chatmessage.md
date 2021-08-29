---
title: Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph
description: Уведомления об изменениях позволяют прослушивать изменения в сообщениях канала или чата
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 82474e8fc13cb1a9dc4d8cc582a9a7aea4f32198
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667810"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a>Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph

Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) сообщений в канале или чате. Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять подпиской. Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

## <a name="subscribe-to-changes-at-the-tenant-level"></a>Подписка на изменения на уровне клиента

Чтобы отслеживать все изменения, связанные с сообщениями в клиенте, вы можете использовать подписки на уровне клиента для сообщений канала и чата. Для этого требуется создать две подписки: одну для отслеживания всех сообщений в [каналах](/graph/api/resources/channel?preserve-view=true), а другую — для отслеживания всех сообщений в [чатах](/graph/api/resources/chat?preserve-view=true).

### <a name="subscribe-to-messages-across-channels"></a>Подписка на сообщения в каналах

Чтобы получать уведомления об изменениях для всех сообщений и ответов по каналам в клиенте, подпишитесь на `/teams/getAllMessages`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

#### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | ChannelMessage.Read.All | Бета-версия, версия 1.0 |

#### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscribe-to-messages-across-chats"></a>Подписка на сообщения в чатах

Чтобы получать уведомления об изменениях всех сообщений в чатах в клиенте, подпишитесь на `/chats/getAllMessages`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

#### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | Chat.Read.All | Бета-версия, версия 1.0 |

#### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-channel"></a>Подписка на сообщения в канале

Чтобы отслеживать сообщения и ответы в канале, вы можете создать подписку на уведомления об изменениях на уровне канала. Для этого подпишитесь на `/teams/{team-id}/channels/{channel-id}/messages`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.

Подписки на уровне канала также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |Поддерживается в версии |
|:--------------------|:---------------------------------------------------------|:--------------------|
|Делегированные (рабочая или учебная учетная запись) | ChannelMessage.Read.All | Бета-версия, версия 1.0 |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | ChannelMessage.Read.Group*, ChannelMessage.Read.All  | Бета-версия, версия 1.0 |

>**Примечание.** Разрешения, помеченные звездочкой (*), поддерживаются в рамках [согласия для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a>Пример 1. Подписка на все сообщения (и ответы) в канале

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a>Пример 2. Подписка на сообщения (и ответы) в канале, содержащие определенный текст

Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a>Пример 3. Подписка на сообщения (и ответы) в канале без данных ресурса

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a>Пример 4. Подписка на сообщения (и ответы) в канале с упоминанием определенного пользователя

Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a>Подписка на сообщения в чате

Чтобы отслеживать сообщения в чате, вы можете создать подписку на уведомления об изменениях на уровне чата. Для этого подпишитесь на `/chats/{chat-id}/messages`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.

Подписки на уровне чата также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.

> **Примечание.** Подписка на сообщения в чате находится в состоянии предварительной версии.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживается в версии |
|:--------------------|:---------------------------------------------------------|:---------------------|
|Делегированные (рабочая или учебная учетная запись) | Chat.Read | Бета-версия, версия 1.0 |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | ChatMessage.Read.Chat*, Chat.Read.All | Бета-версия, версия 1.0 |

>**Примечание.** В настоящее время разрешения, помеченные звездочкой (*), поддерживаются в рамках [согласия для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) только в бета-версии.

### <a name="example-1-subscribe-to-messages-in-a-chat"></a>Пример 1. Подписка на сообщения в чате

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a>Пример 2. Подписка на сообщения в чате, содержащие определенный текст

Следующий запрос отправляет сообщения, содержащие `Hello` подписчику.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a>Пример 3. Подписка на сообщения (и ответы) в чате без данных ресурса

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a>Пример 4. Подписка на сообщения в чате, в которых упоминается определенный пользователь

Чтобы получать уведомления только о сообщениях, в которых упоминался определенный пользователь, укажите ИД пользователя (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` в этом примере) в запросе.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="notification-payloads"></a>Полезные данные уведомлений

В зависимости от вашей подписки вы можете получать уведомление с данными ресурсов или без них. Подписка с данными ресурсов позволяет получать полезные данные вместе с уведомлением, устраняя необходимость обратного вызова и получения содержимого.

### <a name="notifications-with-resource-data"></a>Уведомления с данными ресурсов

Для уведомлений с данными ресурсов полезные данные выглядят следующим образом. Это полезные данные для сообщения, отправленного в чате.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).

Расшифрованные полезные данные уведомления выглядят следующим образом. Полезные данные соответствуют схеме [chatMessage](/graph/api/resources/chatMessage?preserve-view=true). Полезные данные похожи на результаты, возвращаемые операциями GET.

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a>Уведомления без данных о ресурсах

Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения. Для подписок на уведомления без данных о ресурсах не требуется сертификат шифрования (так как фактические данные ресурсов не передаются).

Полезные данные выглядят следующим образом. Это полезные данные для сообщения, отправленного в канале.

```json
 {
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```

Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения. Вызовы GET всегда возвращают текущее состояние сообщения. Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.

## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
