---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 15f177d00c7b024e7b1e4ec8195770e2fa809879
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555161"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

Подписки **chatMessage** можно указать, чтобы включить данные ресурсов. Если задано включение данных ресурсов (**includeResourceData** имеет значение `true`), требуется [шифрование](/graph/webhooks-with-resource-data). Подписку нельзя создать, если для таких подписок не указан [encryptionCertificate](/graph/api/resources/subscription). До создания **подписки chatMessage** с разрешениями приложения, возможно, потребуется запросить доступ. Дополнительные сведения см. в статье [Защищенные API в Microsoft Teams](/graph/teams-protected-apis).

Вы должны использовать заголовок запроса `Prefer: include-unknown-enum-members` для получения следующих значений в **chatMessage** **messageType** [evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `systemEventMessage` для ресурса `/teams/{id}/channels/{id}/messages` и `/chats/{id}/messages`.

> [!NOTE]
>`/teams/getAllMessages`, `/chats/getAllMessages`, `/me/chats/getAllMessages` и `/users/{id}/chats/getAllMessages` имеют [требования к лицензированию и оплате](/graph/teams-licenses).
> `/teams/getAllMessages` и `/chats/getAllMessages` поддерживают параметры `model=A` и `model=B` запросов, а `/me/chats/getAllMessages` и `/users/{id}/chats/getAllMessages` поддерживают только `model=B`.
> Если модель не указана, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

### <a name="conversationmember"></a>conversationMember
**Подписки conversationMember** можно указать, чтобы включить данные ресурсов. Если задано включение данных ресурсов (**includeResourceData** имеет значение `true`), требуется [шифрование](/graph/webhooks-with-resource-data). Создание подписки завершается сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription).

> [!NOTE]
>`/teams/getAllMembers`и `/chats/getAllMembers` имеет требования к [лицензированию и оплате](/graph/teams-licenses).
> `/teams/getAllMembers` и `/chats/getAllMembers` поддерживают параметры `model=A` и `model=B` запросов.
> Если модель не указана, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

### <a name="team-channel-and-chat"></a>команда, канал и чат
**Можно** **указать** подписки  команды, канала и чата, чтобы включить данные ресурсов. Если задано включение данных ресурсов (**includeResourceData** имеет значение `true`), требуется [шифрование](/graph/webhooks-with-resource-data). Создание подписки завершается сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription).

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
