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

### <a name="chatmessage"></a><span data-ttu-id="a2e8d-101">chatMessage</span><span class="sxs-lookup"><span data-stu-id="a2e8d-101">chatMessage</span></span>

<span data-ttu-id="a2e8d-102">Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="a2e8d-102">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="a2e8d-103">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="a2e8d-103">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="a2e8d-104">Создание подписки завершится сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription).</span><span class="sxs-lookup"><span data-stu-id="a2e8d-104">Subscription creation will fail if [encryptionCertificate](/graph/api/resources/subscription) is not specified.</span></span> <span data-ttu-id="a2e8d-105">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="a2e8d-105">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="a2e8d-106">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="a2e8d-106">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="a2e8d-107">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="a2e8d-107">**Notes:**</span></span> 
>
><span data-ttu-id="a2e8d-108">`/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="a2e8d-108">`/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="a2e8d-109">В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на базе количества данных, доступ к которым получен через API-интерфейс.</span><span class="sxs-lookup"><span data-stu-id="a2e8d-109">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>
>
><span data-ttu-id="a2e8d-110">`/chats/getAllMessages` возвращает только сообщения из чатов, принадлежащих клиенту.</span><span class="sxs-lookup"><span data-stu-id="a2e8d-110">`/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="a2e8d-111">Если цепочка чата инициирована пользователем из-за пределов клиента, она не принадлежит клиенту и для нее не создаются уведомления об изменениях.</span><span class="sxs-lookup"><span data-stu-id="a2e8d-111">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>
