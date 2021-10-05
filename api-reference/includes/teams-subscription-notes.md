---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 398ba544748b3bf60728eda051059fc6f7e1d517
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115174"
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