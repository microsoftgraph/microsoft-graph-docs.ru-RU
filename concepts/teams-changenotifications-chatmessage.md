---
title: Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph
description: Уведомления об изменениях позволяют прослушивать изменения в сообщениях канала или чата
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1d9767a913b5fe5878cb1cc8e72ec9900fcec4ac
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000719"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a>Получение уведомлений об изменениях сообщений в каналах и чатах Teams с помощью Microsoft Graph

Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) [сообщений](/graph/api/resources/chatMessage?preserve-view=true) в [канале](/graph/api/resources/channel?preserve-view=true) или [чате](/graph/api/resources/chat?preserve-view=true). Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks?preserve-view=true). Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

>**Примечание.** Максимальный срок действия подписки составляет 60 минут. Однако подписки можно продлевать, пока у вызывающий не получит разрешения на доступ к ресурсу.

## <a name="subscribe-to-changes-at-the-tenant-level"></a>Подписка на изменения на уровне клиента

Чтобы отслеживать все изменения, связанные с сообщениями в клиенте, вы можете использовать подписки на уровне клиента для сообщений канала и чата. Для этого требуется создать две подписки: одну для отслеживания всех сообщений в [каналах](/graph/api/resources/channel?preserve-view=true), а другую — для отслеживания всех сообщений в [чатах](/graph/api/resources/chat?preserve-view=true).

### <a name="subscribe-to-messages-across-channels"></a>Подписка на сообщения в каналах

Чтобы получать уведомления об изменениях всех сообщений и ответов в каналах в клиенте, подпишитесь на `/teams/getAllMessages`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

#### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | ChannelMessage.Read.All |

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

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Chat.Read.All |

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

Чтобы отслеживать сообщения и ответы в канале, вы можете создать подписку на уведомления об изменениях на уровне канала. Для этого подпишитесь на `/teams{id}/channels/{id}/messages`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.

Подписки на уровне канала также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | ChannelMessage.Read.All |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | ChannelMessage.Read.All |

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a>Пример 1. Подписка на все сообщения (и ответы) в канале

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
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
  "resource": "/teams/{id}/channels/{id}/messages?$search=Hello",
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
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a>Подписка на сообщения в чате

Чтобы отслеживать сообщения в чате, вы можете создать подписку на уведомления об изменениях на уровне чата. Для этого подпишитесь на `/chats{id}/messages`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление *в режиме только для приложения*.

Подписки на уровне чата также поддерживают поиск на основе ключевых слов с помощью параметра запроса `$search`.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Chat.Read |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Chat.Read.All |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a>Пример 1. Подписка на сообщения в чате

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
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
  "resource": "/chats/{id}/messages?$search=Hello",
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
  "resource": "/chats/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
