---
title: Уведомления об изменениях ресурсов Microsoft Teams с использованием Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание, обновление и удаление) ресурсов в Microsoft Teams с помощью API Microsoft Graph
author: anandab-msft
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9433a4c5ee000fa34e125440168b865f1bb16172
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430894"
---
# <a name="change-notifications-for-microsoft-teams-resources-using-microsoft-graph"></a>Уведомления об изменениях ресурсов Microsoft Teams с использованием Microsoft Graph

Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) ресурса. Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks?preserve-view=true). Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

> **Примечание.** Максимальный срок действия подписки составляет 60 минут. Однако подписки можно продлевать, пока у вызывающий не получит разрешения на доступ к ресурсу.

## <a name="change-notification-types"></a>Типы уведомлений об изменениях
Microsoft Teams поддерживает два типа уведомлений об изменениях:
- **Уведомление об изменении для отслеживания всех изменений, связанных с ресурсом в клиенте**. Например, вы можете подписаться на изменения сообщений любого канала в клиенте и получать уведомления при создании, обновлении или удалении сообщения в любом канале в клиенте.
- **Уведомление об изменении для отслеживания всех изменений определенного ресурса**. Например, вы можете подписаться на изменения сообщений определенного канала и получать уведомления при создании, обновлении или удалении сообщения в этом канале.

Дополнительные сведения о том, какие ресурсы поддерживают определенные типы уведомлений об изменениях, см. в статье [Уведомления об изменениях Microsoft Graph](webhooks.md).
 

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

Расшифрованные полезные данные уведомления выглядят следующим образом. Расшифрованные полезные данные в предыдущем примере соответствуют схеме [chatMessage](/graph/api/resources/chatMessage?preserve-view=true). Полезные данные похожи на результаты, возвращаемые операциями GET.

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

> **Примечание**. Вызовы GET всегда возвращают текущее состояние ресурса. Если ресурс изменяется с момента отправки уведомления и до его получения, операция возвращает обновленный ресурс.

## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
