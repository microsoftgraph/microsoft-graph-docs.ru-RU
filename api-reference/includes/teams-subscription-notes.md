---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: e9b65c0ed6c82e94a38bbeb08b208fbe24d60176
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390815"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data). Единственным исключением является ресурс `/users/{id}/chats/getAllMessages` (доступный только в бета-версии), который поддерживает данные ресурса независимо от типа разрешения.

Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data). Создание подписки завершается сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription). Перед созданием подписки **chatMessage** требуется запросить доступ. Дополнительные сведения см. в статье [Защищенные API в Microsoft Teams](/graph/teams-protected-apis).

Вы должны использовать заголовок запроса `Prefer: include-unknown-enum-members` для получения следующих значений в **chatMessage** **messageType** [evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `systemEventMessage` для ресурса `/teams/{id}/channels/{id}/messages` и `/chats/{id}/messages`.

> [!NOTE]
>`/teams/getAllMessages`и `/chats/getAllMessages` имеет требования к [лицензированию и оплате](/graph/teams-licenses).
> `/teams/getAllMessages` и `/chats/getAllMessages` поддерживают параметры `model=A` и `model=B` запросов.
> Если модель не указана, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

### <a name="conversationmember"></a>conversationMember

> [!NOTE]
>`/teams/getAllMembers`и `/chats/getAllMembers` имеет требования к [лицензированию и оплате](/graph/teams-licenses).
> `/teams/getAllMembers` и `/chats/getAllMembers` поддерживают параметры `model=A` и `model=B` запросов.
> Если модель не указана, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

#### <a name="request-example"></a>Пример запроса

Укажите параметр запроса `model` в свойстве **ресурса** в тексте запроса.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "chats/getAllMessages?model=A",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
