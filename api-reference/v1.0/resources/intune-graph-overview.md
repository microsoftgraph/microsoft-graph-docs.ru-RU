---
title: Использование API Graph для Intune
description: " Гибридные развертывания Intune не поддерживаются. "
author: dougeby
localization_priority: Priority
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 6b84f59cd18b6e6a5d7bd1ca776c71812fa772b0
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353513"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="b7cd7-103">Работа с Intune в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7cd7-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="b7cd7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="b7cd7-105">API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="b7cd7-106">В сценариях управления мобильными устройствами (MDM) API Microsoft Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="b7cd7-107">Использование API Microsoft Graph для Intune</span><span class="sxs-lookup"><span data-stu-id="b7cd7-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="b7cd7-108">Intune предоставляет данные интерфейсу API Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="b7cd7-109"> API Microsoft Graph используется для объединения сведений из других служб и Intune, чтобы создавать функциональные приложения, работающие с несколькими службами, для ИТ-специалистов или пользователей.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-109"> Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="b7cd7-110">В приведенном ниже примере показано, как определить, установлено ли приложение на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="b7cd7-111">Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя:</span><span class="sxs-lookup"><span data-stu-id="b7cd7-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="b7cd7-112">Затем просмотрите список приложений для вашего клиента:</span><span class="sxs-lookup"><span data-stu-id="b7cd7-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="b7cd7-113">На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):</span><span class="sxs-lookup"><span data-stu-id="b7cd7-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="b7cd7-114">Доступ к API Microsoft Graph для Intune</span><span class="sxs-lookup"><span data-stu-id="b7cd7-114">Accessing the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="b7cd7-115">Intune поддерживает как [делегированные разрешения](https://docs.microsoft.com/graph/auth-v2-user), так и [разрешения приложений](https://docs.microsoft.com/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="b7cd7-115">Intune supports both [delegated permissions](https://docs.microsoft.com/graph/auth-v2-user) and [application permissions](https://docs.microsoft.com/graph/auth-v2-service).</span></span> <span data-ttu-id="b7cd7-116">Делегированные разрешения и разрешения приложений поддерживают операции как чтения, так и записи.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-116">Delegated and application permissions support both read and write operations.</span></span> <span data-ttu-id="b7cd7-117">Разрешения приложений и делегированные разрешения поддерживает как однотенантные, так и многотенантные приложения.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-117">Delegated and application permissions support both single tenant applications, as well as multi-tenant applications.</span></span> <span data-ttu-id="b7cd7-118">Дополнительные сведения о разрешениях, доступных в Microsoft Graph, см. в [справочнике по разрешениям Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7cd7-118">For more information about the permissions available through Microsoft Graph, see [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span>

## <a name="using-permissions"></a><span data-ttu-id="b7cd7-119">Использование разрешений</span><span class="sxs-lookup"><span data-stu-id="b7cd7-119">Using permissions</span></span>

<span data-ttu-id="b7cd7-120">API Microsoft Graph контролирует доступ к ресурсам с помощью разрешений.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-120">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="b7cd7-121">Разработчикам необходимо указать разрешения, необходимые для доступа к ресурсам Intune.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-121">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="b7cd7-122">Как правило, разрешения указываются на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-122">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="b7cd7-123">Дополнительные сведения см. в статье [Справочник по разрешениям Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7cd7-123">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span>

## <a name="whats-new"></a><span data-ttu-id="b7cd7-124">Что нового</span><span class="sxs-lookup"><span data-stu-id="b7cd7-124">What's new</span></span>
<span data-ttu-id="b7cd7-125">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-125">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b7cd7-126">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b7cd7-126">Next Steps</span></span>

- <span data-ttu-id="b7cd7-127">Узнайте, [как использовать Azure AD](https://docs.microsoft.com/intune/intune-graph-apis) для доступа к API Microsoft Graph для Intune.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-127">Learn [how to use Azure AD](https://docs.microsoft.com/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="b7cd7-128">Изучите [примеры PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples), демонстрирующие способ использования API Microsoft Graph для Intune в рабочем контексте.</span><span class="sxs-lookup"><span data-stu-id="b7cd7-128">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>




