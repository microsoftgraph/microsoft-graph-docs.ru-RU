---
title: Использование API Graph для Intune — API Microsoft Graph
description: Перечисление API Microsoft Graph для коечных точек Intune (REST), которые можно использовать для управления организацией клиента, его устройствами, приложениями, доступом и ресурсами.
author: rolyon
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: e1c93c38c1667d1681e280b69ff106060900b46c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031118"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="0a93d-103">Работа с Intune в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0a93d-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="0a93d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a93d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a93d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a93d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a93d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a93d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a93d-107">API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.</span><span class="sxs-lookup"><span data-stu-id="0a93d-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="0a93d-108">В сценариях управления мобильными устройствами (MDM) API Microsoft Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="0a93d-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="0a93d-109">Использование API Microsoft Graph для Intune</span><span class="sxs-lookup"><span data-stu-id="0a93d-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="0a93d-110">Intune предоставляет данные для Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.</span><span class="sxs-lookup"><span data-stu-id="0a93d-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="0a93d-111">С помощью Microsoft Graph вы можете объединить данные из других служб и Intune, чтобы создать используемые в разных службах полнофункциональные приложения для ИТ-специалистов и пользователей.</span><span class="sxs-lookup"><span data-stu-id="0a93d-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="0a93d-112">В приведенном ниже примере показано, как определить, установлено ли приложение на устройстве пользователя.</span><span class="sxs-lookup"><span data-stu-id="0a93d-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="0a93d-113">Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя:</span><span class="sxs-lookup"><span data-stu-id="0a93d-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="0a93d-114">Затем просмотрите список приложений для вашего клиента:</span><span class="sxs-lookup"><span data-stu-id="0a93d-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="0a93d-115">На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):</span><span class="sxs-lookup"><span data-stu-id="0a93d-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="0a93d-116">Использование разрешений Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0a93d-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="0a93d-117">Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения.</span><span class="sxs-lookup"><span data-stu-id="0a93d-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="0a93d-118">Разработчикам необходимо указать разрешения, необходимые для доступа к ресурсам Intune.</span><span class="sxs-lookup"><span data-stu-id="0a93d-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="0a93d-119">Как правило, разрешения указываются на портале Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a93d-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="0a93d-120">Дополнительные сведения см. в статье [Справочник по разрешениям Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a93d-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span>

## <a name="whats-new"></a><span data-ttu-id="0a93d-121">Что нового</span><span class="sxs-lookup"><span data-stu-id="0a93d-121">What's new</span></span>
<span data-ttu-id="0a93d-122">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="0a93d-122">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0a93d-123">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="0a93d-123">Next Steps</span></span>

- <span data-ttu-id="0a93d-124">Узнайте, [как использовать Azure AD](https://docs.microsoft.com/intune/intune-graph-apis) для доступа к API Microsoft Graph для Intune.</span><span class="sxs-lookup"><span data-stu-id="0a93d-124">Learn [how to use Azure AD](https://docs.microsoft.com/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="0a93d-125">Изучите [примеры PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples), демонстрирующие способ использования API Microsoft Graph для Intune в рабочем контексте.</span><span class="sxs-lookup"><span data-stu-id="0a93d-125">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>




