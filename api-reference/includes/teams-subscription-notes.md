---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 0c2faca238d1127462de5f70aadffd1ef3edd2d0
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61132218"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data). Единственным исключением является ресурс `/users/{id}/chats/getAllMessages` (доступный только в бета-версии), который поддерживает данные ресурса независимо от типа разрешения.

Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data). Создание подписки завершается сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription). Перед созданием подписки **chatMessage** требуется запросить доступ. Дополнительные сведения см. в статье [Защищенные API в Microsoft Teams](/graph/teams-protected-apis).

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
