---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.openlocfilehash: f3854b06c7d4dc584a922f9c454947785b74947f
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2021
ms.locfileid: "53005735"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data).

Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data). Создание подписки завершится сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription). Перед созданием подписки **chatMessage** вы должны запросить доступ. Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis). 

> **Примечания.** 
>
>`/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses). В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества данных, доступ к которым получен через API-интерфейс.
