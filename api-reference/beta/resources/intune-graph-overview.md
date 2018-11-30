---
title: Использование API Graph для Intune
description: " Гибридные развертывания Intune не поддерживаются. "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079653"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="df1e0-103">Работа с Intune в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df1e0-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="df1e0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="df1e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df1e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df1e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df1e0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="df1e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="df1e0-107">API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.</span><span class="sxs-lookup"><span data-stu-id="df1e0-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="df1e0-108">В сценариях управления мобильными устройствами (MDM) API Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="df1e0-108">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="df1e0-109">Использование API Graph для Intune</span><span class="sxs-lookup"><span data-stu-id="df1e0-109">Using the Intune Graph API</span></span>

<span data-ttu-id="df1e0-110">Intune предоставляет данные в Microsoft Graph так же, как прочие облачные службы, с расширенными возможностями сущности сведения и отношения навигации.</span><span class="sxs-lookup"><span data-stu-id="df1e0-110">Intune provides data into the Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="df1e0-111">Используйте Microsoft Graph для объединения данных из других служб и Intune создавать полнофункциональный приложения кросс service для ИТ-специалистов и конечных пользователей.</span><span class="sxs-lookup"><span data-stu-id="df1e0-111">  Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="df1e0-112">Ниже приведен пример того, как определить, установлено ли приложение на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="df1e0-112">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="df1e0-113">Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя:</span><span class="sxs-lookup"><span data-stu-id="df1e0-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="df1e0-114">Затем просмотрите список приложений для вашего клиента:</span><span class="sxs-lookup"><span data-stu-id="df1e0-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="df1e0-115">На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):</span><span class="sxs-lookup"><span data-stu-id="df1e0-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a><span data-ttu-id="df1e0-116">С помощью области разрешений график</span><span class="sxs-lookup"><span data-stu-id="df1e0-116">Using Graph permission scopes</span></span>

<span data-ttu-id="df1e0-117">Графическое представление корпорацию Майкрософт управляет доступом к ресурсам, с помощью области разрешений.</span><span class="sxs-lookup"><span data-stu-id="df1e0-117">Microsof Graph controls access to resources using permission scopes.</span></span> <span data-ttu-id="df1e0-118">Разработчикам необходимо указать области разрешений, необходимые для доступа к ресурсам Intune.</span><span class="sxs-lookup"><span data-stu-id="df1e0-118">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="df1e0-119">Как правило, требуемые области разрешений указываются на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="df1e0-119">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="df1e0-120">Дополнительные сведения см. в статье об [областях разрешений в Microsoft Graph](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) и [областях разрешений в Intune](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span><span class="sxs-lookup"><span data-stu-id="df1e0-120">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a><span data-ttu-id="df1e0-121">Чтобы использовать содержания на сайте Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="df1e0-121">To use the Table of Contents on the Microsoft Graph site</span></span>
  
<span data-ttu-id="df1e0-122">Поиск частей документацию по API графике Intune и ресурсов, чтобы увидеть могут просматривать содержание (в левой панели веб-сайта).</span><span class="sxs-lookup"><span data-stu-id="df1e0-122">You can browse the Table of Contents (in the left pane of the site) to find the parts of the Intune Graph API and resource documentation you want to see.</span></span>

1. <span data-ttu-id="df1e0-123">Щелкните **Ссылку /Beta** , чтобы открыть документы бета-версии.</span><span class="sxs-lookup"><span data-stu-id="df1e0-123">Click **/Beta Reference** to open the beta docs.</span></span>
2. <span data-ttu-id="df1e0-124">Прокрутите список вниз и выберите **Intune**.</span><span class="sxs-lookup"><span data-stu-id="df1e0-124">Scroll down and click **Intune**.</span></span>
3. <span data-ttu-id="df1e0-125">Продолжайте щелкать элемент для части API-интерфейса подразделах ниже **Intune** вы</span><span class="sxs-lookup"><span data-stu-id="df1e0-125">Continue to click subsections below **Intune** for the parts of the API you</span></span> 
