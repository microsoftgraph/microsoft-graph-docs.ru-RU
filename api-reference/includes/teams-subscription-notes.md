---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 6e5f62d52969dcc1b332b2cd6e5f02f318c8b6a9
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65135271"
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
