---
title: Получение уведомлений об изменениях участников в командах и каналах с помощью Microsoft Graph
description: Получение уведомлений о любых изменениях (создание, обновление и удаление) участников команд и каналов с помощью Microsoft Graph.
author: anandab
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: bdc228637496774dd7eb90dcd9b09dff8a6c9da7
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900477"
---
# <a name="get-change-notifications-for-membership-changes-in-teams-and-channels-using-microsoft-graph"></a>Получение уведомлений об изменениях участников в командах и каналах с помощью Microsoft Graph

Уведомления об изменениях позволяют подписаться на изменения участников (создание, обновление и удаление) в командах и закрытых каналах. Вы можете получать уведомления при добавлении, удалении или изменении участника в команде или в закрытом канале. Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

## <a name="subscribe-to-changes-in-membership-of-a-particular-team"></a>Подписка на изменения участников определенной команды

Чтобы получать уведомления об изменениях участников определенной команды, подпишитесь на `/teams/{team-id}/members`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | TeamMember.Read.All, TeamMember.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | TeamMember.Read.Group*, TeamMember.Read.All, TeamMember.ReadWrite.All   |

>**Примечание.** Разрешения, помеченные звездочкой (*), поддерживаются в рамках [согласия для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-membership-changes-in-all-private-channels-of-a-particular-team"></a>Подписка на изменения участников во всех закрытых каналах определенной команды

Чтобы получать уведомления об изменениях участников во всех закрытых каналах определенной команды, подпишитесь на `/teams/{team-id}/channels/getAllMembers`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

[!INCLUDE [teams-model-A-and-B-disclaimer](../includes/teams-model-A-and-B-disclaimer.md)]

### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | ChannelMember.Read.All   |


### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/getAllMembers",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```




### <a name="notifications-with-resource-data"></a>Уведомления с данными ресурсов

Для уведомлений с данными ресурсов полезные данные выглядят следующим образом. Эти полезные данные относятся к изменению участников в команде.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
        "resourceData": {
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
            "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
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

Полезные данные для событий участников канала аналогичны предыдущим полезным данным, за исключением того, что свойство **ресурса** указывает на участника канала, а не на участника команды.

Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).

Расшифрованные полезные данные уведомления выглядят следующим образом. Полезные данные соответствуют схеме [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true). Полезные данные похожи на результаты, возвращаемые операциями GET.

```json
{
  "id": "/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [
    "owner"
  ],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="notifications-without-resource-data"></a>Уведомления без данных о ресурсах

Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения. Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).

Для уведомлений без данных ресурса полезные данные выглядят следующим образом. Эти полезные данные относятся к изменению участников в команде.

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
  "resourceData": {
    "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk",
    "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
    "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
  }
}
```

Полезные данные для событий участников канала аналогичны предыдущим полезным данным, за исключением того, что свойство **ресурса** указывает на участника канала, а не на участника команды.

Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения. Вызовы GET всегда возвращают текущее состояние сообщения. Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.

## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
