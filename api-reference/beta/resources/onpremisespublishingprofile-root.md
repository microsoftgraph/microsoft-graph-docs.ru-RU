---
title: Профили локальной публикации
description: Различные службы Azure (например, azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) позволяют получить условный доступ к различным ресурсам из-за пределов корпоративной сети.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 44d09da274413b23092afea6290c0c32a64f8500
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134878"
---
# <a name="on-premises-publishing-profiles"></a><span data-ttu-id="0f33b-103">Профили локальной публикации</span><span class="sxs-lookup"><span data-stu-id="0f33b-103">On-premises publishing profiles</span></span>

<span data-ttu-id="0f33b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f33b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f33b-105">Различные службы Azure (например, azure Active Directory Connect [Passthrough Authentication,](/azure/active-directory/hybrid/how-to-connect-pta) [Workday to Azure AD users provisioning,](/azure/active-directory/saas-apps/workday-inbound-tutorial)and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network.</span><span class="sxs-lookup"><span data-stu-id="0f33b-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy)  allow access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="0f33b-106">[Локально установленные](onpremisesagent.md) администратором [](connector.md) клиента агенты (или соединители для прокси приложения) могут быть настроены для маршрутов запросов на [определенный опубликованный ресурс.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="0f33b-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by a tenant administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="0f33b-107">[Группы агентов](onpremisesagentgroup.md) (или группы [соединителок](connectorgroup.md) для прокси приложения) позволяют администратору клиента назначать определенных агентов для обслуживания определенных опубликованных локального ресурса.</span><span class="sxs-lookup"><span data-stu-id="0f33b-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="0f33b-108">Администраторы клиента могут сгруппить несколько агентов, а затем назначить каждый опубликованный ресурс группе.</span><span class="sxs-lookup"><span data-stu-id="0f33b-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="0f33b-109">Весь набор сущностями того же локального типа публикации представлен [onPremisesPublishingProfile.](onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0f33b-109">The entire set of entities of the same on-premises publishing type is represented by [onPremisesPublishingProfile](onpremisespublishingprofile.md).</span></span>

<span data-ttu-id="0f33b-110">Администратор клиента может настроить для каждого **onPremisesPublishingProfile** период времени, в течение которого агенты могут получать обновления или откладывать обновления для агентов. [](updatewindow.md)</span><span class="sxs-lookup"><span data-stu-id="0f33b-110">A tenant admin can configure for each **onPremisesPublishingProfile** the [time window](updatewindow.md) during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="0f33b-111">Конфигурация [средства](hybridagentupdaterconfiguration.md) обновления, указанная для **onPremisesPublishingProfile,** применима ко всем агентам в **этом onPremisesPublishingProfile.**</span><span class="sxs-lookup"><span data-stu-id="0f33b-111">The [updater configuration](hybridagentupdaterconfiguration.md) specified for an **onPremisesPublishingProfile** is applicable to all the agents within that **onPremisesPublishingProfile**.</span></span>

<span data-ttu-id="0f33b-112">Руководство по настройке прокси приложения см. в руководстве по автоматизации настройки прокси приложения [с помощью API Microsoft Graph.](/graph/application-proxy-configure-api)</span><span class="sxs-lookup"><span data-stu-id="0f33b-112">For a tutorial about configuring Application Proxy, see [Automate the configuration of Application Proxy using the Microsoft Graph API](/graph/application-proxy-configure-api).</span></span>

## <a name="see-also"></a><span data-ttu-id="0f33b-113">См. также</span><span class="sxs-lookup"><span data-stu-id="0f33b-113">See also</span></span>

- [<span data-ttu-id="0f33b-114">Локальное агент</span><span class="sxs-lookup"><span data-stu-id="0f33b-114">On-premises agent</span></span>](onpremisesagent.md)
- [<span data-ttu-id="0f33b-115">Группа локального агента</span><span class="sxs-lookup"><span data-stu-id="0f33b-115">On-premises agent group</span></span>](onpremisesagentgroup.md)
- [<span data-ttu-id="0f33b-116">Профиль локальной публикации</span><span class="sxs-lookup"><span data-stu-id="0f33b-116">On-premises publishing profile</span></span>](onpremisespublishingprofile.md)
- [<span data-ttu-id="0f33b-117">Опубликованный ресурс</span><span class="sxs-lookup"><span data-stu-id="0f33b-117">Published resource</span></span>](publishedresource.md)
- [<span data-ttu-id="0f33b-118">Connector</span><span class="sxs-lookup"><span data-stu-id="0f33b-118">Connector</span></span>](connector.md)
- [<span data-ttu-id="0f33b-119">Группа соединители</span><span class="sxs-lookup"><span data-stu-id="0f33b-119">Connector group</span></span>](connectorgroup.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



