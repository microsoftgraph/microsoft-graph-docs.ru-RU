---
title: Microsoft 365 Lighthouse Обзор API
description: Microsoft 365 Lighthouse является порталом администрирования, который помогает управляемым поставщикам услуг (MSP) обеспечивать безопасность устройств, данных и пользователей в масштабе для клиентов малого и среднего бизнеса(SMB), использующих Microsoft 365 бизнес премиум.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
ms.openlocfilehash: 177a2f03fe5ee0e2e7d90ade038dcef1f7d6c3db
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401893"
---
# <a name="overview-for-multi-tenant-management-using-the-microsoft-365-lighthouse-api"></a><span data-ttu-id="1bc29-103">Обзор управления несколькими клиентами с Microsoft 365 Lighthouse API</span><span class="sxs-lookup"><span data-stu-id="1bc29-103">Overview for multi-tenant management using the Microsoft 365 Lighthouse API</span></span>

<span data-ttu-id="1bc29-104">Microsoft 365 Lighthouse является порталом администрирования, который позволяет управляемым поставщикам услуг (MSP) удаленно управлять несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="1bc29-104">Microsoft 365 Lighthouse is an admin portal that lets Managed Service Providers (MSPs) remotely manage multiple customer tenants.</span></span> <span data-ttu-id="1bc29-105">Это помогает msPs обеспечить безопасность устройств, данных и пользователей в масштабе для клиентов малого и среднего бизнеса (SMB), использующих Microsoft 365 бизнес премиум.</span><span class="sxs-lookup"><span data-stu-id="1bc29-105">It helps MSPs secure and manage devices, data, and users at scale for small- and medium-sized business (SMB) customers who are using Microsoft 365 Business Premium.</span></span>

<span data-ttu-id="1bc29-106">Microsoft 365 Lighthouse помогает msPs упростить процесс Microsoft 365 бизнес премиум клиентов.</span><span class="sxs-lookup"><span data-stu-id="1bc29-106">Microsoft 365 Lighthouse helps MSPs simplify onboarding of Microsoft 365 Business Premium customer tenants.</span></span> <span data-ttu-id="1bc29-107">Он предлагает службе MSP удобство представлений с несколькими клиентами во всех средах клиента.</span><span class="sxs-lookup"><span data-stu-id="1bc29-107">It offers an MSP the convenience of multi-tenant views across all its customer tenant environments.</span></span> <span data-ttu-id="1bc29-108">Он может рекомендовать базовые параметры конфигурации безопасности, адаптированные к клиентам SMB MSP.</span><span class="sxs-lookup"><span data-stu-id="1bc29-108">It can recommend security configuration baselines tailored to the MSP's SMB customers.</span></span> <span data-ttu-id="1bc29-109">С Microsoft 365 Lighthouse, msPs может масштабировать управление клиентом клиентов, сосредоточиться на наиболее важных, быстро найти и исследовать риски, а также принять меры, чтобы помочь их клиенты клиентов в здоровом и безопасном состоянии.</span><span class="sxs-lookup"><span data-stu-id="1bc29-109">With Microsoft 365 Lighthouse, MSPs can scale the management of their customer tenants, focus on what's most important, quickly find and investigate risks, and take action to help get their customer tenants to a healthy and secure state.</span></span>

> [!NOTE]  
> <span data-ttu-id="1bc29-110">Эта документация о Microsoft 365 Lighthouse API, доступном в _Microsoft Graph._</span><span class="sxs-lookup"><span data-stu-id="1bc29-110">This documentation is about the Microsoft 365 Lighthouse API available on _Microsoft Graph_.</span></span> <span data-ttu-id="1bc29-111">Аналогичное предложение, Azure Lighthouse, помогает поставщикам услуг предоставлять управляемые службы для служб Azure с помощью комплексного и надежного инструмента управления, встроенного в _платформу Azure._</span><span class="sxs-lookup"><span data-stu-id="1bc29-111">A similar offering, Azure Lighthouse, helps service providers deliver managed services for Azure services by using comprehensive and robust management tooling built into the _Azure_ platform.</span></span> <span data-ttu-id="1bc29-112">Дополнительные дополнительные информации см. [в видеоролике What is Azure Lighthouse.](/azure/lighthouse/overview)</span><span class="sxs-lookup"><span data-stu-id="1bc29-112">To learn more, see [What is Azure Lighthouse](/azure/lighthouse/overview).</span></span>

## <a name="why-integrate-with-microsoft-365-lighthouse"></a><span data-ttu-id="1bc29-113">Зачем интегрироваться с Microsoft 365 Lighthouse?</span><span class="sxs-lookup"><span data-stu-id="1bc29-113">Why integrate with Microsoft 365 Lighthouse?</span></span>

<span data-ttu-id="1bc29-114">В качестве MSP вы можете использовать API Microsoft 365 Lighthouse Microsoft Graph, чтобы получить сведения о выявленных рисках и принять меры, чтобы помочь вашим клиентам в здоровом и безопасном состоянии.</span><span class="sxs-lookup"><span data-stu-id="1bc29-114">As an MSP, you can use the Microsoft 365 Lighthouse API in Microsoft Graph to gain insights into identified risks and take action to help get your customers into a healthy and secure state.</span></span>

### <a name="devices"></a><span data-ttu-id="1bc29-115">Устройства</span><span class="sxs-lookup"><span data-stu-id="1bc29-115">Devices</span></span>

<span data-ttu-id="1bc29-116">API Маяка можно использовать для выполнения следующих задач устройства:</span><span class="sxs-lookup"><span data-stu-id="1bc29-116">You can use the Lighthouse API to perform the following device tasks:</span></span>

- <span data-ttu-id="1bc29-117">Анализ [тенденций соответствия](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) требованиям устройств, чтобы лучше понять, как со временем развивается соответствие требованиям к устройствам для клиентов.</span><span class="sxs-lookup"><span data-stu-id="1bc29-117">Analyze [device compliance trends](/graph/api/resources/managedtenants-manageddevicecompliancetrend?view=graph-rest-beta&preserve-view=true) to better understand how device compliance is evolving over time for your customers.</span></span>
- <span data-ttu-id="1bc29-118">Поймите, [какие политики](/graph/api/resources/managedtenants-manageddevicecompliance) соответствия требованиям к устройствам были созданы для ваших клиентов, и состояние политик.</span><span class="sxs-lookup"><span data-stu-id="1bc29-118">Understand what [device compliance policies](/graph/api/resources/managedtenants-manageddevicecompliance) have been created across your customers and the status of the policies.</span></span>

### <a name="threat-management"></a><span data-ttu-id="1bc29-119">Управление угрозами</span><span class="sxs-lookup"><span data-stu-id="1bc29-119">Threat management</span></span>

<span data-ttu-id="1bc29-120">API Маяка можно использовать для выполнения следующих задач по управлению угрозами:</span><span class="sxs-lookup"><span data-stu-id="1bc29-120">You can use the Lighthouse API to perform the following threat management tasks:</span></span>

- <span data-ttu-id="1bc29-121">Сведения о состоянии [вредоносных](/graph/api/resources/managedtenants-windowsdevicemalwarestate) программ, которые присутствуют на Windows устройствах, зарегистрированных для управления клиентами.</span><span class="sxs-lookup"><span data-stu-id="1bc29-121">Gain insight to the state of [malware](/graph/api/resources/managedtenants-windowsdevicemalwarestate) that is present on the Windows devices registered for management across your customers.</span></span>
- <span data-ttu-id="1bc29-122">Просмотр состояния [защиты](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) для Windows устройств, зарегистрированных для управления в клиентах, чтобы убедиться, что Защитник Windows находятся в нормальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="1bc29-122">View the [protection state](/graph/api/resources/managedtenants-windowsprotectionstate?view=graph-rest-beta&preserve-view=true) for Windows devices registered for management across your customers to ensure those using Windows Defender are in a healthy state.</span></span>

### <a name="users"></a><span data-ttu-id="1bc29-123">Пользователи</span><span class="sxs-lookup"><span data-stu-id="1bc29-123">Users</span></span>

<span data-ttu-id="1bc29-124">API Маяка можно использовать для выполнения следующих пользовательских задач:</span><span class="sxs-lookup"><span data-stu-id="1bc29-124">You can use the Lighthouse API to perform the following user tasks:</span></span>

- <span data-ttu-id="1bc29-125">Откройте [для себя рискованных пользователей](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) в ваших клиентах.</span><span class="sxs-lookup"><span data-stu-id="1bc29-125">Discover [risky users](/graph/api/resources/managedtenants-riskyuser?view=graph-rest-beta&preserve-view=true) across your customers.</span></span>
- <span data-ttu-id="1bc29-126">Просмотреть [сводку](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) регистрации пользователей учетных данных, чтобы понять, какие пользователи в ваших клиентах зарегистрировались для многофакторной проверки подлинности и сброса пароля самообслуживления.</span><span class="sxs-lookup"><span data-stu-id="1bc29-126">View [credential user registration summary](/graph/api/resources/managedtenants-credentialuserregistrationssummary?view=graph-rest-beta&preserve-view=true) to understand what users across your customers have registered for multi-factor authentication and self-service password reset.</span></span>

## <a name="api-reference"></a><span data-ttu-id="1bc29-127">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="1bc29-127">API reference</span></span>

<span data-ttu-id="1bc29-128">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="1bc29-128">Looking for the API reference for this service?</span></span>

<span data-ttu-id="1bc29-129">См. [Microsoft 365 Lighthouse API в Microsoft Graph (предварительный просмотр).](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1bc29-129">See [Microsoft 365 Lighthouse API in Microsoft Graph (preview)](/graph/api/resources/managedtenants-managedtenant?view=graph-rest-beta&preserve-view=true).</span></span>

> [!NOTE]
> <span data-ttu-id="1bc29-130">API Microsoft 365 Lighthouse определяется в поднаемной области OData. `microsoft.graph.managedTenants`</span><span class="sxs-lookup"><span data-stu-id="1bc29-130">The Microsoft 365 Lighthouse API is defined in the OData subnamespace, `microsoft.graph.managedTenants`.</span></span>


## <a name="next-steps"></a><span data-ttu-id="1bc29-131">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1bc29-131">Next steps</span></span>

- <span data-ttu-id="1bc29-132">Узнайте больше о [портале Microsoft 365 Lighthouse.](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1bc29-132">Learn more about the [Microsoft 365 Lighthouse](/microsoft-365/lighthouse/m365-lighthouse-overview?view=o365-worldwide&preserve-view=true) portal.</span></span>
- <span data-ttu-id="1bc29-133">Узнайте о [последних новых функций](/graph/whats-new-overview) и обновлениях API Маяка.</span><span class="sxs-lookup"><span data-stu-id="1bc29-133">Find out about the [latest new features and updates](/graph/whats-new-overview) for the Lighthouse API.</span></span>
- <span data-ttu-id="1bc29-134">Изучите [примеры](https://developer.microsoft.com/graph/graph/examples), чтобы получить более четкое представление об использовании Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1bc29-134">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
