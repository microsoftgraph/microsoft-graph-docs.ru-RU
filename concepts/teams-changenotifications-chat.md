---
title: Получение уведомлений об изменениях чатов с помощью Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание и обновление) чатов с помощью API Microsoft Graph.
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 0846cef129ff103cbf5ba8ca8095fe7bdf26aa4e
ms.sourcegitcommit: 4c8444b732b8d6d0de8a95f6666c42095f146266
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/08/2022
ms.locfileid: "62442822"
---
# <a name="get-change-notifications-for-chats-using-microsoft-graph"></a>Получение уведомлений об изменениях чатов с помощью Microsoft Graph

Уведомления об изменениях позволяют подписаться на изменения (создание и обновление) чатов. Вы можете получать уведомления при создании или обновлении чата. Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

## <a name="subscribe-to-changes-in-any-chat-at-tenant-level"></a>Подписка на изменения в любом чате на уровне клиента

Чтобы получать уведомления обо всех изменениях (создание и обновление), связанных с любым чатом в клиенте, подпишитесь на `/chats`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Сервер приложений | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All   | бета|

### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-chat"></a>Подписка на изменения в определенном чате


Чтобы получать уведомления обо всех изменениях, связанных с определенным чатом, подпишитесь на `/chats/{id}`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite | Бета |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All | Бета |

> **Примечание**. Разрешения, помеченные звездочкой (*), используют [согласие для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a>Уведомления с данными ресурсов

Для уведомлений с данными ресурсов полезные данные выглядят следующим образом. Эти полезные данные относятся к изменению свойства в чате.

```json
{
    "value": [{
        "subscriptionId": "352887e3-9be0-4b6f-a4e6-dec118d857db",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T09:50:37.719033+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
        "resourceData": {
            "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
            "@odata.type": "#microsoft.graph.chat",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        }
            "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
        }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).

Расшифрованные полезные данные уведомления выглядят следующим образом. Полезные данные соответствуют схеме [chats](/graph/api/resources/chat?preserve-view=true). Полезные данные похожи на результаты, возвращаемые операциями GET.

```json
{
  "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
  "topic": null,
  "createdDateTime": "2021-06-03T14:25:04+05:30",
  "lastUpdatedDateTime": "2021-06-03T14:25:04.387Z",
  "chatType": "oneOnOne",
  "members": [
    {
      "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyM5NzZmNGIzMS1mZDAxLTRlMGItOTE3OC0yOWNjNDBjMTQ0Mzg=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    },
    {
      "userId": "ee723d3d-22d0-4394-9c32-5764d68f4672",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyNlZTcyM2QzZC0yMmQwLTQzOTQtOWMzMi01NzY0ZDY4ZjQ2NzI=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    }
  ],
  "messages": [],
  "installedApps": [],
  "tabs": [],
  "permissionGrants": [],
  "operations": []
}
```

### <a name="notifications-without-resource-data"></a>Уведомления без данных о ресурсах

Следующие полезные данные описывают сведения, отправляемые в запросе на уведомления без данных ресурса. Эти конкретные полезные данные означают, что создан новый чат.

```json
{
    "subscriptionId": "8d85051d-779d-45bc-be92-e433f0a5d8ac",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:26:09.8959595+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
    "resourceData": {
        "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
        "@odata.type": "#microsoft.graph.chat",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
    }
}
```

Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные сведений о чате. Вызовы GET всегда возвращают текущее состояние сведений о чате. Если сведения о чате обновились после отправки уведомления и до получения сведений о чате, операция возвращает обновленные сведения о чате.

## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
