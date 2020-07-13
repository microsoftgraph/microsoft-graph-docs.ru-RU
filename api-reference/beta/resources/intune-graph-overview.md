---
title: Использование API Graph для Intune — API Microsoft Graph
description: Перечисление API Microsoft Graph для коечных точек Intune (REST), которые можно использовать для управления организацией клиента, его устройствами, приложениями, доступом и ресурсами.
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: 789c461fcac36c82d3dee3a7d0f8db9a159bd333
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353499"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="284c0-103">Работа с Intune в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="284c0-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="284c0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="284c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="284c0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="284c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="284c0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="284c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="284c0-107">API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.</span><span class="sxs-lookup"><span data-stu-id="284c0-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="284c0-108">В сценариях управления мобильными устройствами (MDM) API Microsoft Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/ru-RU/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="284c0-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/ru-RU/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="284c0-109">Использование API Microsoft Graph для Intune</span><span class="sxs-lookup"><span data-stu-id="284c0-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="284c0-110">Intune предоставляет данные для Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.</span><span class="sxs-lookup"><span data-stu-id="284c0-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="284c0-111">С помощью Microsoft Graph вы можете объединить данные из других служб и Intune, чтобы создать используемые в разных службах полнофункциональные приложения для ИТ-специалистов и пользователей.</span><span class="sxs-lookup"><span data-stu-id="284c0-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="284c0-112">В приведенном ниже примере показано, как определить, установлено ли приложение на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="284c0-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="284c0-113">Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя:</span><span class="sxs-lookup"><span data-stu-id="284c0-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="284c0-114">Затем просмотрите список приложений для вашего клиента:</span><span class="sxs-lookup"><span data-stu-id="284c0-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="284c0-115">На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):</span><span class="sxs-lookup"><span data-stu-id="284c0-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="284c0-116">Использование разрешений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="284c0-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="284c0-117">Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения.</span><span class="sxs-lookup"><span data-stu-id="284c0-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="284c0-118">Разработчикам необходимо указать разрешения, необходимые для доступа к ресурсам Intune.</span><span class="sxs-lookup"><span data-stu-id="284c0-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="284c0-119">Как правило, разрешения указываются на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="284c0-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="284c0-120">Дополнительные сведения см. в статье [Справочник по разрешениям Microsoft Graph](https://docs.microsoft.com/ru-RU/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="284c0-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/ru-RU/graph/permissions-reference).</span></span>

## <a name="whats-new"></a><span data-ttu-id="284c0-121">Что нового</span><span class="sxs-lookup"><span data-stu-id="284c0-121">What's new</span></span>
<span data-ttu-id="284c0-122">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="284c0-122">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="284c0-123">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="284c0-123">Next Steps</span></span>

- <span data-ttu-id="284c0-124">Узнайте, [как использовать Azure AD](https://docs.microsoft.com/ru-RU/intune/intune-graph-apis) для доступа к API Microsoft Graph для Intune.</span><span class="sxs-lookup"><span data-stu-id="284c0-124">Learn [how to use Azure AD](https://docs.microsoft.com/ru-RU/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="284c0-125">Изучите [примеры PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples), демонстрирующие способ использования API Microsoft Graph для Intune в рабочем контексте.</span><span class="sxs-lookup"><span data-stu-id="284c0-125">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

