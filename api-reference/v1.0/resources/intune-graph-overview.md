---
title: Использование API Graph для Intune
description: " Гибридные развертывания Intune не поддерживаются. "
ms.openlocfilehash: 23f6550fca708b64357b7b5132a2a42060cfa4bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024369"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="c87d6-103">Работа с Intune в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c87d6-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="c87d6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c87d6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="c87d6-105">API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.</span><span class="sxs-lookup"><span data-stu-id="c87d6-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="c87d6-106">В сценариях управления мобильными устройствами (MDM) API Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c87d6-106">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="c87d6-107">Использование API Graph для Intune</span><span class="sxs-lookup"><span data-stu-id="c87d6-107">Using the Intune Graph API</span></span>

<span data-ttu-id="c87d6-108">Intune предоставляет данные интерфейсу API Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.</span><span class="sxs-lookup"><span data-stu-id="c87d6-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="c87d6-109">С помощью API Microsoft Graph вы можете объединить данные из других служб и Intune, чтобы создать используемых в разных службах полнофункциональные приложения для ИТ-специалистов и пользователей.</span><span class="sxs-lookup"><span data-stu-id="c87d6-109">  Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="c87d6-110">Ниже приведен пример того, как определить, установлено ли приложение на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="c87d6-110">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="c87d6-111">Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя:</span><span class="sxs-lookup"><span data-stu-id="c87d6-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="c87d6-112">Затем просмотрите список приложений для вашего клиента:</span><span class="sxs-lookup"><span data-stu-id="c87d6-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="c87d6-113">На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):</span><span class="sxs-lookup"><span data-stu-id="c87d6-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a><span data-ttu-id="c87d6-114">Использование областей разрешений</span><span class="sxs-lookup"><span data-stu-id="c87d6-114">Using permission scopes</span></span>

<span data-ttu-id="c87d6-115">API Microsoft Graph управляет доступом к ресурсам, используя области разрешений.</span><span class="sxs-lookup"><span data-stu-id="c87d6-115">Microsoft Graph API controls access to resources using permission scopes.</span></span> <span data-ttu-id="c87d6-116">Разработчикам необходимо указать области разрешений, необходимые для доступа к ресурсам Intune.</span><span class="sxs-lookup"><span data-stu-id="c87d6-116">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="c87d6-117">Как правило, требуемые области разрешений указываются на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c87d6-117">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="c87d6-118">Дополнительные сведения см. в статье об [областях разрешений в Microsoft Graph](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) и [областях разрешений в Intune](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span><span class="sxs-lookup"><span data-stu-id="c87d6-118">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="next-steps"></a><span data-ttu-id="c87d6-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c87d6-119">Next Steps</span></span>

- <span data-ttu-id="c87d6-120">Узнайте, [как использовать Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) для доступа к Microsoft Graph API для Intune.</span><span class="sxs-lookup"><span data-stu-id="c87d6-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="c87d6-121">Изучите [Примеры PowerShell Intune](https://github.com/microsoftgraph/powershell-intune-samples), которой показано, как использовать API график для Intune в контексте рабочие примеры.</span><span class="sxs-lookup"><span data-stu-id="c87d6-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use Graph API for Intune in context of working examples.</span></span>