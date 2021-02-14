---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.openlocfilehash: f2def5f5a22267146d5b3005cd2f9be82e1d0db9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50243084"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data).

Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data). Создание подписки завершится сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription). Перед созданием подписки **chatMessage** вы должны запросить доступ. Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis). 

> **Примечания.** 
>
>`/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).
В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на базе количества данных, доступ к которым получен через API-интерфейс.
>
>`/chats/getAllMessages` возвращает только сообщения из чатов, принадлежащих клиенту. Если цепочка чата инициирована пользователем из-за пределов клиента, она не принадлежит клиенту и для нее не создаются уведомления об изменениях.
