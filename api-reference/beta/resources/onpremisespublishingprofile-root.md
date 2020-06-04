---
title: Локальные профили публикации
description: Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3774ceb0a2e03b8c625bf317467c670c93596ac9
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556242"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="cdbf3-103">Локальные профили публикации</span><span class="sxs-lookup"><span data-stu-id="cdbf3-103">On-premises publishing profiles</span></span>

<span data-ttu-id="cdbf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdbf3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdbf3-105">Различные службы Azure (например, [сквозная проверка подлинности](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)подключения Azure Active Directory, подключение [рабочего дня к пользователям Azure AD](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)и [прокси приложения](https://aka.ms/whyappproxy) — предоставление доступа к различным локальным ресурсам извне корпоративной сети).</span><span class="sxs-lookup"><span data-stu-id="cdbf3-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="cdbf3-106">[Локальные агенты](onpremisesagent.md) (или [соединители](connector.md) для прокси-сервера приложения), установленные администратором клиента, можно настроить на маршрутизацию запросов к определенному [опубликованному ресурсу](publishedresource.md).</span><span class="sxs-lookup"><span data-stu-id="cdbf3-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="cdbf3-107">[Группы агентов](onpremisesagentgroup.md) (или [группы соединителей](connectorgroup.md) для прокси приложения) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="cdbf3-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="cdbf3-108">Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе.</span><span class="sxs-lookup"><span data-stu-id="cdbf3-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="cdbf3-109">Весь набор сущностей одного локального типа публикации представлен [онпремисеспублишингпрофиле](onpremisespublishingprofile.md).</span><span class="sxs-lookup"><span data-stu-id="cdbf3-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="cdbf3-110">Администратор клиента может настраивать для каждого **онпремисеспублишингпрофиле** [периода времени](updatewindow.md) , в течение которого агенты могут получать обновления или закладывать обновления для агентов.</span><span class="sxs-lookup"><span data-stu-id="cdbf3-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="cdbf3-111">[Конфигурация обновления](hybridagentupdaterconfiguration.md) , указанная для **онпремисеспублишингпрофиле** , относится ко всем агентам в **онпремисеспублишингпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="cdbf3-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

## <a name="see-also"></a><span data-ttu-id="cdbf3-112">См. также</span><span class="sxs-lookup"><span data-stu-id="cdbf3-112">See also</span></span>

- [<span data-ttu-id="cdbf3-113">Локальный агент</span><span class="sxs-lookup"><span data-stu-id="cdbf3-113">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="cdbf3-114">Локальная группа агентов</span><span class="sxs-lookup"><span data-stu-id="cdbf3-114">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="cdbf3-115">Профиль локальной публикации</span><span class="sxs-lookup"><span data-stu-id="cdbf3-115">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="cdbf3-116">Опубликованный ресурс</span><span class="sxs-lookup"><span data-stu-id="cdbf3-116">Published resource</span></span>](publishedresource.md)
- [<span data-ttu-id="cdbf3-117">Connector</span><span class="sxs-lookup"><span data-stu-id="cdbf3-117">Connector</span></span>](connector.md)
- [<span data-ttu-id="cdbf3-118">Группа соединителей</span><span class="sxs-lookup"><span data-stu-id="cdbf3-118">Connector group</span></span>](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
