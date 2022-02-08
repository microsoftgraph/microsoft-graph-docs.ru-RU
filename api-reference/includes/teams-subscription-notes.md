---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 5702c0489c9662f85b02c31a6cf6d3aba241208b
ms.sourcegitcommit: 38e16940da74bda465f890d945f9dc4aa412c6f4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/05/2022
ms.locfileid: "62425300"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data). Единственным исключением является ресурс `/users/{id}/chats/getAllMessages` (доступный только в бета-версии), который поддерживает данные ресурса независимо от типа разрешения.

Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data). Создание подписки завершается сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription). Перед созданием подписки **chatMessage** требуется запросить доступ. Дополнительные сведения см. в статье [Защищенные API в Microsoft Teams](/graph/teams-protected-apis).

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
