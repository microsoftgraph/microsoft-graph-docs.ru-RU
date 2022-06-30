---
title: Получение уведомлений об изменениях собраний по сети в Microsoft Graph
description: Уведомления об изменениях в Microsoft Graph позволяют подписаться на начатые/завершенные собрания по сети и обновления состава участников для собраний Microsoft Teams.
author: benlee-msft
ms.localizationpriority: high
ms.prod: cloud-communications
ms.custom: scenarios:getting-started
ms.openlocfilehash: 90cae49f4f342a05eafe1e0099bb6eb60d3c2b04
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436409"
---
# <a name="get-change-notifications-for-meeting-call-updates-in-microsoft-graph"></a>Получение уведомлений об изменениях для обновлений звонков собраний в Microsoft Graph

Уведомления об изменениях в Microsoft Graph позволяют подписаться на начатые/завершенные звонки и обновления состава звонков для собраний Microsoft Teams. Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять подпиской. Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.

### <a name="subscribe-to-messages-across-all-channels"></a>Подписка на сообщения во всех каналах

Чтобы получать уведомления об изменениях событий звонков собрания в приложении, подпишитесь на `/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'`. Этот ресурс поддерживает [включение данных ресурса](/graph/webhooks-with-resource-data) в уведомление.

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
  "resource": "/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2021-02-01T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="joinweburl"></a>JoinWebUrl
URL-адрес для присоединения к собранию включается в свойство joinWebUrl ресурса [onlineMeeting](/graph/api/resources/onlineMeeting) или в клиент Teams для собрания.


## <a name="notifications-with-encrypted-resource-data"></a>Уведомления с зашифрованными данными ресурсов
```json
{
  "value": [{
    "subscriptionId": "{Subscription id}",
    "clientState": "{secret client state}",
    "changeType": "updated",
    "tenantId": "{Organization/Tenant id}",
    "resource": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
    "subscriptionExpirationDateTime": "2022-02-28T00:00:00.0000000Z",
    "resourceData": {
      "@odata.id": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'"
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

Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](/graph/webhooks-with-resource-data).

### <a name="event-notifications-types"></a>Типы уведомлений о событиях
Ниже указаны поддерживаемые события собраний.
- CallStarted — возникает при начале звонка собрания.
- CallEnded — возникает при завершении звонка собрания.
- CallRosterUpdate — возникает, когда участник присоединяется к звонку или покидает его.

### <a name="decrypted-payload-examples"></a>Расшифрованные примеры полезных данных

#### <a name="callstartedcallended"></a>CallStarted/CallEnded.
```json
{
  "@odata.type":"#Microsoft.Graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "eventType":"{Microsoft.Communication.CallStarted or Microsoft.Communication.CallEnded}",
  "eventDateTime":"2022-02-28T00:00:00.0000000Z",
  "state":"active"
}
```

#### <a name="callrosterupdate"></a>CallRosterUpdate
```json
{
  "@odata.type":"#Microsoft.Graph.onlineMeeting",
  "@odata.id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "id":"communications/onlineMeetings?$filter=joinWebUrl+eq+'{joinWebUrl}'",
  "eventType":"Microsoft.Communication.CallRosterUpdate",
  "eventDateTime":"2022-02-28T00:00:00.0000000Z",
  "state":"active",
  "activeParticipants@delta": ["{meetingParticipantInfo list of users that joined}"],
  "activeParticipants@remove": ["{meetingParticipantInfo list of users that left}"]
}
```
События **CallRosterUpdate** будут включать два дополнительных свойства: **activeParticipants@delta** для отображения участников, добавленных в собрание, и **activeParticipants@remove** для участников, покидающих собрание по сети. Подробности о сведениях об участниках см. в разделе о [типе ресурса meetingParticipantInfo](/graph/api/resources/meetingparticipants).

Вы можете пропустить шифрование, не включив свойство **includeResourceData** или присвоив это значение для `false` в тексте запроса на подписку. Это приведет к добавлению в **resourceData** свойств, которые были бы частью зашифрованных полезных данных.


## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](/graph/webhooks)
- [Обзор API Microsoft Teams](/graph/teams-concept-overview)
- [Ресурс собрания по сети](/graph/api/resources/onlineMeeting)
