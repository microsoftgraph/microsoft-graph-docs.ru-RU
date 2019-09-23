---
title: Локальные профили публикации
description: Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 73fbd77064f434b93b3dca91d3bc28d5b4101aba
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113916"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="2af25-103">Локальные профили публикации</span><span class="sxs-lookup"><span data-stu-id="2af25-103">On-premises publishing profiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2af25-104">Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="2af25-104">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="2af25-105">[Локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="2af25-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="2af25-106">[Группы агентов](onpremisesagentgroup.md) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="2af25-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="2af25-107">Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе.</span><span class="sxs-lookup"><span data-stu-id="2af25-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="2af25-108">Весь набор сущностей одного локального типа публикации представлен [онпремисеспублишингпрофиле](onpremisespublishingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2af25-108">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="2af25-109">Администратор клиента может настраивать для каждого **онпремисеспублишингпрофиле** [периода времени](updatewindow.md) , в течение которого агенты могут получать обновления или закладывать обновления для агентов.</span><span class="sxs-lookup"><span data-stu-id="2af25-109">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="2af25-110">[Конфигурация обновления](hybridagentupdaterconfiguration.md) , указанная для **онпремисеспублишингпрофиле** , относится ко всем агентам в **онпремисеспублишингпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="2af25-110">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="2af25-111">См. также</span><span class="sxs-lookup"><span data-stu-id="2af25-111">See also</span></span>

- [<span data-ttu-id="2af25-112">Локальный агент</span><span class="sxs-lookup"><span data-stu-id="2af25-112">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="2af25-113">Локальная группа агентов</span><span class="sxs-lookup"><span data-stu-id="2af25-113">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="2af25-114">Профиль локальной публикации</span><span class="sxs-lookup"><span data-stu-id="2af25-114">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="2af25-115">Опубликованный ресурс</span><span class="sxs-lookup"><span data-stu-id="2af25-115">Published resource</span></span>](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
