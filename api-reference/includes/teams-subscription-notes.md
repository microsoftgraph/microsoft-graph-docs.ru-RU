---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 0bd1801747eb5f4871e121009bb2017b2c17c9f3
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61323857"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data). Единственным исключением является ресурс `/users/{id}/chats/getAllMessages` (доступный только в бета-версии), который поддерживает данные ресурса независимо от типа разрешения.

Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data). Создание подписки завершается сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription). Перед созданием подписки **chatMessage** требуется запросить доступ. Дополнительные сведения см. в статье [Защищенные API в Microsoft Teams](/graph/teams-protected-apis).

Для получения следующих значений в `Prefer: include-unknown-enum-members` **chatMessage** **messageType** [evolvable enum:](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)for and resource необходимо использовать заготку `systemEventMessage` `/teams/{id}/channels/{id}/messages` `/chats/{id}/messages` запроса.

> [!NOTE]
>`/teams/getAllMessages`и `/chats/getAllMessages` имеет требования к [лицензированию и оплате.](/graph/teams-licenses)
> `/teams/getAllMessages` и `/chats/getAllMessages` поддерживают `model=A` параметры и `model=B` запросы.
> Если модель не указана, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

### <a name="conversationmember"></a>conversationMember

> [!NOTE]
>`/teams/getAllMembers`и `/chats/getAllMembers` имеет требования к [лицензированию и оплате.](/graph/teams-licenses)
> `/teams/getAllMembers` и `/chats/getAllMembers` поддерживают `model=A` параметры и `model=B` запросы.
> Если модель не указана, будет использоваться [режим оценки](/graph/teams-licenses#evaluation-mode-default-requirements).

### <a name="request-example"></a>Пример запроса

Укажите `model` параметр запроса в **свойстве ресурса** в теле запроса.

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
