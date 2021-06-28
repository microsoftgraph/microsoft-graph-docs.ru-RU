---
title: Обзор доступа к сведениям о работоспособности и взаимодействии служб с помощью Microsoft Graph
description: Используйте API взаимодействия служб в Microsoft Graph для доступа к состоянию работоспособности и записям центра сообщений об облачных службах (Майкрософт).
author: payiAzure
localization_priority: Priority
ms.prod: service-communications
ms.custom: scenarios:getting-started
ms.openlocfilehash: f10aabbdbdb7028af3f16058a6137bd9da8615d6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109009"
---
# <a name="overview-for-accessing-service-health-and-communications-in-microsoft-graph"></a><span data-ttu-id="1eb4e-103">Обзор доступа к сведениям о работоспособности и взаимодействии служб в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1eb4e-103">Overview for accessing service health and communications in Microsoft Graph</span></span>
<span data-ttu-id="1eb4e-104">Вы можете использовать API взаимодействия служб в Microsoft Graph для доступа к состоянию работоспособности и записям центра сообщений об облачных службах (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="1eb4e-104">You can use the service communications API in Microsoft Graph to access the health status and message center posts about Microsoft cloud services.</span></span> <span data-ttu-id="1eb4e-105">Фактическое состояние работоспособности и записи соответствуют службам Microsoft 365 и Dynamics 365, которые поддерживаются API-интерфейсом и подписка на которые есть у клиента.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-105">The actual health status and posts correspond to the Microsoft 365 and Dynamics 365 services that are supported by the API and subscribed by the tenant.</span></span>

## <a name="why-integrate-with-service-health-and-communications-data"></a><span data-ttu-id="1eb4e-106">Зачем интегрировать данные о работоспособности и взаимодействии служб?</span><span class="sxs-lookup"><span data-stu-id="1eb4e-106">Why integrate with service health and communications data?</span></span>

### <a name="get-service-health-and-message-center-posts-for-a-tenant"></a><span data-ttu-id="1eb4e-107">Получение сведений о работоспособности служб и записей центра сообщений для клиента</span><span class="sxs-lookup"><span data-stu-id="1eb4e-107">Get service health and message center posts for a tenant</span></span>
<span data-ttu-id="1eb4e-108">Клиенты могут получать текущие или исторические данные о работоспособности поддерживаемых служб Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-108">Customers can get current or historical health data of supported Microsoft services.</span></span> <span data-ttu-id="1eb4e-109">При возникновении проблем со службой Майкрософт они могут проверить ее состояние работоспособности, чтобы узнать, идентифицирована ли проблема и выполняется ли работа по ее решению, прежде чем звонить в службу поддержки или тратить время на устранение неполадок.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-109">When experiencing problems with a Microsoft service, they can check its health status to verify if an issue has been identified with a resolution in progress, before calling for support or spending time troubleshooting.</span></span> 

<span data-ttu-id="1eb4e-110">Клиенты могут регулярно проверять записи в центре сообщений, чтобы отслеживать ожидаемые новые функции и обновления, а также другие важные объявления.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-110">Customers can regularly review message center posts to keep track of upcoming new features and updates, and other important announcements.</span></span> <span data-ttu-id="1eb4e-111">Благодаря этому они могут предвидеть, как эти изменения повлияют на пользователей, и подготовить соответствующий план действий.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-111">They can then anticipate how these changes may affect users and plan accordingly.</span></span>

### <a name="integrate-service-communications-data-into-custom-workflows"></a><span data-ttu-id="1eb4e-112">Интеграция данных о взаимодействии служб в пользовательские рабочие процессы</span><span class="sxs-lookup"><span data-stu-id="1eb4e-112">Integrate service communications data into custom workflows</span></span>
<span data-ttu-id="1eb4e-113">Разработчики приложений могут интегрировать сведения об активных проблемах с работоспособностью служб в пользовательские приложения, позволяя администраторам рассматривать и делиться сведениями о состоянии с затронутой аудиторией.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-113">App developers can integrate active service health issues directly into custom applications, allowing administrators to triage and share status information with impacted audiences.</span></span>

<span data-ttu-id="1eb4e-114">Приложения могут поддерживать пользовательские рабочие процессы для администраторов с целью проверки, назначения и рассмотрения сообщений об изменениях в центре сообщений.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-114">Apps can enable custom workflows for administrators to review, assign, and triage change communications from the message center.</span></span>

### <a name="build-customer-facing-dashboards"></a><span data-ttu-id="1eb4e-115">Создание панелей мониторинга для клиентов</span><span class="sxs-lookup"><span data-stu-id="1eb4e-115">Build customer-facing dashboards</span></span>

<span data-ttu-id="1eb4e-116">Создавайте приложения с панелями мониторинга для клиентов, чтобы отображать работоспособность служб Майкрософт и позволить клиентам отслеживать предстоящие изменения и другие важные объявления о службах.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-116">Create applications with customer-facing dashboards to show the health of Microsoft services, and let customers keep track of upcoming changes and other important announcements about the services.</span></span>


## <a name="dashboards-examples-in-microsoft-365-admin-center"></a><span data-ttu-id="1eb4e-117">Примеры панелей мониторинга в Центре администрирования Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="1eb4e-117">Dashboards examples in Microsoft 365 admin center</span></span>
<span data-ttu-id="1eb4e-118">В этом разделе показаны примеры в [Центре администрирования Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage), который использует API взаимодействия служб для создания соответствующих панелей мониторинга о работоспособности.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-118">This section shows examples in the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/homepage) that uses the service communications API to build respective health dashboards.</span></span> <span data-ttu-id="1eb4e-119">Войдите в Центр администрирования с помощью учетной записи администратора и щелкните **Работоспособность**, чтобы увидеть следующие панели мониторинга.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-119">Sign in to the admin center with an admin account, then click **Health** to see the following dashboards:</span></span>
- [<span data-ttu-id="1eb4e-120">Работоспособность служб</span><span class="sxs-lookup"><span data-stu-id="1eb4e-120">Service health</span></span>](#service-health-dashboard)
- [<span data-ttu-id="1eb4e-121">Работоспособность выпуска Windows</span><span class="sxs-lookup"><span data-stu-id="1eb4e-121">Windows release health</span></span>](#windows-release-health-dashboard)
- [<span data-ttu-id="1eb4e-122">Центр сообщений</span><span class="sxs-lookup"><span data-stu-id="1eb4e-122">Message center</span></span>](#message-center-dashboard)

### <a name="service-health-dashboard"></a><span data-ttu-id="1eb4e-123">Панель мониторинга работоспособности служб</span><span class="sxs-lookup"><span data-stu-id="1eb4e-123">Service health dashboard</span></span>

<span data-ttu-id="1eb4e-124">На панели мониторинга **Работоспособность служб** можно просмотреть работоспособность служб Майкрософт, на которые у вас есть подписка. К ним могут относиться Office в Интернете, Yammer, Microsoft Dynamics CRM и облачные службы управления мобильными устройствами.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-124">From the **Service health** dashboad, you can view the health of your subscribed Microsoft services, which can include Office on the web, Yammer, Microsoft Dynamics CRM, and mobile device management cloud services.</span></span> <span data-ttu-id="1eb4e-125">См. примеры, показанные на рис. 1.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-125">See examples as demarcated in figure 1.</span></span>

<span data-ttu-id="1eb4e-126">**Рис. 1. Панель мониторинга работоспособности служб в Центре администрирования Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="1eb4e-126">**Figure 1. Service health dashboard in Microsoft 365 admin center**</span></span>

![Снимок экрана: панель мониторинга работоспособности служб для пользователя в Центре администрирования Microsoft 365](images/service-communications-concept-overview-admin-center-serviceHealth2.png)

### <a name="windows-release-health-dashboard"></a><span data-ttu-id="1eb4e-128">Панель мониторинга работоспособности выпуска Windows</span><span class="sxs-lookup"><span data-stu-id="1eb4e-128">Windows release health dashboard</span></span>

<span data-ttu-id="1eb4e-129">На панели мониторинга **Работоспособность выпуска Windows** можно просмотреть важную информацию о ежемесячных исправлениях и обновлениях компонентов, а также о новейшие функции и улучшения для Windows.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-129">From the **Windows release health** dashboad, you can view essential information about monthly quality and feature updates, and the latest features and enhancements for Windows.</span></span> <span data-ttu-id="1eb4e-130">См. пример, показанный на рис. 2.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-130">See an example as demarcated in figure 2.</span></span>

<span data-ttu-id="1eb4e-131">**Рис. 2. Панель мониторинга работоспособности выпуска Windows в Центре администрирования Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="1eb4e-131">**Figure 2. Windows release health dashboard in Microsoft 365 admin center**</span></span>

![Снимок экрана: панель мониторинга работоспособности выпуска Windows для пользователя в Центре администрирования Microsoft 365](images/service-communications-concept-overview-admin-center-windowshealth2.png)


### <a name="message-center-dashboard"></a><span data-ttu-id="1eb4e-133">Панель мониторинга центра сообщений</span><span class="sxs-lookup"><span data-stu-id="1eb4e-133">Message center dashboard</span></span>
<span data-ttu-id="1eb4e-134">На панели мониторинга **Центр сообщений** вы можете просматривать предстоящие изменения, в том числе новые и измененные компоненты, запланированное обслуживание и другие важные объявления.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-134">From the **Message center** dashboad, you can view upcoming changes, including new and changed features, planned maintenance, and other important announcements.</span></span> <span data-ttu-id="1eb4e-135">См. примеры, показанные на рис. 3.</span><span class="sxs-lookup"><span data-stu-id="1eb4e-135">See examples as demarcated in figure 3.</span></span>

<span data-ttu-id="1eb4e-136">**Рис. 3. Панель мониторинга центра сообщений в Центре администрирования Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="1eb4e-136">**Figure 3. Message center dashboard in Microsoft 365 admin center**</span></span>

![Снимок экрана: панель мониторинга центра сообщений для пользователя в Центре администрирования Microsoft 365](images/service-communications-concept-overview-admin-center-messagecenter2.png)



## <a name="next-steps"></a><span data-ttu-id="1eb4e-138">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1eb4e-138">Next steps</span></span>

- <span data-ttu-id="1eb4e-139">Попробуйте примеры запросов взаимодействия служб в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer/?request=admin%2FserviceAnnouncement%2FhealthOverviews&version=beta).</span><span class="sxs-lookup"><span data-stu-id="1eb4e-139">Try service communications sample queries in [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=admin%2FserviceAnnouncement%2FhealthOverviews&version=beta).</span></span>

- <span data-ttu-id="1eb4e-140">Узнайте больше об [API взаимодействия служб](/graph/api/resources/service-communications-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="1eb4e-140">Learn more about the [service communications API](/graph/api/resources/service-communications-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>