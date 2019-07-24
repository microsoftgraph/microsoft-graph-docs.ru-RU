---
title: Локальные профили публикации
description: Различные службы Azure (например, Азуе, сквозная проверка подлинности подключения Active Directory, подготовка пользователей к работе в Azure AD) разрешает условный доступ к различным локальным ресурсам извне корпоративной сети.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b0e975d932226adfa2c455baaa396c1d580f6ff
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841334"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="e038f-103">Локальные профили публикации</span><span class="sxs-lookup"><span data-stu-id="e038f-103">On-premises publishing profiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e038f-104">Различные службы Azure (например, Азуе, сквозная проверка подлинности подключения Active Directory, подготовка пользователей к работе в Azure AD) разрешает условный доступ к различным локальным ресурсам извне корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="e038f-104">Various Azure services (for example, Azue Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="e038f-105">[Локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному опубликованному ресурсу или [](publishedresource.md)обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="e038f-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="e038f-106">[Группы агентов](onpremisesagentgroup.md) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e038f-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="e038f-107">Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе.</span><span class="sxs-lookup"><span data-stu-id="e038f-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="e038f-108">Весь набор сущностей одного локального типа публикации представлен [онпремисеспублишингпрофиле](onpremisespublishingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e038f-108">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="e038f-109">Администратор клиента может настраивать для каждого **онпремисеспублишингпрофиле** [периода времени](updatewindow.md) , в течение которого агенты могут получать обновления или закладывать обновления для агентов.</span><span class="sxs-lookup"><span data-stu-id="e038f-109">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="e038f-110">[Конфигурация обновления](hybridagentupdaterconfiguration.md) , указанная для **онпремисеспублишингпрофиле** , относится ко всем агентам в **онпремисеспублишингпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="e038f-110">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="e038f-111">См. также</span><span class="sxs-lookup"><span data-stu-id="e038f-111">See also</span></span>

- [<span data-ttu-id="e038f-112">Локальный агент</span><span class="sxs-lookup"><span data-stu-id="e038f-112">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="e038f-113">Локальная группа агентов</span><span class="sxs-lookup"><span data-stu-id="e038f-113">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="e038f-114">Профиль локальной публикации</span><span class="sxs-lookup"><span data-stu-id="e038f-114">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="e038f-115">Опубликованный ресурс</span><span class="sxs-lookup"><span data-stu-id="e038f-115">Published resource</span></span>](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
