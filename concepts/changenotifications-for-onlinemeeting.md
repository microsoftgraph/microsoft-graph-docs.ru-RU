---
title: Получение уведомлений об изменениях для обновлений звонков собраний в Microsoft Graph
description: Уведомления об изменениях в Microsoft Graph позволяют подписаться на начатые/завершенные звонки и обновления состава звонков для собраний Microsoft Teams.
author: benlee-msft
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: bca104717d5b6c50f53eabe21e450ea3520d2a8b
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63376523"
---
# <a name="get-change-notifications-for-meeting-call-updates-in-microsoft-graph"></a>Получение уведомлений об изменениях для обновлений звонков собраний в Microsoft Graph

Уведомления об изменениях в Microsoft Graph позволяют подписаться на начатые/завершенные звонки и обновления состава звонков для собраний Microsoft Teams. Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять подпиской. Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

### <a name="subscribe-to-messages-across-all-channels"></a>Подписка на сообщения во всех каналах

Чтобы получать уведомления об изменениях событий звонков собрания в приложении, подпишитесь на `/communications/onlineMeetings/{meeting-id}`. Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.

#### <a name="permissions"></a>Разрешения

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              | Поддерживаемые версии |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается. | Не поддерживается. |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    | Не поддерживается. |
|Для приложений | OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All | бета |

#### <a name="example"></a>Пример

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/communications/onlineMeetings/{meeting-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2021-02-01T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```
## <a name="notifications-with-encrypted-resource-data"></a>Уведомления с зашифрованными данными ресурсов
```json
{
  "value": [{
    "subscriptionId": "{Subscription id}",
    "clientState": "{secret client state}",
    "changeType": "updated",
    "tenantId": "{Organization/Tenant id}",
    "resource": "communications/onlineMeeting/{meeting-id}",
    "subscriptionExpirationDateTime": "2022-02-28T02:00:00-08:00",
    "resourceData": {
      "@odata.id": "communications/onlineMeetings/{meeting-id}",
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "communications/onlineMeetings/{meeting-id}"
    },
    "organizationId": "{Organization/Tenant id}",
    "encryptedContent": {
      "data": "{Encrypted content}",
      "dataSignature": "{Encrypted data signature}",
      "dataKey": "{Encrypted data key for encrypting content}",
      "encryptionCertificateId": "{User specified id of encryption certificate}",
      "encryptionCertificateThumbprint": "{Encrpytion certification thumbprint}"
    }
  }],
  "validationTokens": ["{Validation Tokens}"]
}
```

Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).

Расшифрованные полезные данные уведомления выглядят следующим образом.
```json
{
  "@odata.type":"#microsoft.graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings/{meeting-id}",
  "id":"communications/onlineMeetings/{meeting-id}",
  "eventType":"Microsoft.Communication.CallStarted",
  "eventDateTime":"2022-02-28T18:41:33.0553203Z",
  "state":"active"
}
```

Вы можете пропустить шифрование, не включив свойство **includeResourceData** или присвоив это значение для `false` в тексте запроса на подписку.
## <a name="event-notifications-types"></a>Типы уведомлений о событиях
Ниже указаны поддерживаемые события собраний.
- CallStarted — возникает при начале звонка собрания.
- CallEnded — возникает при завершении звонка собрания.
- CallRosterUpdate — возникает, когда участник присоединяется к звонку или покидает его.

События **CallRosterUpdate** будут включать два дополнительных свойства (**activeParticipants@delta** и **activeParticipants@remove**), чтобы изобразить в свойстве **resourceData** участников, присоединяющихся к звонку собрания или покидающих его.

## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
- [Ресурс собрания по сети](/graph/api/resources/onlinemeeting.md)
