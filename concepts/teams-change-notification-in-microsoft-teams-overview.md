---
title: Уведомления об изменениях для ресурсов Microsoft Teams
description: Подпишитесь на изменения ресурсов и данных ресурсов в Microsoft Teams с помощью API Microsoft Graph. Узнайте о типах уведомлений об изменениях и полезной нагрузке.
author: anandab-msft
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0091ded928de826220b837a66873e736fb1e84bc
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555571"
---
# <a name="change-notifications-for-microsoft-teams-resources"></a>Уведомления об изменениях для ресурсов Microsoft Teams

Уведомления об изменениях ресурсов Microsoft Teams с помощью Microsoft Graph позволяют подписаться на изменения (создание, обновление и удаление) ресурса. Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks). Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

> [!NOTE]
> Максимальное время подписки может длиться 60 минут; однако подписки можно продлевать до тех пор, пока вызывающая сторона не получит разрешения на доступ к ресурсу.

## <a name="change-notification-types"></a>Типы уведомлений об изменениях

Microsoft Teams поддерживает два типа уведомлений об изменениях:

- **Уведомление об изменении для отслеживания всех изменений, связанных с ресурсом в клиенте:** например, вы можете подписаться на изменения в сообщениях в любом канале в клиенте и получать уведомления всякий раз, когда сообщение создается, обновляется или удаляется в любом канале в клиенте. Эти уведомления могут иметь [требования к лицензированию и оплате](/graph/teams-licenses), такие как уведомления об изменениях для [сообщений](teams-changenotifications-chatmessage.md) и [членства](teams-changenotifications-chatMembership.md).

- **Уведомление об изменении для отслеживания всех изменений для определенного ресурса:** например, вы можете подписаться на изменения в сообщениях в определенном канале и получать уведомления всякий раз, когда сообщение создается, обновляется или удаляется в этом канале.

Дополнительные сведения о том, какие ресурсы поддерживают определенные типы уведомлений об изменениях, см. в статье [Уведомления об изменениях Microsoft Graph](webhooks.md).

## <a name="supported-resources"></a>Поддерживаемые ресурсы
В следующей таблице перечислены ресурсы Microsoft Teams и соответствующие пути к ресурсам, которые сейчас поддерживаются.

| **Ресурс** | **Поддерживаемые пути ресурсов** | **Можно ли данные ресурсов включать в уведомления** |
|:----------------|:------------|:-----------------------------------------|
| [Канал](/graph/api/resources/channel) Teams  | Изменения каналов во всех командах:<br>`/teams/getAllChannels` <br>Изменения канала в определенной команде:<br>`/teams/{id}/channels` | Да |
| [Чат](/graph/api/resources/chat) Teams | Изменения в любом чате в клиенте:<br>`/chats` <br>Изменения в конкретном чате:<br>`/chats/{id}` | Да |
| [chatMessage](/graph/api/resources/chatMessage) Teams | Изменения в сообщениях чата во всех каналах во всех командах:<br>`/teams/getAllMessages` <br>Изменения в сообщениях чата на определенном канале:<br>`/teams/{id}/channels/{id}/messages`<br>Изменения в сообщениях чата во всех чатах:<br>`/chats/getAllMessages` <br>Изменения в сообщениях чата в конкретном чате:<br>`/chats/{id}/messages`<br>Изменения в сообщениях чата во всех чатах, в которых участвует конкретный пользователь:<br>`/users/{id}/chats/getAllMessages` | Да |
| [conversationMember](/graph/api/resources/conversationMember) в Teams | Изменения участия в определенной команде:<br>`/teams/{id}/members` <br> Изменения участия в определенном чате:<br>`/chats/{id}/members` <br> Изменения участия во всех чатах:<br>`/chats/getAllMembers` <br> Изменения участия во всех каналах определенной команды:<br>`teams/{id}/channels/getAllMembers` | Да |
| [Команда](/graph/api/resources/team) Teams | Изменения в любой команде в клиенте:<br>`/teams` <br>Изменения в конкретной команде:<br>`/teams/{id}` | Да |
 

## <a name="notification-payloads"></a>Полезные данные уведомлений

В зависимости от вашей подписки вы можете получать уведомление с данными ресурсов или без них. Подписка с данными ресурсов позволяет получать полезные данные сообщения вместе с уведомлением, что устраняет необходимость обратного вызова и получения содержимого.

### <a name="notifications-with-resource-data"></a>Уведомления с данными ресурсов

Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.  Эти полезные данные предназначены для уведомления, соответствующего ресурсу сообщения чата. Фактическое уведомление включает свойства **resource** и **resourceData**, представляющие ресурс, который вызвал уведомление.

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

Расшифрованные полезные данные уведомления выглядят следующим образом. Расшифрованные полезные данные в предыдущем примере соответствуют схеме [chatMessage](/graph/api/resources/chatMessage). Полезные данные похожи на результаты, возвращаемые операциями GET.

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

### <a name="notifications-without-resource-data"></a>Уведомления без данных ресурса

Уведомления без данных ресурса предоставляют достаточно сведений, чтобы выполнить вызов GET для получения ресурса. Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).

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

В примере выше показано уведомление, соответствующее ресурсу сообщения чата. Фактическое уведомление включает свойства **resource** и **resourceData**, представляющие ресурс, который вызвал уведомление. Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные ресурса.

> [!NOTE]
> Вызовы GET всегда возвращают текущее состояние ресурса. Если ресурс изменяется между отправкой уведомления и получением ресурса, операция возвращает обновленный ресурс.

## <a name="see-also"></a>См. также

- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
