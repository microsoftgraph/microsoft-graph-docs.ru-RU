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

### <a name="chatmessage"></a><span data-ttu-id="f930a-101">chatMessage</span><span class="sxs-lookup"><span data-stu-id="f930a-101">chatMessage</span></span>

<span data-ttu-id="f930a-102">Подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурса (**includeResourceData** должен иметь значение `false`) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="f930a-102">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="f930a-103">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="f930a-103">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="f930a-104">Создание подписки завершится сбоем, если не указан [encryptionCertificate](/graph/api/resources/subscription).</span><span class="sxs-lookup"><span data-stu-id="f930a-104">Subscription creation will fail if [encryptionCertificate](/graph/api/resources/subscription) is not specified.</span></span> <span data-ttu-id="f930a-105">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="f930a-105">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="f930a-106">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="f930a-106">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="f930a-107">**Примечания.**</span><span class="sxs-lookup"><span data-stu-id="f930a-107">**Notes:**</span></span> 
>
><span data-ttu-id="f930a-p102">`/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses). В дальнейшем корпорация Майкрософт может потребовать у вас или ваших клиентов оплаты дополнительных сборов на основе количества данных, доступ к которым получен через API-интерфейс.</span><span class="sxs-lookup"><span data-stu-id="f930a-p102">`/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses). In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>
