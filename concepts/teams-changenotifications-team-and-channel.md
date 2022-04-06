---
title: Получение уведомлений об изменениях команд и каналов с помощью Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание, обновление и удаление) команд и каналов с помощью API Microsoft Graph.
author: anandab
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: b6bbfac2cbdb8fcafccbd385c4aa43c994f3c04d
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684699"
---
# <a name="get-change-notifications-for-teams-and-channels-using-microsoft-graph"></a>Получение уведомлений об изменениях команд и каналов с помощью Microsoft Graph

Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) команд и каналов. Вы можете получать уведомления при создании, обновлении и удалении команды или канала. Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

## <a name="subscribe-to-changes-in-any-team-at-tenant-level"></a>Подписка на изменения в любой команде на уровне клиента

Чтобы получать уведомления обо всех изменениях (создание, обновление и удаление), связанных с любой командой в клиенте, подпишитесь на `/teams`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All   | бета|

### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-team"></a>Подписка на изменения в определенной команде


Чтобы получать уведомления обо всех изменениях, связанных с определенной командой в клиенте, подпишитесь на `/teams/{team-id}`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All | Бета |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All    | Бета |

>**Примечание.** Разрешения, помеченные звездочкой (*), поддерживаются в рамках [согласия для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


## <a name="subscribe-to-changes-in-any-channel-at-tenant-level"></a>Подписка на изменения в любом канале на уровне клиента

Чтобы получать уведомления обо всех изменениях (создание, обновление и удаление), связанных с любым каналом в клиенте, подпишитесь на `/teams/getAllChannels`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.


### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Приложение | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All | бета |

### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllChannels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-any-channel-of-a-particular-team"></a>Подписка на изменения в любом канале определенной команды


Чтобы получать уведомления обо всех изменениях, связанных с любым каналом в определенной команде, подпишитесь на `/teams/{team-id}/channels`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление. Уведомления об изменениях для частных каналов не поддерживаются в делегированном контексте. В этом случае подписчик этого ресурса в делегированном контексте получает уведомления только для стандартных каналов определенной команды, но не для частных каналов. Уведомления об изменениях для общих каналов не поддерживаются.


### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All | Бета |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Для приложений | ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All   | Бета |

>**Примечание.** Разрешения, помеченные звездочкой (*), поддерживаются в рамках [согласия для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a>Уведомления с данными ресурсов

Для уведомлений с данными ресурсов полезные данные выглядят следующим образом. Эти полезные данные относятся к изменению свойства в команде.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.Team",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')"
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



Расшифрованные полезные данные уведомления выглядят следующим образом. Полезные данные соответствуют схеме [teams](/graph/api/resources/team?preserve-view=true). Полезные данные похожи на результаты, возвращаемые операциями GET.

>**Примечание.** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) и [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) не предоставляются в полезных данных.

```json
{
  "id": "4c533ad3-e1dd-4277-a672-92ab64ed225c",
  "createdDateTime": "2021-03-18T10:31:14.597Z",
  "displayName": "Sample name",
  "description": "Sample description",
  "internalId": "19:2077546f765a42c1ba71236f4df70aa2@thread.tacv2",
  "specialization": "none",
  "visibility": "public",
  "webUrl": "https://teams.microsoft.com/l/team/19:2077546f724a42c1ba71236f4df79aa2%40thread.tacv2/conversations?groupId=4c533ad3-e1dd-4277-a672-92ab64ed225c&tenantId=0f2e8f59-862a-483b-9ca8-82a10665e17d",
  "isArchived": false,
  "isMembershipLimitedToOwners": false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowCreatePrivateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "allowCreateUpdateChannels": false,
    "allowDeleteChannels": false
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "moderate",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```


Для уведомлений с данными ресурсов полезные данные выглядят следующим образом. Эти полезные данные относятся к изменению свойства в канале.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')",
        "resourceData": {
            "id": "19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2",
            "@odata.type": "#Microsoft.Graph.Channel",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')"
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
  

Расшифрованные полезные данные уведомления выглядят следующим образом. Полезные данные соответствуют схеме [channel](/graph/api/resources/channel?preserve-view=true). Полезные данные похожи на результаты, возвращаемые операциями GET.

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


### <a name="notifications-without-resource-data"></a>Уведомления без данных о ресурсах

Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения. Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).

Для уведомлений без данных ресурса полезные данные выглядят следующим образом. Эти полезные данные относятся к изменению свойства в команде.

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.Teams",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')"
  }
}
```

Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения. Вызовы GET всегда возвращают текущее состояние сообщения. Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.


>**Примечание.** Адрес электронной почты канала не возвращается в полезных данных.

Для уведомлений без данных ресурса полезные данные выглядят следующим образом. Эти полезные данные относятся к изменению свойства в команде.

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
