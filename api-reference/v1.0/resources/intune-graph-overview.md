---
title: Использование API Graph для Intune
description: " Гибридные развертывания Intune не поддерживаются. "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 2dfeb5ff55670f3e11b175e0472359002b09bab6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551814"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="fa634-103">Работа с Intune в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fa634-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="fa634-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/ru-RU/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fa634-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/ru-RU/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="fa634-105">API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.</span><span class="sxs-lookup"><span data-stu-id="fa634-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="fa634-106">В сценариях управления мобильными устройствами (MDM) API Microsoft Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/ru-RU/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="fa634-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/ru-RU/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="fa634-107">Использование API Microsoft Graph для Intune</span><span class="sxs-lookup"><span data-stu-id="fa634-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="fa634-108">Intune предоставляет данные интерфейсу API Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.</span><span class="sxs-lookup"><span data-stu-id="fa634-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="fa634-109"> API Microsoft Graph используется для объединения сведений из других служб и Intune, чтобы создавать функциональные приложения, работающие с несколькими службами, для ИТ-специалистов или пользователей.</span><span class="sxs-lookup"><span data-stu-id="fa634-109">Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="fa634-110">В приведенном ниже примере показано, как определить, установлено ли приложение на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="fa634-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="fa634-111">Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя:</span><span class="sxs-lookup"><span data-stu-id="fa634-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="fa634-112">Затем просмотрите список приложений для вашего клиента:</span><span class="sxs-lookup"><span data-stu-id="fa634-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="fa634-113">На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):</span><span class="sxs-lookup"><span data-stu-id="fa634-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permissions"></a><span data-ttu-id="fa634-114">Использование разрешений</span><span class="sxs-lookup"><span data-stu-id="fa634-114">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="fa634-115">API Microsoft Graph контролирует доступ к ресурсам с помощью разрешений.</span><span class="sxs-lookup"><span data-stu-id="fa634-115">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="fa634-116">Разработчикам необходимо указать разрешения, необходимые для доступа к ресурсам Intune.</span><span class="sxs-lookup"><span data-stu-id="fa634-116">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="fa634-117">Как правило, разрешения указываются на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fa634-117">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="fa634-118">Дополнительные сведения см. в статье [Справочник по разрешениям Microsoft Graph](https://docs.microsoft.com/ru-RU/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa634-118">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/ru-RU/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="fa634-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="fa634-119">Next Steps</span></span>

- <span data-ttu-id="fa634-120">Узнайте, [как использовать Azure AD](https://docs.microsoft.com/ru-RU/intune/intune-graph-apis) для доступа к API Microsoft Graph для Intune.</span><span class="sxs-lookup"><span data-stu-id="fa634-120">Learn [how to use Azure AD](https://docs.microsoft.com/ru-RU/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="fa634-121">Изучите [примеры PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples), демонстрирующие способ использования API Microsoft Graph для Intune в рабочем контексте.</span><span class="sxs-lookup"><span data-stu-id="fa634-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
